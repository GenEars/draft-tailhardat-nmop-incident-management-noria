---
title: "Knowledge Graphs for Enhanced Cross-Operator Incident Management and Network Design"
abbrev: "Knowledge Graphs & Incident Management"
category: info

docname: draft-tailhardat-nmop-incident-management-noria-latest
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"

#number: 00
#date: 2024-06-27

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

informative:
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

  NORIA-DI-2023:
    author:
      - name: Lionel Tailhardat
      - name: Raphaël Troncy
      - name: Yoan Chabot
    title: "Designing NORIA: a Knowledge Graph-based Platform for Anomaly Detection and Incident Management in ICT Systems"
    date: 2023
    target: https://ceur-ws.org/Vol-3471/paper3.pdf

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

  SemNIDS-2023:
    author:
      - name: Dario Ferrero
      - name: Yash Agarwalla
      - name: Lionel Tailhardat
      - name: Thibault Ehrhart
    title: "SemNIDS, bringing semantics into Network Intrusion Detection Systems"
    date: 2023
    target: https://github.com/D2KLab/SemNIDS

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

  AMO-2012:
    author:
      - name: Michel Buffa
      - name: Catherine Faron-Zucker
    title: "Ontology-Based Access Rights Management"
    date: 2012
    target: https://doi.org/10.1007/978-3-642-25838-1_3


--- abstract

Operational efficiency in incident management on telecom and computer networks requires correlating and interpreting large volumes of heterogeneous technical information.
Knowledge graphs can provide a unified view of complex systems through shared vocabularies.
YANG data models enable describing network configurations and automating their deployment.
However, both approaches face challenges in vocabulary alignment and adoption, hindering knowledge capitalization and sharing on network designs and best practices.
To address this, the concept of a IT Service Management (ITSM) Knowledge Graph (KG) is introduced to leverage existing network infrastructure descriptions in YANG format and enable abstract reasoning on network behaviors.
The principle of ITSM-KG is to transform YANG representations of network infrastructures into an equivalent knowledge graph representation, and then embed it into a more extensive data model for Anomaly Detection (AD) and Risk Management applications.
An experiment is proposed to assess the potential of the ITSM-KG in improving network quality and designs.


--- middle

# Introduction

Incident management on telecom and computer networks, whether it is related to infrastructure or cybersecurity issues, requires the ability to simultaneously and quickly correlate and interpret a large number of heterogeneous technical information sources.
Knowledge Graphs (KGs), by structuring heterogeneous data through shared vocabularies, enable providing a unified view of complex technical systems, their ecosystem, and the activities and operations related to them (see {{?I-D.marcas-nmop-knowledge-graph-yang}} and {{NORIA-O-2024}}).
Using such formal knowledge representation allows for a simplified interpretation of networks and their behavior, both for NetOps & SecOps teams and artificial intelligence (AI) algorithms (e.g. anomaly detection, root cause analysis, diagnostic aid, situation summarization), and paves the way, in line with the Network Digital Twin vision {{?I-D.irtf-nmrg-network-digital-twin-arch}}, for the development of tools for detecting and analyzing complex network incident situations through explainable, actionable, and shareable models (see {{FOLIO-2018}}, {{SLKG-2023}}, and {{GPL-2024}}).

However, despite potential benefits of using knowledge graphs, these are not mainstream yet in commercial network deployment systems and decision support systems (see {{NORIA-UI-2024}} for more on the decision support systems perspective).
YANG is a widely used standard among operators for describing network configurations and automating their deployment.
Using YANG representations in the form of a KG, as suggested in {{?I-D.marcas-nmop-knowledge-graph-yang}}, would minimize the effort required to adapt network management tools towards the unified vision and applications evoked above.
The lack of alignment between various YANG models on key concepts (e.g. for describing network topology) is, however, hindering this evolution {{?I-D.boucadair-nmop-rfc3535-20years-later}}.

