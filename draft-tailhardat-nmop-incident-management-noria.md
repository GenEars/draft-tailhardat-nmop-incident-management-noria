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

  RML:
    title: "RDF Mappling Language (RML)"
    author:
      - name: Anastasia Dimou
      - name: Miel Vander Sande
      - name: Ben De Meester
      - name: Pieter Heyvaert
      - name: Thomas Delva
    target: https://rml.io/specs/rml/
    date: June 2024

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

  ONTO-MATCH-2022:
    author:
      - name: Portisch, Jan
      - name: Costa, Guilherme
      - name: Stefani, Karolin
      - name: Kreplin, Katharina
      - name: Hladik, Michael
      - name: Paulheim, Heiko
    title: "Ontology Matching Through Absolute Orientation of Embedding Spaces"
    date: 2022
    target: https://doi.org/10.1007/978-3-031-11609-4_29

--- abstract

Operational efficiency in incident management on telecom and computer networks requires correlating and interpreting large volumes of heterogeneous technical information.
Knowledge graphs can provide a unified view of complex systems through shared vocabularies.
YANG data models enable describing network configurations and automating their deployment.
However, both approaches face challenges in vocabulary alignment and adoption, hindering knowledge capitalization and sharing on network designs and best practices.
To address this, the concept of a IT Service Management (ITSM) Knowledge Graph (KG) is introduced to leverage existing network infrastructure descriptions in YANG format and enable abstract reasoning on network behaviors.
The key principle to achieve the construction of such ITSM-KG is to transform YANG representations of network infrastructures into an equivalent knowledge graph representation, and then embed it into a more extensive data model for Anomaly Detection (AD) and Risk Management applications.
In addition to use case analysis and design pattern analysis, an experiment is proposed to assess the potential of the ITSM-KG in improving network quality and designs.


--- middle

# Introduction {#sec-intro}

Incident management on telecom and computer networks, whether it is related to infrastructure or cybersecurity issues, requires the ability to simultaneously and quickly correlate and interpret a large number of heterogeneous technical information sources.
Knowledge graphs, by structuring heterogeneous data through shared vocabularies, enable providing a unified view of complex technical systems, their ecosystem, and the activities and operations related to them (see {{?I-D.marcas-nmop-knowledge-graph-yang}} and {{NORIA-O-2024}}).
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
Firstly, the concept of an ITSM-KG is introduced in {{sec-itsm-base}} towards leveraging existing network infrastructure descriptions in YANG format and enabling abstract reasoning on network behaviors.
The relation of the ITSM-KG proposal to the Digital Map {{?I-D.havel-nmop-digital-map-concept}} is notably discussed in this section.
Secondly, strategies for the ITSM-KG construction are discussed in {{sec-kgc}}.
This include YANG models transformation in {{sec-yang-to-kg}}, implementing alignments of models with the ITSM-KG in {{sec-gluing-techniques}}, and knowledge graph construction pipeline designs in {{sec-etl-kgc}}.
The {{sec-etl-kgc}} notably focuses on addressing the handling of event data streams and providing a unified view for different stakeholders, also known as the data federation architecture.
Finally, an experiment is proposed in {{sec-experiments}} to assess the potential of the ITSM-KG in improving network quality and designs.
The implementation status related to this document is also reported in this section.

# Conventions and Definitions

{::boilerplate bcp14-tagged}


# An ITSM-KG for learning and sharing network behavioral models {#sec-itsm-base}

## Principles

As evoked in {{sec-intro}}, a detailed characterization of network behavior requires combining several facets of data related both to the configuration of the networks and to their lifecycle, as well as the ecosystem in which they are operated.
In this document, we will consider the following fundamental definitions as a means to achieve the combination of all these facets of data in a convenient way, regardless of their origin, for operational efficiency in incident management and change management with the aid of AI tools:

ITSM-KG:
: A knowledge graph in RDFS/OWL syntax tha enables change management activities, anomaly detection, and risk analysis at the organizational level by combining heterogeneous data sources from the configuration data of the network's structural elements, events occurring on this network, and any other data useful to the business for the effective management of the services provided by this network.

ONTO-ITSM:
: For a given ITSM-KG, the RDFS/OWL ontology that structures the ITSM-KG.

ONTO-YANG-MODEL:
: For a given YANG model, its equivalent RDFS/OWL representation.

