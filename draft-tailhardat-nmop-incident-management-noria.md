---
title: "Knowledge Graphs for Enhanced Cross-Operator Incident Management and Network Design"
abbrev: "Knowledge Graphs & Incident Management"
category: info

docname: draft-tailhardat-nmop-incident-management-noria-latest
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
number: 00
date: 2024-06-27
consensus: true
v: 3
area: "Operations and Management"
workgroup: "Network Management Operations"
keyword:
- knowledge graphs
- incident management
- anomaly detection
#venue:
#  group: WG
#  type: Working Group
#  mail: WG@example.com
#  arch: https://example.com/WG
#  github: USER/REPO
#  latest: https://example.com/LATEST

author:
 -
    fullname: Lionel Tailhardat
    organization: Orange
    email: "lionel.tailhardat@orange.com"
 -
    fullname: Raphaël Troncy
    organization: EURECOM
    email: raphael.troncy@eurecom.fr
 -
    fullname: Yoan Chabot
    organization: Orange
    email: yoan.chabot@orange.com

normative:

informative:


--- abstract

TODO Abstract


--- middle

# Introduction

TODO Introduction


# Conventions and Definitions

{::boilerplate bcp14-tagged}


# Security Considerations

TODO Security

~~~~ ascii-art
               ┌──────────┐   ┌────────────────┐   ┌──────────┐   ┌───────────────┐   ┌────────┐
┌──────────┐   │          │   │                │   │          │   │               │   │┌──────┐│
│  Events  │──►│  E.S.B.  ├──►│ Stream mapping ├──►│  S.S.B.  ├──►│ Stream loader ├──►││ K.G. ││
└──────────┘   │          │   │                │   │          │   │               │   │└──────┘│
               └──────────┘   └────────────────┘   └────┬─────┘   └───────────────┘   └────────┘
                                                        │
                                    ┌───────────────────┴──────────────────────┐
                                    │(event/LOG_login_03)=>(object/RES/router1)│
                                    └─┌──────────────────────────────────────────┐
                                      │(event/LOG_login_03)=>(object/RES/router1)│
                                      └─┌──────────────────────────────────────────┐
                                        │(event/LOG_login_03)=>(object/RES/router1)│
                                        └──────────────────────────────────────────┘
