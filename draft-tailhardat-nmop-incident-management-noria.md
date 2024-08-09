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
venue:
  group: "Network Management Operations"
  type: "Working Group"
  mail: "nmop@ietf.org"
  arch: "https://mailarchive.ietf.org/arch/browse/nmop/"
  github: "genears/draft-tailhardat-nmop-incident-management-noria"
  latest: "https://genears.github.io/draft-tailhardat-nmop-incident-management-noria/draft-tailhardat-nmop-incident-management-noria.html"

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
  OWL:
    title: "OWL 2 Web Ontology Language Document Overview (Second Edition)"
    author:
      organization: W3C
    target: https://www.w3.org/TR/owl2-overview/
    date: December 2012

  RDF:
    title: "Resource Description Framework (RDF): Concepts and Abstract Syntax"
    author:
      organization: W3C
    target: https://www.w3.org/TR/rdf11-concepts/
    date: February 2014

  RDFS:
    title: "RDF Schema 1.1"
    author:
      organization: W3C
    target: https://www.w3.org/TR/rdf-schema/
    date: February 2014

  SPARQL11-QL:
    title: "SPARQL 1.1 Query Language"
    author:
      organization: W3C
    target: https://www.w3.org/TR/sparql11-query/
    date: March 2013

  SPARQL11-FQ:
    title: "SPARQL 1.1 Federated Query"
    author:
      organization: W3C
    target: https://www.w3.org/TR/sparql11-federated-query/
    date: March 2013

  SKOS:
    title: "SKOS Simple Knowledge Organization System Reference"
    author:
      organization: W3C
    target: https://www.w3.org/TR/skos-reference/
    date: 18 August 2009