ONTO-META:
: An ontology that contributes to structuring some ITSM-KG, regardless of the specifics of a given application domain or ITSM-KG instance, in the sense that it provides an abstract IT Service Management model (i.e. it holds generic concept and property definitions for realizing IT Service Management activities).

ONTO-LINKER:
: For a given (set of) ONTO-YANG-MODEL and a given ONTO-META, the implementation of the equivalence relationships between the key concepts and key properties of the (set of) ONTO-YANG-MODEL and ONTO-META.

Based on these definitions, which will be discussed in more detail later in this document, {{fig-incident-context}} can be seen as an illustration of ITSM-KG from which a subgraph has been extracted, allowing for incident situation to be analyzed through querying.
For example, close to ideas from {{?I-D.netana-nmop-network-anomaly-lifecycle}}, querying the evolution of network entities states from the ITSM-KG during some incident remediation stage could bring to identify the causal graph underlying incident resolution.
As the querying would go through the ONTO-ITSM, the causal graph would de-facto be an abstraction of the situation, thereby enabling knowledge capitalization and sharing for similar incidents that could occur later.

## Relation to the Digital Map {#sec-digital-map}

Similar to the concept of ITSM-KG discussed in this document, the concept of Digital Map discussed in {{?I-D.havel-nmop-digital-map-concept}} emphasizes the need to structure heterogeneous data describing networks in order to simplify network management operations through unified access to this data.
The ITSM-KG can be seen as a meta-knowledge graph that extends the Digital Map concept by adding information about the lifecycle of infrastructures and services, as well as the context of their usage. These additional pieces of information are considered essential for learning shareable activity models of systems.

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

### Design Requirements {#sec-digital-map-design}

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



# Strategies for the ITSM-KG construction {#sec-kgc}

In this section, we firstly define in {{sec-yang-to-kg}} two YANG-based data transformation scenario, namely the YANG-KG-SEMANTIC-EQUIVALENCE and YANG-KG-SEMANTIC-GENERALIZATION scenarios.
The YANG-KG-SEMANTIC-GENERALIZATION scenario is then used as a basis in {{sec-gluing-techniques}} to illustrate strategies to reuse YANG models transformed in RDFS/OWL syntax in a higher-level ontology that would structure the ITSM-KG.
Finally, two Extract-Transform-Load (ETL) pipeline approaches and a data federation architecture are presented in {{sec-etl-kgc}} to meet the needs of constructing and exploiting the ITSM-KG.


## From YANG-based configurations to meta-knowledge graph {#sec-yang-to-kg}

In the following, we consider the use of Semantic Web technologies as the foundation for representing data in the form of a knowledge graph.
We also assume the ability to transform a description of configurations and network infrastructures expressed accordingly to a given (set of) YANG model(s) into a knowledge graph representation.

For the realization of this data transformation, we identify the following scenarios:

YANG-KG-SEMANTIC-EQUIVALENCE:
: The ontology structuring the target knowledge graph is an exact equivalence of the many YANG models organizing the configuration data.

YANG-KG-SEMANTIC-GENERALIZATION:
: The ontology structuring the target KG is a generalization of the YANG models organizing the configuration data.

We note that the YANG-KG-SEMANTIC-EQUIVALENCE case requires a significant knowledge engineering effort to align all YANG models into a coherent ontology with a sufficient level of abstraction to enable the discovery and analysis of emergent behavioral models of networks independently of local configuration specifics.
However, this case has the advantage of being relatively easy to implement based on the available configuration data of an operator, for example, by implementing {{RML}} rules for constructing a knowledge graph from this data.

For the YANG-KG-SEMANTIC-GENERALIZATION case, we observe that the transformation effort involves:

1. Being able to transform YANG models into their RDFS/OWL equivalent to provide a consistent interpretation of configuration data in a knowledge graph that aligns with each data source.
2. Being able to provide a generalized interpretation of these transformed YANG models by identifying alignments between key concepts in these models and those in a more expressive ontology.

As an example, the YANG-KG-SEMANTIC-GENERALIZATION case could involve wanting to integrate Service and Network topology data, matching the Network Topologies {{!RFC8345}} and Service Assurance {{!RFC9418}} YANG data models, into a knowledge graph structured by the NORIA-O ontology {{NORIA-O-2024}}.