~~~~
{: #fig-stream-kg-only title="KG-only data integration architecture for event data streams"}

~~~~ ascii-art
                         <object/RES_router3>
<object/RES_router2>          │
               │              │            ┌────────┐
             <object/RES_router1>─rdf:type─┤Resource│
                       │                   └────────┘
                       │
          logOriginatingManagedObject
                       │
             <event/LOG_login_01>             ┌───────────┐
               <event/LOG_login_02>──rdf:type─┤EventRecord│
                 <event/LOG_login_03>         └───────────┘
~~~~
{: #fig-stream-kg-only-kr title="Resulting knowledge representation for the KG-only data integration architecture for event data streams"}

~~~~ ascii-art
                              ┌────────────────┐
                              │    Complex     │
                              │     Event      │
                              │   Processing   │
                              └───────┬┬───────┘
               ┌──────────┐   ┌───────┴┴───────┐   ┌──────────┐   ┌───────────────┐   ┌────────┐
┌──────────┐   │          │   │                │   │          │   │               │   │┌──────┐│
│  Events  │──►│  E.S.B.  ├──►│ Stream mapping ├──►│  S.S.B.  ├──►│ Stream loader ├──►││ K.G. ││
└──────────┘   │          │   │                │   │          │   │               │   │└──────┘│
               └────────┬─┘   └────────────────┘   └────┬─────┘   └───────────────┘   └────────┘
                        │                               │
                        │           ┌───────────────────┴──────────────────────┐
                        │           │(event/AIS_login_01)=>(object/RES/router1)│
                        │           └──────────────────────────────────────────┘
                        │
                        │                                         ┌───────────────┐   ┌────────┐
                        │                                         │               │   │┌──────┐│
                        └────────────────────────────────────────►│ Stream loader ├──►││ TSDB ││
                                                                  │               │   │└──────┘│
                                                                  └───────────────┘   └────────┘
~~~~
{: #fig-stream-mixed title="Mixed KG/non-KG data integration architecture for event data streams"}


~~~~ ascii-art
                                <object/RES_router3>
       <object/RES_router2>          │
                      │              │            ┌────────┐
                    <object/RES_router1>─rdf:type─┤Resource│
                              │                   └────────┘
                              │
                 logOriginatingManagedObject
                              │                    ┌───────────┐
┌──────────────────►<event/AIS_login_01>──rdf:type─┤EventRecord│
│                    │              │ │            └───────────┘
│                duration           │ │
│                    │              │ │
│  "P0Y0M0DT0H3M30S"^^xsd:duration  │ └─dcterms:type─<Notification/EventType/inferredAlert>
│                                   │                                │
│                              loggingTime                        rdf:type
│                                   │                          ┌─────┴──────┐
│                 "2024-02-07T16:22:42Z"^^xsd:dateTime         │skos:Concept│
│                                                              └────────────┘
│  KG knowledge representation
│  ========================================================================================
│  Time series database (TSDB) data representation
│
│
│  Timestamp             Origin                Event
│  2024-02-07T16:22:42Z  <object/RES_router1>  Login Attempt
│  2024-02-07T16:23:13Z  <object/RES_router1>  Login Attempt
│  2024-02-07T16:26:12Z  <object/RES_router1>  Login Attempt
│                                 ▲
└──shared─identifier──────────────┘
~~~~
{: #fig-stream-mixed-kr title="Resulting knowledge representation for the mixed KG/non-KG data integration architecture for event data streams"}


~~~~ ascii-art
Data domain &   ───On-premise────────────────────────────   ┌─┐  Scope-based querying
access policy   ┌───────┐                                   │ │
                │┌─────┐│  ┌──────┐           ┌─────────┐   │ │           ┌───────────┐
  Domain A ────►││ KG  ││◄─┤KGDBMS├───────────┤SPARQL EP├──►│ ├─Network &─┤  NetOps   │
   -   UG2      │└─────┘│  └──────┘           └─────────┘   │ ├─Usage─────┤Application│
                └───────┘                                   │ │           └───────────┘
                ┌───────┐                                   │ │           ┌───────────┐
                │┌─────┐│  ┌──────┐           ┌─────────┐   │ ├─Network &─┤  SecOps   │
  Domain B ────►││ KG  ││◄─┤KGDBMS├───────────┤SPARQL EP├──►│ ├─Security──┤Application│
  UG1   -       │└─────┘│  └──────┘           └─────────┘   │F│           └───────────┘
                └─────┬─┘                                   │E│
                      └─────────────────────────────────────│D│─────────────┐
                ───On-premise / public-cloud─────────────   │E│             │
                ┌───────┐                                   │R│             ▼  Usage
                │┌─────┐│  ┌──────┐ ┌───┐     ┌─────────┐   │A│           ┌────scope──┐
  Domain C ────►││ RDB ││◄─┤RDBMS ├─┤VKG├─────┤SPARQL EP├──►│T│           │*          │
  UG1 & UG2     │└─────┘│  └──────┘ └───┘     └─────────┘   │E│   Network │   *  *    │
                └───────┘                                   │D│   scope───│────────┐  │
                ┌───────┐                                   │ │       │   │ *  *   │  │
                │┌─────┐│  ┌──────┐ ┌───┐     ┌─────────┐   │Q│       │  *└───────────┘
  Domain D ────►││NoSQL││◄─┤RDBMS ├─┤VKG├─────┤SPARQL EP├──►│U│       │  ┌───────────┐
  UG1   -       │└─────┘│  └──────┘ └───┘     └─────────┘   │E│       │* │ *  *    │ │
                └───────┘                                   │R│       └──│─────────┘ │
                ┌───────┐                                   │I│        ▲ │     *     │
                │┌─────┐│  ┌──────┐ ┌───────┐ ┌─────────┐   │E│        │ │ *       * │
  Domain E ────►││ LPG ││◄─┤GDBMS ├─│QL tlt.├─┤SPARQL EP│──►│S│        │ └──Security─┘
   -   UG2      │└─────┘│  └──────┘ └───────┘ └─────────┘   │ │        │    scope ▲
                └───┬───┘                                   │ │        │          │
                    └───────────────────────────────────────│ │────────┼──────────┘
                                                            │ │        │
                ───Public-cloud──────────────────────────   │ │        │
                ┌───────┐                                   │ │        │
                │┌─────┐│  ┌──────┐           ┌─────────┐   │ │        │
  Domain F ────►││ KG  ││◄─┤KGDBMS├───────────┤SPARQL EP├──►│ │        │
  UG1 & UG2     │└─────┘│  └──────┘           └─────────┘   │ │        │
                └───┬───┘                                   └─┘        │
                    └──────────────────────────────────────────────────┘
~~~~
{: #fig-multi-store title="Unified access to data distributed across various technological platforms"}

# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