informative:
  I.D.draft-marcas-nmop-knowledge-graph-yang:
    title: "Knowledge Graphs for YANG-based Network Management"
    seriesinfo:
      Internet-Draft: draft-marcas-nmop-knowledge-graph-yang-03
    author:
      - name: I.D. Martinez-Casanueva
      - name: L. Cabanillas
    target: https://datatracker.ietf.org/doc/draft-marcas-nmop-knowledge-graph-yang/
    date: 5 July 2024

  I.D.draft-netana-nmop-network-anomaly-lifecycle:
    author:
      - name: A. Roberto
      - name: T. Graf
      - name: W. Du
      - name: A. Huang Feng
    title: "Experiment: Network Anomaly Lifecycle"
    seriesinfo:
      Internet-Draft: draft-netana-nmop-network-anomaly-lifecycle-03
    date: 8 July 2024
    target: https://datatracker.ietf.org/doc/draft-netana-nmop-network-anomaly-lifecycle/

  I.D.draft-netana-nmop-network-anomaly-semantics:
    author:
      - name: T. Graf
      - name: W. Du
      - name: A. Huang Feng
      - name: V. Riccobene
      - name: A. Roberto
    title: "Semantic Metadata Annotation for Network Anomaly Detection"
    seriesinfo:
      Internet-Draft: draft-netana-nmop-network-anomaly-semantics-02
    date: 7 July 2024
    target: https://datatracker.ietf.org/doc/draft-netana-nmop-network-anomaly-semantics/

  I.D.draft-boucadair-nmop-rfc3535-20years-later:
    author:
      - name: Mohamed Boucadair
      - name: Luis M. Contreras
      - name: Oscar Gonzalez de Dios
      - name: Thomas Graf
      - name: Reshad Rahman
    title: "RFC 3535, 20 Years Later: An Update of Operators Requirements on Network Management Protocols and Modelling"
    seriesinfo:
      Internet-Draft: draft-boucadair-nmop-rfc3535-20years-later-04
    date: 22 July 2024
    target: https://datatracker.ietf.org/doc/draft-boucadair-nmop-rfc3535-20years-later/

  I.D.draft-irtf-nmrg-network-digital-twin-arch:
    author:
      - name: Cheng Zhou
      - name: Hongwei Yang
      - name: Xiaodong Duan
      - name: Diego Lopez
      - name: Antonio Pastor
      - name: Qin Wu
      - name: Mohamed Boucadair
      - name: Christian Jacquenet
    title: "Network Digital Twin: Concepts and Reference Architecture"
    seriesinfo:
      Internet-Draft: draft-irtf-nmrg-network-digital-twin-arch-06
    date: 7 July 2024
    target: https://datatracker.ietf.org/doc/draft-irtf-nmrg-network-digital-twin-arch/

  NORIA-O-2024:
    author:
      - name: Lionel Tailhardat
      - name: Raphaël Troncy
      - name: Yoan Chabot
    title: "NORIA-O: An Ontology for Anomaly Detection and Incident Management in ICT Systems"
    date: 2024
    target: https://doi.org/10.1007/978-3-031-60635-9_2

  SLKG-2023:
    author:
      - name: Lionel Tailhardat
      - name: Raphaël Troncy
      - name: Yoan Chabot
    title: "Leveraging Knowledge Graphs For Classifying Incident Situations in ICT Systems"
    date: 2023
    target: https://doi.org/10.1145/3600160.3604991

  GPL-2024:
    author:
      - name: Lionel Tailhardat
      - name: Benjamin Stach
      - name: Yoan Chabot
      - name: Raphaël Troncy
    title: "Graphameleon: Relational Learning and Anomaly Detection on Web Navigation Traces Captured as Knowledge Graphs"
    date: 2024
    target: https://doi.org/10.1145/3589335.3651447

  NORIA-UI-2024:
    author:
      - name: Lionel Tailhardat
      - name: Yoan Chabot
      - name: Antoine Py
      - name: Perrine Guillemette
    title: "NORIA UI: Efficient Incident Management on Large-Scale ICT Systems Represented as Knowledge Graphs"
    date: 2024
    target: https://doi.org/10.1145/3664476.3670438

  FLAGSM-2021:
    author:
      - name: Bram Steenwinckel
      - name: Dieter De Paepe
      - name: Sander Vanden Hautte
      - name: Pieter Heyvaert
      - name: Mohamed Bentefrit
      - name: Pieter Moens
      - name: Anastasia Dimou
      - name: Bruno Van Den Bossche
      - name: Filip De Turck
      - name: Sofie Van Hoecke
      - name: Femke Ongenae
    title: "FLAGS: A Methodology for Adaptive Anomaly Detection and Root Cause Analysis on Sensor Data Streams by Fusing Expert Knowledge with Machine Learning"
    date: 2021
    target: https://doi.org/10.1016/j.future.2020.10.015

  FOLIO-2018:
    author:
      - name: Bram Steenwinckel
      - name: Pieter Heyvaert
      - name: Dieter De Paepe
      - name: Olivier Janssens
      - name: Sander Vanden Hautte
      - name: Anastasia Dimou
      - name: Filip De Turck
      - name: Sofie Van Hoecke
      - name: Femke Ongenae
    title: "Towards Adaptive Anomaly Detection and Root Cause Analysis by Automated Extraction of Knowledge from Risk Analyses"
    date: 2018
    target: https://www.ceur-ws.org/Vol-2213/paper2.pdf

  DevOpsInfra-2021:
    author:
      - name: Oscar Corcho
      - name: David Chaves-Fraga
      - name: Jhon Toledo
      - name: Juli{\'a}n Arenas-Guerrero
      - name: Carlos Badenes-Olmedo
      - name: Mingxue Wang
      - name: Hu Peng
      - name: Nicholas Burrett
      - name: Jos{\'e} Mora
      - name: Puchao Zhang
    title: "A High-Level Ontology Network for ICT Infrastructures"
    date: 2021
    target: https://doi.org/10.1007/978-3-030-88361-4_26


--- abstract

Incident management on telecom and computer networks requires the ability to simultaneously and quickly correlate and interpret a large number of heterogeneous technical information sources.
Knowledge graphs, by structuring heterogeneous data through shared vocabularies, enable the provision of a unified view of complex technical systems and their dynamics.
Similarly, YANG data models enable describing networks configurations and automating the deployment of these configurations.
However, both knowledge graphs and YANG formalisms suffer vocabulary alignment and adoption challenges that hinders the learning and sharing of knowledge on network designs failure modes and best practices to adopt towards an overall improvement of IT systems and the Internet.
To adress these challenges, this document introduces the concept of meta-knowledge graph to leverage already existing network infrastructure descriptions in YANG format while enabling abstract reasoning on the networks behaviors.
It also describes an experiment to carry-out to assess the meta-knowledge graph proposal, learn pros & cons of it, and evaluate its potential for solving continuous improvement of network quality & designs challenges.

--- middle

# Introduction

Incident management on telecom and computer networks, whether it is related to infrastructure or cybersecurity issues, requires the ability to simultaneously and quickly correlate and interpret a large number of heterogeneous technical information sources.
Knowledge Graphs (KGs), by structuring heterogeneous data through shared vocabularies, enable the provision of a unified view of complex technical systems, their ecosystem, and the activities and operations related to them (see {{I.D.draft-marcas-nmop-knowledge-graph-yang}} and {{NORIA-O-2024}}).
Using such formal knowledge representation allows for a simplified interpretation of networks and their behavior, both for NetOps & SecOps teams and artificial intelligence (AI) algorithms (e.g. anomaly detection, root cause analysis, diagnostic aid, situation summarization), and paves the way, in line with the Network Digital Twin vision {{I.D.draft-irtf-nmrg-network-digital-twin-arch}}, for the development of tools for detecting and analyzing complex network incident situations through explainable, actionable, and shareable models (see {{FOLIO-2018}}, {{SLKG-2023}}, and {{GPL-2024}}).

However, despite potential benefits of using knowledge graphs, these are not mainstream yet in commercial network deployment systems and decision support systems (see {{NORIA-UI-2024}} for more on the decision support systems perspective).
YANG is a widely used standard among operators for describing networks configurations and automating the deployment of these configurations.
Using YANG representations in the form of a KG, as suggested in {{I.D.draft-marcas-nmop-knowledge-graph-yang}}, would minimize the effort required to adapt network management tools towards the unified vision and applications evoked above.
The lack of alignment between various YANG models on key concepts (e.g. for describing network topology) is, however, hindering this evolution {{I.D.draft-boucadair-nmop-rfc3535-20years-later}}.

Furthermore, although {{I.D.draft-netana-nmop-network-anomaly-lifecycle}} addresses the capitalization of incident management knowledge through a YANG model, it can be observed that the overall scope of YANG models does not naturally cover the description of the networks' ecosystem (e.g. physical equipment location, operator organization, supervision systems) or the description of network operations from an IT service management (ITSM) perspective (e.g. business processes and design rules used by the company, scheduled modification operations, remediation actions performed during incident handling).
As a consequence, the continuous improvement of network quality & designs requires additional data cross-referencing operations to properly contextualize incidents and learn from remediation actions taken (e.g. analyzing intervention technicians' verbatim, comparing actions performed on similar incidents but occurring on different networks).
As a result of these additional efforts of contextualization, the capitalization of knowledge typically remains confined at the level of each network operator.
This, in turn, hinders the sharing of information within the community of researchers and system designers regarding failure modes and best practices to adopt, considering the concept of overall improvement of IT systems and the Internet.

Realizing an ITSM knowledge graph for network deployment, anomaly detection and risk management applications has been studied for several years in the Semantic Web community (i.e. knowledge representation and automated reasoning leveraging Web technologies such as {{RDF}}, {{RDFS}}, {{OWL}}, and {{SKOS}}).
Among other examples: the DevOpsInfra ontology {{DevOpsInfra-2021}} allows for describing sets of computing resources and how they are allocated for hosting services; the NORIA-O ontology {{NORIA-UI-2024}} allows for describing a network infrastructure & ecosystem, its events, diagnosis and repair actions performed during incident management.

TODO Introduction

# Conventions and Definitions

{::boilerplate bcp14-tagged}

# A meta-KG to align operator-specificities and share behavioral models of technical architectures

## Aligning operator-specificities with a multi-faceted knowledge graph

## Learning and sharing behavioral models

## NetOps perspective

## SecOps perspective

## Experiments

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

We would like to thank Benoit Claise for spontaneously seeking to include the work of the NORIA research project in the vision of the NMOP working group through direct contact.