Although identifying alignments in the YANG-KG-SEMANTIC-GENERALIZATION case may appear non-trivial for "constructor" YANG models, it is worth noting that the design of YANG models generally relies on principles of concept hierarchies and reuse of common concepts between models to promote model interoperability, as is the case with the Abstract Network Model of {{!RFC8345}}.
Therefore, the task of identifying alignments can theoretically benefit from these design principles.

In continuity of the above RFC8345 / NORIA-O example, providing an alignment may mean asserting a semantic equivalence between the RDFS/OWL representation of the "node" concept from {{!RFC8345}} with the "noria:Resource" concept from {{NORIA-O-2024}}.
Examples of approaches for linking ontologies are provided in {{sec-gluing-techniques}}.


## Implementing alignments of model-specificities to a multi-faceted knowledge graph {#sec-gluing-techniques}

Building on the previously defined YANG-KG-SEMANTIC-GENERALIZATION scenario, this section presents two approaches to construct the structuring ontology of the ITSM-KG by combining YANG models translated into RDFS/OWL and a meta-ontology enabling the analysis of the operational context of the network lifecycle.
As techniques for identifying alignments between data models is beyond the scope of this document, we refer interested readers to specialized literature in this field, such as {{ONTO-MATCH-2022}}.

To present the approaches, we assume the ability to convert a given YANG model into its ONTO-YANG-MODEL (i.e. its equivalent RDFS/OWL representation).
The code snippet in {{snippet-ietf-network-node}} is a fictional example of translating the "node" concept from {{!RFC8345}} into its RDFS/OWL equivalent.

~~~
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

<urn:ietf:params:xml:ns:yang:ietf-network#node>
  rdf:type owl:Class ;
  rdfs:comment  "The inventory of nodes of this network." ;