Furthermore, although {{?I-D.netana-nmop-network-anomaly-lifecycle}} addresses the capitalization of incident management knowledge through a YANG model, it can be observed that the overall scope of YANG models does not naturally cover the description of the networks' ecosystem (e.g. physical equipment location, operator organization, supervision systems) or the description of network operations from an IT service management (ITSM) perspective (e.g. business processes and design rules used by the company, scheduled modification operations, remediation actions performed during incident handling).
As a consequence, the continuous improvement of network quality & designs requires additional data cross-referencing operations to properly contextualize incidents and learn from remediation actions taken (e.g. analyzing intervention technicians' verbatim, comparing actions performed on similar incidents but occurring on different networks).
As a result of these additional efforts of contextualization, the capitalization of knowledge typically remains confined at the level of each network operator.
This, in turn, hinders the sharing of information within the community of researchers and system designers regarding failure modes and best practices to adopt, considering the concept of overall improvement of IT systems and the Internet.

Realizing an ITSM knowledge graph for network deployment, anomaly detection and risk management applications has been studied for several years in the Semantic Web community (i.e. knowledge representation and automated reasoning leveraging Web technologies such as {{RDF}}, {{RDFS}}, {{OWL}}, and {{SKOS}}).
Among other examples: the DevOpsInfra ontology {{DevOpsInfra-2021}} allows for describing sets of computing resources and how they are allocated for hosting services; the NORIA-O ontology {{NORIA-O-2024}} allows for describing a network infrastructure & ecosystem, its events, diagnosis and repair actions performed during incident management.
Assuming the continuous integration into a knowledge graph of data from ticketing systems, network monitoring solutions, and network configuration management databases, we remark that the resulting knowledge graph ({{fig-incident-context}}) implicitely holds the necessary information to (automatically) learn incident contexts (i.e. the network topology, its set of states and set of events prior to the incident) and remediation procedures (i.e. the set of actions and network configuration changes carried-out to resolve the incident).

~~~~ ascii-art
┌───Incident context────────────────────────────┐
│                 ┌────────────┐                │
│                 │skos:Concept│                │
│                 └─┬┬─────────┘                │
│                  <server>                     │
│                    ▲                          │
│                    │                          │
│                 resourceType                  │
│         ┌────────┐ │                          │      ┌─────────────┐
│         │Resource│ │                          │      │TroubleTicket│
│         └──────┬┬┘ │                          │      └─────┬┬──────┘
│                ││  │                          │            ││
│        <ne_2>──<ne_1>◄──troubleTicketRelatedResource──<incident_01>
│           │      │                            │            │
│           │      │                            │      problemCategory
│<ne_5>──<ne_4>────┼──<ne_3>────<log_2>         │            │
│           │      │    │                       │            ▼
│           │      │    │                       │       <packet-loss>
│       <log_3>    │  <ne_6>                    │            ││
│                  │                            │       ┌────┴┴──────┐
│     logOriginatingManagedObject               │       │skos:Concept│
│                  │                            │       └────────────┘
│                  ▼                            │
│               <log_1>──────┐                  │
│      ┌─────────┴┴┐     dcterms:type           │
│      │EventRecord│         │                  │
│      └───────────┘         ▼                  │
│                    <integrityViolation>       │
│                       ┌────┴┴──────┐          │
│                       │skos:Concept│          │
│                       └────────────┘          │
└───────────────────────────────────────────────┘
~~~~
{: #fig-incident-context title="Learning an incident signature seen as a classification model that is trained on the relationship of the incident context (i.e. a subgraph centered around a Resource entity concerned by a given TroubleTicket) to the problem class defined at the TroubleTicket entity level. Arrows are for object properties (owl:ObjectProperty), double line edges are for object class relationships (rdf:type)."}

By going a step further, we notice that a generic understanding of incident context can be extracted and shared among operators from knowledge graphs.
Indeed, a knowledge graph, being an instantiation of shared vocabularies (e.g. RDFS/OWL ontologies and controlled vocabularies in SKOS syntax), sharing incident signatures can be done without revealing infrastructure details (e.g. hostname, IP address), but rather the abstract representation of the network (i.e. the class of the knowledge graph entities and relationships, such as "server" or "router", and or "IPoWDM link").

The remainder of this document is organized as follows.
Firstly, the concept of a *meta-knowledge graph* is introduced to leverage existing network infrastructure descriptions in YANG format and enable abstract reasoning on network behaviors.
Secondly, an experiment is proposed to assess the potential of the meta-knowledge graph in improving network quality and designs.
In addition to the main parts of the proposal, the document also covers data integration and data federation architectures in the Security Considerations section. This section specifically addresses the handling of event data streams and the provision of a unified view for different stakeholders.

# Conventions and Definitions

{::boilerplate bcp14-tagged}

# A meta-knowledge graph to align operator-specificities and share behavioral models of technical architectures

TODO Introduce and develop the following topics.

Topics:

* Principles for implicit learning of incident characteristics and resolution methods through a graph and activity tracing.
  - Aligning operator-specificities with a multi-faceted knowledge graph.
  - Learning and sharing behavioral models.
  - Relation to the Network Anomaly Lifecycle experiment {{?I-D.netana-nmop-network-anomaly-lifecycle}}.
  - Relation to the Digital Map concept {{?I-D.havel-nmop-digital-map-concept}}.

* Meta-KG construction
  - Integrating Service and Network topology data from YANG data models, such as Network Topologies {{!RFC8345}} and Service Assurance {{!RFC9418}}}.
  - Relation to the NORIA-O ontology {{NORIA-O-2024}}.
  - Trends towards some Yang to OWL / Yang to RDF data transformation tool.

* Experiments towards the meta-KG proposal.

## Aligning operator-specificities with a multi-faceted knowledge graph

TODO Meta-KG construction

TODO Relate the Meta-KG construction part to the following REQ-DM-SCALES related considerations.

The following figures illustrate different scenarios for constructing a meta-KG through an Extract-Transform-Load (ETL) data integration pipeline.
From the perspective of the Digital Map Requirements ({{sec-digital-map}}), the {{fig-stream-mixed}}, {{fig-stream-mixed-kr}} and {{fig-multi-store}} particularly address the REQ-DM-SCALES requirement.

~~~~ ascii-art
          ┌──────┐  ┌─────────┐  ┌──────┐  ┌────────┐  ┌──────┐
┌──────┐  │      │  │ Stream  │  │      │  │ Stream │  │┌────┐│
│Events├─►│E.S.B.├─►│ mapping ├─►│S.S.B.├─►│ loader ├─►││K.G.││
└──────┘  │      │  │         │  │      │  │        │  │└────┘│
          └──────┘  └─────────┘  └──┬───┘  └────────┘  └──────┘
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
                  ┌────────────┐
                  │  Complex   │
                  │   Event    │
                  │ Processing │
                  └────┬──┬────┘
          ┌──────┐  ┌──┴──┴───┐  ┌──────┐  ┌────────┐  ┌──────┐
┌──────┐  │      │  │ Stream  │  │      │  │ Stream │  │┌────┐│
│Events├─►│E.S.B.├─►│ mapping ├─►│S.S.B.├─►│ loader ├─►││K.G.││
└──────┘  │      │  │         │  │      │  │        │  │└────┘│
          └──┬───┘  └─────────┘  └──┬───┘  └────────┘  └──────┘
             │                      │
             │  ┌───────────────────┴──────────────────────┐
             │  │(event/AIS_login_01)=>(object/RES/router1)│
             │  └──────────────────────────────────────────┘
             │                             ┌────────┐  ┌──────┐
             │                             │ Stream │  │┌────┐│
             └────────────────────────────►│ loader ├─►││TSDB││
                                           │        │  │└────┘│
                                           └────────┘  └──────┘
~~~~
{: #fig-stream-mixed title="Mixed KG/non-KG data integration architecture for event data streams"}


~~~~ ascii-art
                                <object/RES_router3>
       <object/RES_router2>          │
                      │              │            ┌────────┐
                    <object/RES_router1>─rdf:type─┤Resource│
                              │                   └────────┘
                 logOriginatingManagedObject
                              │                    ┌───────────┐
┌──────────────────►<event/AIS_login_01>──rdf:type─┤EventRecord│
│                    │             │  \            └───────────┘
│                duration          │   \
│                    │             │ dcterms:type
│  "P0Y0M0DT0H3M30S"^^xsd:duration │     \
│                                  │   <Notification/
│                          loggingTime   EventType/inferredAlert>
│                                  │                   │
│        "2024-02-07T16:22:42Z"^^xsd:dateTime       rdf:type
│                                                ┌─────┴──────┐
│                                                │skos:Concept│
│  KG knowledge representation                   └────────────┘
│  ==============================================================
│  Time series database (TSDB) data representation
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
  ───On-premise────────────────────────────  ┌─┐  Scope-based querying
  ┌Dom.─A─┐                                  │ │
  │┌─────┐│  ┌──────┐           ┌─────────┐  │ │           ┌───────────┐
─►││ KG  ││◄─┤KGDBMS├───────────┤SPARQL EP├─►│ ├─Network &─┤  NetOps   │
  │└─────┘│  └──────┘           └─────────┘  │ ├─Usage─────┤Application│
  └UG.─2──┘                                  │ │           └───────────┘
  ┌Dom. B─┐                                  │ │           ┌───────────┐
  │┌─────┐│  ┌──────┐           ┌─────────┐  │ ├─Network &─┤  SecOps   │
─►││ KG  ││◄─┤KGDBMS├───────────┤SPARQL EP├─►│ ├─Security──┤Application│
  │└─────┘│  └──────┘           └─────────┘  │F│           └───────────┘
  └UG.─1┬─┘                                  │E│
        └────────────────────────────────────│D│─────────────┐
  ───On-premise / public-cloud─────────────  │E│             │
  ┌Dom.─C─┐                                  │R│             ▼  Usage
  │┌─────┐│  ┌──────┐ ┌───┐     ┌─────────┐  │A│           ┌────scope──┐
─►││ RDB ││◄─┤RDBMS ├─┤VKG├─────┤SPARQL EP├─►│T│           │*          │
  │└─────┘│  └──────┘ └───┘     └─────────┘  │E│   Network │   *  *    │
  └UG.─1&2┘                                  │D│   scope───│────────┐  │
  ┌Dom.─D─┐                                  │ │       │   │ *  *   │  │
  │┌─────┐│  ┌──────┐ ┌───┐     ┌─────────┐  │Q│       │  *└───────────┘
─►││NoSQL││◄─┤RDBMS ├─┤VKG├─────┤SPARQL EP├─►│U│       │  ┌───────────┐
  │└─────┘│  └──────┘ └───┘     └─────────┘  │E│       │* │ *  *    │ │
  └UG.─1──┘                                  │R│       └──│─────────┘ │
  ┌Dom.─E─┐                                  │I│        ▲ │     *     │
  │┌─────┐│  ┌──────┐ ┌───────┐ ┌─────────┐  │E│        │ │ *       * │
─►││ LPG ││◄─┤GDBMS ├─┤QL tlt.├─┤SPARQL EP├─►│S│        │ └──Security─┘
  │└─────┘│  └──────┘ └───────┘ └─────────┘  │ │        │    scope ▲
  └UG.┬2──┘                                  │ │        │          │
      └──────────────────────────────────────│ │────────┼──────────┘
                                             │ │        │
  ───Public-cloud──────────────────────────  │ │        │
  ┌Dom.─F─┐                                  │ │        │
  │┌─────┐│  ┌──────┐           ┌─────────┐  │ │        │
─►││ KG  ││◄─┤KGDBMS├───────────┤SPARQL EP├─►│ │        │
  │└─────┘│  └──────┘           └─────────┘  │ │        │
  └UG.┬1&2┘                                  └─┘        │
      └─────────────────────────────────────────────────┘
~~~~
{: #fig-multi-store title="Unified access to data distributed across various technological platforms"}


## Learning and sharing behavioral models

TODO NetOps perspective

TODO SecOps perspective

## Relation to the Digital Map {#sec-digital-map}

Similar to the concept of *meta-knowledge graph* (meta-KG) discussed in this document, the concept of *Digital Map* discussed in {{?I-D.havel-nmop-digital-map-concept}} emphasizes the need to structure heterogeneous data describing networks in order to simplify network management operations through unified access to this data.
The meta-knowledge graph extends the Digital Map concept by adding information about the lifecycle of infrastructures and services, as well as the context of their usage. These additional pieces of information are considered essential for learning shareable activity models of systems.

To clarify this positioning, the following lists ({{sec-digital-map-core}}, {{sec-digital-map-design}}, and {{sec-digital-map-archi}}) reflect the compliance of the meta-KG concept with the Digital Map Requirements defined in {{?I-D.havel-nmop-digital-map-concept}}.
A symbol to the right of each requirement name indicates the nature of compliance: **+** for compatibility, **/** for partial satisfaction, **-** for non-compliance with the requirement.
A comment is provided as necessary.

### Core Requirements {#sec-digital-map-core}

**+** REQ-BASIC-MODEL-SUPPORT:
: nothing to report (n.t.r.)

**+** REQ-LAYERED-MODEL:
: n.t.r.

**/** REQ-PROG-OPEN-MODEL:
: Partially satifying the requirement as the concept of meta-KG mainly relate to the knowledge representation topic rather than to the platform running the Digital Map service on top of the meta-knowledge graph.

**/** REQ-STD-API-BASED:
: Same remark as for REQ-PROG-OPEN-MODEL.

**+** REQ-COMMON-APP:
: n.t.r.

**+** REQ-SEMANTIC:
: n.t.r.

**+** REQ-LAYER-NAVIGATE:
: n.t.r.

**+** REQ-EXTENSIBLE:
: Knowledge graphs implicitly satisfy this requirement, notably with OWL {{OWL}} and SKOS {{SKOS}} constructs if considering RDF knowledge graphs for the meta-KG (e.g. `owl:sameAs` to relate a meta-KG entity to some other entity of another knowledge graph, `owl:equivalentClass` to link concepts and properties used to interpret the meta-KG to concepts and properties from other data models, `skos:inScheme` to group new items of a controled-vocabulary as part of a `skos:ConceptScheme`).

**+** REQ-PLUGG:
: Same remark as for REQ-EXTENSIBLE.

**+** REQ-GRAPH-TRAVERSAL:
: This capability is naturally enabled as the meta-KG concept involves using a graph data structure.

#### Design Requirements {#sec-digital-map-design}

**-** REQ-TOPO-ONLY:
: Requirement not satisfied as the meta-KG involves to have more than topological data to interpret and contextualize the network behavior.

**-** REQ-PROPERTIES:
: Same remark as for REQ-TOPO-ONLY.

**-** REQ-RELATIONSHIPS:
: Same remark as for REQ-TOPO-ONLY.

**+** REQ-CONDITIONAL:
: Native, notably considering the expressiveness of SPARQL {{SPARQL11-QL}} if using the Semantic Web protocol stack to run the meta-KG concept.

**+** REQ-TEMPO-HISTO:
: n.t.r.

### Architectural Requirements {#sec-digital-map-archi}

**+** REQ-DM-SCALES:
: This capability applies as we can use data aggregation at the graph level ({{fig-stream-mixed}} and {{fig-stream-mixed-kr}} compared to {{fig-stream-kg-only}} and {{fig-stream-kg-only-kr}}), aggregation without loss of information ({{fig-stream-mixed}} and {{fig-stream-mixed-kr}}), and load balancing (horizontal scaling) by partitioning the meta-KG ({{fig-multi-store}}). Further, ease of integration is enabled thanks to existing standard graph data access protocols (e.g. SPARQL Federated Queries {{SPARQL11-FQ}}, as illustrated in {{fig-multi-store}}).

**/** REQ-DM-DISCOVERY:
: Same remark as for REQ-PROG-OPEN-MODEL.

## Experiments

TODO Experiments

## Implementation status

This section provides pointers to existing open source implementations of this draft or in close relation to it.

### NORIA

The NORIA project aims at enabling advanced network anomaly detection using knowledge graphs.
Among the components resulting from this project, the following ones serve the use case described in this document:

* NORIA-O {{NORIA-O-2024}}, is a data model for IT networks, events and operations information.
The ontology is developed using web technologies (e.g. RDF, OWL, SKOS) and is intended as a structure for realizing an ITSM knowledge graph for Anomaly Detection (AD) and Risk Management applications.
Its use for anomaly detection is discussed in:
  - {{SLKG-2023}} with a model-based design approach (i.e. query the graph to retrieve anomalies and their context) and a statistical learning approach (i.e. relate entities based on context
similarities, then use this relatedness to alert and guide the repair).
  - {{GPL-2024}} with a process mining approach to align a sequence of entities to activity models, then use this relatedness to guide the repair actions.
  - {{NORIA-UI-2024}} a Web-based knowledge graph exploration design for incident management that combines the above {{SLKG-2023}} and {{GPL-2024}} techniques for broader coverage of anomaly cases and knowledge capitalization.

* A knowledge graph-based platform design {{NORIA-DI-2023}} using Semantic Web technologies and open source data integration tools to build an ITSM knowledge graph:
  - SMASSIF-RML, a Semantic Web stream processing solution with declarative data mapping capability.
  - ssb-consum-up, a Kafka to SPARQL gateway enabling end-to-end Semantic Web data flow architecture with a Semantic Service Bus (SSB) approach.
  - grlc, a fork of CLARIAH/grlc with SPARQL UPDATE and GitLab interface features to facilitate the call and versioning of stored user queries in SPARQL syntax (e.g. for anomaly detection following the model-based design approach).

* SemNIDS {{SemNIDS-2023}}, a test bench involving network trafic generation, open source Network Intrusion Detection Systems (NIDS), knowledge graphs, process mining and conformance checking components.

# Security Considerations

As this document covers the *meta-knowledge graph* concepts, and use cases, there is no specific security considerations.

However, as the concept of a meta-knowledge graph involves the construction of a multi-faceted graph (i.e. including network topologies, operational data, and service and client data), it poses the risk of simplifying access to network operational data and functions that fall outside the knowledge graph users' responsibility or that could facilitate the intervention of malicious individuals.
To support the discussion on mitigating this risk, we suggest referring to {{fig-multi-store}}, which illustrates the concept of partial access to the meta-knowledge graph based on rights associated with each user group (UG) at the data domain level.
We also recommend referring to {{AMO-2012}} for an example of implemention of access rights in a content management system that relies on Semantic Web models and technologies.
This implementation uses the AMO ontology, which includes a set of classes and properties for annotating resources that require access control, as well as a base of inference rules that model the access management strategy to carry out.

# IANA Considerations

This document has no IANA actions.

--- back

# Acknowledgments
{:numbered="false"}

We would like to thank Benoit Claise for spontaneously seeking to include the work of the NORIA research project in the vision of the NMOP working group through direct contact.

We would also like to thank Fano Rampary for his initial analysis of the possibilities of defining a model conversion algebra for going from Yang data models to OWL ontologies.