.
~~~
{: #snippet-ietf-network-node title="Snippet of the ONTO-YANG-MODEL describing the 'node' concept from RFC8345 into its RDFS/OWL equivalent, in Turtle syntax."}

The following sub-sections build on the ONTO-YANG-MODEL example from {{snippet-ietf-network-node}}.

### The network of ontologies approach

The network of ontologies approach is a common practice in the field of knowledge engineering and Semantic Web technologies.
The principle involves assembling vocabularies from different domains to form a coherent set, for example to infer - through graph traversal or reasoning - relationships between entities in the graph, starting from a concept defined in one of the vocabularies and leading to an instance of a concept from another vocabulary.

In our example, the code snippet of {{snippet-onto-itsm}} implements the ONTO-ITSM by importing concepts from the ONTO-YANG-MODEL ({{snippet-ietf-network-node}}) and concepts from the ONTO-META ({{snippet-noria-o-as-it-is}}).
An additional import in {{snippet-onto-linker}} relates to the ONTO-LINKER.

~~~
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .

<https://example.com/ontologies/itsm/>
  rdf:type owl:Ontology ;
  owl:imports
    # ===> Import of one of the ONTO-YANG-MODEL <===
    <https://example.com/ontologies/ietf-network-topology> ,
    # ===> Import of the ONTO-META <===
    <https://w3id.org/noria/ontology/> ,
    # ===> Import of the ONTO-LINKER definitions <===
    <https://example.com/ontologies/ietf-noria-linker> ;
.
~~~
{: #snippet-onto-itsm title="The implementation of the ONTO-ITSM to structure the relation of ONTO-YANG-MODEL(s) with ONTO-META, in Turtle syntax."}

~~~
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

@prefix seas: <https://w3id.org/seas/>.  # Smart Energy Aware Systems
@prefix bot:  <https://w3id.org/bot#> .  # Building Topology Ontology
@prefix observable:  # Unified Cybersecurity Ontology (UCO)
  <https://unifiedcyberontology.org/ontology/uco/observable#> .
@prefix log: <https://w3id.org/sepses/ns/log#> .  # a.k.a. SLOGERT

@prefix noria: <https://w3id.org/noria/ontology/> .

noria:Resource
    rdf:type owl:Class ;
    rdfs:label "Resource" ;
    rdfs:comment """General resource record of the Communication Device
      kind from the logistics park. It is a managed entity that can be
      either Physical or Virtual."""@en ;
    rdfs:subClassOf noria:StructuralElement ;
    rdfs:subClassOf
        seas:System,
        seas:CommunicationDevice,
        bot:Element ,
        observable:Device ,
        log:Host ;
    rdfs:isDefinedBy noria: ;
.
~~~
{: #snippet-noria-o-as-it-is title="Snippet of the ONTO-META describing the 'noria:Resource' concept from NORIA-O v0.3, in Turtle syntax."}


~~~
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix noria: <https://w3id.org/noria/ontology/> .

noria:Resource
  owl:equivalentClass <urn:ietf:params:xml:ns:yang:ietf-network#node> ;
.
~~~
{: #snippet-onto-linker title="Snippet of the ONTO-LINKER to relate ONTO-YANG-MODEL definition(s) with ONTO-META definition(s), in Turtle syntax."}

As a result, querying any ITSM-KG structured by the ONTO-ITSM, as shown in {{snippet-sparql-equivalent}}, enables retrieving entities of the ITSM-KG using ONTO-META concepts, even if entities are described with ONTO-YANG-MODEL concepts.

~~~
PREFIX owl: <http://www.w3.org/2002/07/owl#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>
PREFIX noria: <http://data-noria.securite.fr.intraorange/ontology/>

SELECT ?res

WHERE {
  # Pattern for the base class from ONTO-META
  # or any equivalent class from ONTO-YANG-MODEL
  ?resClass (owl:equivalentClass|^owl:equivalentClass)* noria:Resource .

  # Pattern to retrieve instances from the ITSM-KG
  ?res rdf:type ?resClass .
}
~~~
{: #snippet-sparql-equivalent title="Snippet to retrieve entities of the ITSM-KG assuming the relatedness of ONTO-META concepts with ONTO-YANG-MODEL concepts, in SPARQL syntax."}

### Explicit linking in the ONTO-META

In this approach, we assume that we have the means to evolve ONTO-META, which allows for the implementation of equivalence relationships between the concepts of ONTO-META and ONTO-YANG-MODEL directly within ONTO-META, as shown in {{snippet-noria-o-extended}}.

In this sense, ONTO-ITSM is part of ONTO-META, and ONTO-LINKER is within ONTO-META.
The query in {{snippet-sparql-equivalent}} applies here as well and will yield the same results.

~~~
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

@prefix seas: <https://w3id.org/seas/>.  # Smart Energy Aware Systems
@prefix bot:  <https://w3id.org/bot#> .  # Building Topology Ontology
@prefix observable:  # Unified Cybersecurity Ontology (UCO)
  <https://unifiedcyberontology.org/ontology/uco/observable#> .
@prefix log: <https://w3id.org/sepses/ns/log#> .  # a.k.a. SLOGERT

@prefix noria: <https://w3id.org/noria/ontology/> .

<https://w3id.org/noria/ontology/>
  a owl:Ontology ;
  # ===> Import of one of the ONTO-YANG-MODEL <===
  <https://example.com/ontologies/ietf-network-topology> .

noria:Resource
    rdf:type owl:Class ;
    rdfs:label "Resource" ;
    rdfs:comment """General resource record of the Communication Device
      kind from the logistics park. It is a managed entity that can be
      either Physical or Virtual."""@en ;
    rdfs:subClassOf noria:StructuralElement ;
    rdfs:subClassOf
        seas:System,
        seas:CommunicationDevice,
        bot:Element ,
        observable:Device ,
        log:Host ;
    rdfs:isDefinedBy noria: ;
    # ===> Explicit linking to ONTO-YANG-MODEL <===
    owl:equivalentClass <urn:ietf:params:xml:ns:yang:ietf-network#node>
.
~~~
{: #snippet-noria-o-extended title="Snippet of the ONTO-META describing the 'noria:Resource' concept from NORIA-O v0.3 with added linking to ONTO-YANG-MODEL, in Turtle syntax."}


## Extract-Transform-Load pipelines for the ITSM-KG {#sec-etl-kgc}

Based on {{?I-D.marcas-nmop-knowledge-graph-yang}} and {{NORIA-DI-2023}}, which present the technical means to implement a pipeline for constructing the ITSM-KG, this section focuses on two complementary viewpoints:
{{sec-etl-kgc-streams}} the management of streaming data such as alarms and logs,
and {{sec-etl-kgc-fq}} the deployment of a federated data architecture when various technical foundations or business units are involved in providing the ITSM-KG.

From the perspective of the Digital Map Requirements ({{sec-digital-map}}), the {{fig-stream-mixed}}, {{fig-stream-mixed-kr}} and {{fig-multi-store}} particularly address the REQ-DM-SCALES requirement.

### Handling event streams {#sec-etl-kgc-streams}

The following figures illustrate different scenarios for constructing a ITSM-KG through an Extract-Transform-Load (ETL) data integration pipeline.

{{fig-stream-kg-only}} illustrates a common design pattern providing the capability to record event streams into a knowledge graph, such as an ITMS-KG if considering that event data are mapped to ONTO-META concepts and network entities to ONTO-YANG-MODEL concepts.
The {{fig-stream-kg-only-kr}} provides an example of the resulting representation in the form of a knowledge graph.

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
{: #fig-stream-kg-only title="KG-only data integration architecture for event data streams."}

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

As event streams can be high-paced, it could be beneficial to leverage input/output (I/O) performance optimizations specific to each type of database management system (DBMS), such as Time-Series DataBases (TSDBs) for streaming data and graph databases for knowledge graphs.
{{fig-stream-mixed}} illustrates the capability to handle both a knowledge graph and a time-series representation of the network's lifecycle while maintaining a link between the two representations ({{fig-stream-mixed-kr}}).
Each serve different purposes, such as context analysis with the knowledge graph representation and trend analysis with the TSDB.
Thanks to the linking between the two storage systems, users browsing aggregated data from the knowledge graph can access the raw data within the relevant time span for further analysis, and vice versa.

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
{: #fig-stream-mixed title="Mixed KG/non-KG data integration architecture for event data streams."}


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
{: #fig-stream-mixed-kr title="Resulting knowledge representation for the mixed KG/non-KG data integration architecture for event data streams."}


### Federated data architecture {#sec-etl-kgc-fq}

The {{fig-multi-store}} illustrates the principles for providing unified access to data distributed across various technological platforms and stakeholders thanks to Federated Queries {{SPARQL11-FQ}} and the use of a shared ONTO-ITSM across data management platforms.

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
{: #fig-multi-store title="Unified access to data distributed across various technological platforms."}



# Experiments {#sec-experiments}

## Experimental plan

In terms of experimentation, we consider the YANG-KG-SEMANTIC-GENERALIZATION case defined in {{sec-kgc}} as the reference approach and recommend implementing a data processing pipeline that performs the following use cases:

Y-MODEL-FROM-DATA:
: Based on a dataset of configuration data expressed in YANG models, the goal is to enable extracting the list of models involved for their conversion to their RDFS/OWL equivalent.

Y-MODEL-DEPENDENCIES:
: Based on a given YANG model, the goal is to enable identifying and retrieving all the YANG models that the model refers to, in order to build a complete corpus of models for their conversion to their RDFS/OWL equivalent as a coherent set.

Y-MODEL-TO-RDFS-OWL:
: Based on a YANG model and the associated model corpus (i.e. Y-MODEL-DEPENDENCIES), the goal is to enable producing a semantically equivalent RDFS/OWL representation (i.e. ONTO-YANG-MODEL).
: Ideally, a YANG to RDFS/OWL/YANG projection algebra would be used to provide a formal proof of semantic equivalence; testing mechanisms should be implemented as a fallback to provide a proof of equivalence.

Y-INSTANCE-TO-KG:
: Based on a dataset of configuration data expressed in YANG models and the related (set of) ONTO-YANG-MODEL, the goal is to enable constructing a knowledge graph from the configuration data, with the knowledge graph structured by the (set of) ONTO-YANG-MODEL.

Y-MODEL-META-KG-ALIGNMENT:
: Based on a corpus of YANG models transformed into RDFS/OWL (i.e. Y-MODEL-TO-RDFS-OWL) and a reference ontology structuring the ITSM-KG, the goal is to enable querying of the configuration entities present in the graph (i.e. data derived from the Y-INSTANCE-TO-KG case) through the concepts of the reference ontology.
: In addition to identifying the class and property correspondences between the resulting Y-MODEL-TO-RDFS-OWL models and the reference ontology, this capability requires implementing a necessary and sufficient number of class equivalence relations and property equivalence relations.

META-KG-BEHAVIORAL-MODEL:
: Based on the ITSM-KG, which results from the composition of the Y-INSTANCE-TO-KG case with Y-MODEL-META-KG-ALIGNMENT and additional operational data structured by ONTO-META, the goal is to learn behavioral models (e.g. incident signatures) in a formalism that can be interpreted through the lenses of ONTO-ITSM and shared with other stakeholders with minimal discrepancies in the underlying configuration data.

## Implementation status

This section provides pointers to existing open source implementations of this document or in close relation to it.

### NORIA

The NORIA project aims at enabling advanced network anomaly detection using knowledge graphs.
Among the components resulting from this project, the following ones serve the use case described in this document:

* NORIA-O {{NORIA-O-2024}}, is a data model for IT networks, events and operations information.
The ontology is developed using web technologies (e.g. RDF, OWL, SKOS) and is intended as a structure for realizing an ITSM knowledge graph for Anomaly Detection (AD) and Risk Management applications.
The NORIA-O implementation is available as open source at [https://w3id.org/noria/](https://w3id.org/noria/).
Its use for anomaly detection is discussed in:
  - {{SLKG-2023}} with a model-based design approach (i.e. query the graph to retrieve anomalies and their context) and a statistical learning approach (i.e. relate entities based on context
similarities, then use this relatedness to alert and guide the repair).
  - {{GPL-2024}} with a process mining approach to align a sequence of entities to activity models, then use this relatedness to guide the repair actions.
  - {{NORIA-UI-2024}} a Web-based knowledge graph exploration design for incident management that combines the above {{SLKG-2023}} and {{GPL-2024}} techniques for broader coverage of anomaly cases and knowledge capitalization.

* A knowledge graph-based platform design {{NORIA-DI-2023}} using Semantic Web technologies and open source data integration tools to build an ITSM knowledge graph:
  - SMASSIF-RML, a Semantic Web stream processing solution with declarative data mapping capability. Available as open source at [https://github.com/Orange-OpenSource/smassif-rml](https://github.com/Orange-OpenSource/smassif-rml).
  - ssb-consum-up, a Kafka to SPARQL gateway enabling end-to-end Semantic Web data flow architecture with a Semantic Service Bus (SSB) approach. Available as open source at [https://github.com/Orange-OpenSource/ssb-consum-up](https://github.com/Orange-OpenSource/ssb-consum-up).
  - grlc, a fork of CLARIAH/grlc with SPARQL UPDATE and GitLab interface features to facilitate the call and versioning of stored user queries in SPARQL syntax (e.g. for anomaly detection following the model-based design approach). Available as open source at [https://github.com/Orange-OpenSource/grlc](https://github.com/Orange-OpenSource/grlc).

* SemNIDS {{SemNIDS-2023}}, a test bench involving network trafic generation, open source Network Intrusion Detection Systems (NIDS), knowledge graphs, process mining and conformance checking components.

Note that the NORIA project does not currently address the Y-MODEL-FROM-DATA, Y-MODEL-DEPENDENCIES, and Y-MODEL-TO-RDFS-OWL use cases.

# Security Considerations

As this document covers the *ITSM-KG* concepts, and use cases, there is no specific security considerations.

However, as the concept of a meta-knowledge graph involves the construction of a multi-faceted graph (i.e. including network topologies, operational data, and service and client data), it poses the risk of simplifying access to network operational data and functions that fall outside the knowledge graph users' responsibility or that could facilitate the intervention of malicious individuals.
To support the discussion on mitigating this risk, we suggest referring to {{fig-multi-store}}, which illustrates the concept of partial access to the meta-knowledge graph based on rights associated with each user group (UG) at the data domain level.
We also recommend referring to {{AMO-2012}} for an example of implementation of access rights in a content management system that relies on Semantic Web models and technologies.
This implementation uses the AMO ontology, which includes a set of classes and properties for annotating resources that require access control, as well as a base of inference rules that model the access management strategy to carry out.

# IANA Considerations

This document has no IANA actions.

--- back

# Acknowledgments
{:numbered="false"}

We would like to thank Benoit Claise for spontaneously seeking to include the work of the NORIA research project in the vision of the NMOP working group through direct contact.

We would also like to thank Fano Ramparany for his initial analysis of the possibilities of defining a model conversion algebra for going from YANG data models to OWL ontologies.
