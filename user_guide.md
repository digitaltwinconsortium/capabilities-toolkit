---
title: Digital Twin Capabilities Periodic Table User Guide
subtitle: Version 1.2
date: \today
author: The Digital Twin Consortium CPT Working Group  
# abstract: A Digital Twin Consortium User Guide

---

\newpage

# What is new in version 1.2

Since the release of Version 1.1, the Digital Twin Consortium's Capabilities Periodic Table (CPT) continues to evolve in response to user needs and technological advances. Version 1.2 introduces several key innovations:

* **Computable CPT Format** – The core innovation in Version 1.2 is the conversion of the Capabilities Periodic Table into a YAML file format, creating what we call a "computable version" of the CPT. This transformation dramatically enhances interoperability with generative AI systems.

* **Multiple Format Generation** – From the base YAML file, we've developed generators that can produce alternative formats including JSON, XLSX, and PowerPoint files, significantly expanding accessibility and integration options.

* **Minor Content Updates** – We've resolved an ID overlap issue and completed previously missing content, ensuring the CPT is comprehensive and consistent.

The computable nature of this version enables AI-assisted capability assessments, automated requirements specifications, and dynamic visualization of capability mappings. Organizations can now programmatically interact with the CPT, embedding it into their digital twin implementation workflows and toolchains.

## Computable CPT Format

With Version 1.2, the Digital Twin Consortium introduces the Computable CPT in YAML format. This structure enables programmatic access to the Capabilities Periodic Table, enabling new ways to leverage the framework.

### Available CPT Formats

The CPT is now available in the following machine-readable formats:

1. **YAML** - The base format that serves as the source of truth for the CPT data structure
2. **JSON** - For integration with web applications and services
3. **XLSX** - Excel format for traditional spreadsheet analysis and reporting
4. **PowerPoint** - For presentation and communication purposes

### Benefits of the Computable Format

The computable CPT format offers several significant advantages:

- **AI Integration** - Allows generative AI systems to directly understand and work with the CPT structure
- **Automation** - Enables automated capability assessment and requirements generation
- **Visualization** - Supports dynamic visualization tools that can adapt to specific use cases
- **Extensibility** - Makes it easier to expand and enhance the CPT in future versions
- **Consistency** - Ensures all derived formats maintain the same underlying structure and content

### Accessing the Computable CPT

The computable version of the CPT can be accessed through the Digital Twin Consortium's GitHub repository, where users can download the latest version in their preferred format.

The member's GitHub repo (restricted access) is here: https://github.com/digitaltwinconsortium/dtc-capabilities-toolkit . For access, members can send their GitHub ID (not their email address) to the DTC co-ordinators.  

The public version is here: https://github.com/digitaltwinconsortium/capabilities-toolkit . It contains a synced subset of files from the member repo.

\newpage
# Part I: Core

## Introduction

The Digital Twin Capabilities Periodic Table (CPT) is an architecture and technology agnostic requirements definition framework. It is aimed at organizations who want to design, develop, deploy and operate digital twins based on use case capability requirements versus the features of technology solutions.

The Digital Twin Capabilities Periodic Table framework facilitates collaboration in multidisciplinary or fusion teams that need to create digital twins requirements specifications in large scale complex environments. The framework keeps the focus on the capability requirements of individual use cases, which can then be aggregated to determine the overall capability requirements, digital twin platforms and other technology solutions that are required to address the specific business needs.

It follows a periodic table approach with capabilities grouped or "clustered" around common characteristics. It is easy to interpret at both the boardroom when explaining the business case to get funding for a digital twin project, and the shopfloor when gathering requirements for a digital twin application. It provides visual guidance for collaboration, brainstorming and making capability requirements explicit.

End users that are investigating digital twin technology to address business transformation and other digitalization needs often ask these three questions:

- What is a digital twin?
- Why should I care?
- How do I get started?

Digital Twin Consortium's [definition of a digital twin](https://www.digitaltwinconsortium.org/initiatives/the-definition-of-a-digital-twin.htm) provides a comprehensive answer to the first question:

> A digital twin is an integrated data-driven virtual representation of real-world entities and processes, with synchronized interaction at a specified frequency and fidelity.
>
> - Digital Twins are motivated by outcomes, driven by use cases, powered by integration, built on data, enhanced by physics, guided by domain knowledge, and implemented in dependable and trustworthy IT/OT/ET systems.
> - Digital Twin Systems transform business by accelerating and automating holistic understanding, continuous improvement, decision-making, and interventions through effective action.
> - Digital Twin Systems are built on integrated and synchronized IT/OT/ET systems, use real-time and historical data to represent the past and present, and simulate predicted futures.
> - Digital Twin Prototypes use data to model and simulate predicted futures before being integrated into IT/OT/ET Systems and before synchronization with the real-world entity or process.

The second question is addressed by the use case reference library that is being developed by the DTC. It describes the problem, the impact and the way that a digital twin addresses the specific business challenge. It highlights the benefits and impact of digital twins in various use cases and industries.

The purpose of this guide is to assist with the third question on how to get started with digital twins. It provides a framework for organizations that are just starting on the journey, and it provides a consistent approach as organizations scale out and increase their digital twin maturity.

### Capability vs Technology

Capability is the ability to perform or achieve certain actions/outcomes. The ability to drill a hole is a very simple example of a capability. There are multiple use cases that require holes and each of them will have unique requirements in terms of the size, the depth or the substance that is drilled. This may be one of many capabilities required to successfully complete a project where the hole is part of the solution.

Digital twins provide unique capabilities as described in the DTC definition, but a digital twin, in itself, is composed from a number of technical capabilities to provide an overall solution.

The Digital Twin Capabilities Periodic Table is focused on these technology-based capabilities, but it is agnostic to specific technology or product solutions. For example, machine learning capability can be provided by several technology providers, each with different products. During the assessment of vendor capabilities, it is important to clarify that the technology solution can fulfill the technological capability requirement of the business use case.

The approach used in the Digital Twins Capabilities Periodic Table to describe these capabilities follows a simple structure:

- what it is (capability name),
- what it does (capability description) and
- what it means or purpose (what does it enable).

The Digital Twins Capabilities Periodic Table is not a reference architecture, but it supports multiple architectural approaches. It highlights the capability building blocks for composable digital twins. The Digital Twin Consortium reference architecture provides recommended structures and integrations of Internet of Things (IoT), Information Technology (IT), Operational Technology) OT, and Engineering Technology (ET) products and services to form a digital twin solution. In addition to the DTC reference architecture for digital twins, the Capabilities Periodic Table supports other reference architectures that end-users may already have developed using their own corporate standards.

### Enable Composable Digital Twins

Composable Digital Twins (CDT) is an application development approach for digital twins that is based on the composable enterprise architectural pattern. Composable applications, such as CDTs, focus on faster time to value, service-based orchestration and reusing packaged business capabilities to develop and adapt applications as business requirements evolve.

Packaged Business Capabilities (PBC) are modular combinations of technical capabilities that are presented as bundled services. These PBCs are orchestrated together through an application composition platform to deliver unique digital twin applications for specific use cases.

The Digital Twin Capabilities Periodic Table provides a consistent framework to identify the capabilities that can be grouped together to create these PBCs. Figure \ref{fig:composable} shows a composable Digital twin reference model that outlines the different data types and data sources that are leveraged by PBCs to create reusable and agile digital twin compositions.

![Composable Digital Twin Reference Model for discrete and system of system digital twins.](./img/composable_digital_twin_reference_model.jpg){#fig:composable}

A key characteristic of a composable digital twin is that it is typically a combination of capabilities from multiple technology vendors. Composite or system-of-systems digital twins are based on an ecosystem of capabilities rather than a single vendor.

### Ecosystem vs Single Vendor

The smorgasbord of capabilities that are all captured in the Digital Twin Capabilities Periodic table are beyond the scope of any single vendor. It requires an ecosystem of interoperable technical capabilities to address large scale, complex digital twin use cases. The Digital Twin Capabilities Periodic Table provides a common framework for multiple vendors to identify and present key capabilities that they provide for a digital twins solution.

This common framework is a major benefit of the Digital Twin Capabilities Periodic Table for an end user organization that is clarifying requirements for a digital twin. It removes the focus from vendor specific technologies and places it on the key capabilities that are required to successfully deliver a digital twin solution. It is useful in analyzing a vendor solution to see if it is complete or not in aligning with the use case needs. It provides the opportunity to light up the capabilities in the requirements and then overlay the capabilities in the solution to see how well they align.

### Fits Across The Digital Twins Lifecycle

The Digital Twin Capabilities Periodic table is applicable across the full life cycle of the digital twin. The capabilities may differ during the different phases, but the approach to identify the key capabilities for each phase remains the same throughout the overall life cycle.

Some capabilities may transfer between lifecycle phases, while others may become obsolete and new capabilities are introduced for new use cases. Capabilities during the design and construction phase may not all transfer to the operations and maintenance phase of an entity like a production plant. This help facilitates the development of the digital thread as it transitions through the different lifecycle phases. The digital twin supports the digital thread through these capabilities. The Digital Twin Capabilities Periodic table can also be used to identify capabilities for the digital thread.

![Capabilities during the digital twin and digital thread lifecycle.](./img/digital_twin_lifecycle.jpg){#fig:lifecycle}

The Digital Twin Capabilities Periodic Table provides a consistent approach for increasing capability maturity at both project and organizational levels throughout full product life cycles.

## The Digital Twin Capability Periodic Table (CPT)

### The Digital Twin CPT Categories

The Digital Twin CPT is organized into six logical groupings, matching capabilities that have similar characteristics and application. Figure \ref{fig:domains} provides context to the different categories that reflect both the digital and physical twins.

![Digital twins CPT categories in physical and virtual domains.](./img/digital_twin_capabilities_physical_virtual_domains.jpg){#fig:domains} 

Table 1 provides a summary view of the category name and the category description for the Digital Twin Capability Periodic Table.

| Id | Name                 | Description                                                                                        |
|:---|:---------------------|:---------------------------------------------------------------------------------------------------|
| DS | Data&nbsp;Services   | Enables data access, ingestion and data management across the platform from the edge to the cloud. |
| IR | Integration          | Enables data access to existing internal and external enterprise systems and applications.         |
| IC | Intelligence         | Provides an environment for the development and deployment of industrial digital twin solutions.   |
| UX | User&nbsp;Experience | Provides the user with the ability to interact with digital twins and visualize its data.          |
| MN | Management           | System and ecosystem management capabilities.                                                      |
| TW | Trustworthiness      | Security, privacy, safety, reliability and resilience capabilities.                                |

*Table 1: Digital twins CPT category descriptions.*

The six categories are used in the visual representation of the Digital Twin Capabilities Periodic Table and are represented in Figure \ref{fig:caplevel0}, the Digital Twin Capabilities Periodic Table outline.

![Digital Twin Capabilities Periodic Table outline.](./img/digital_twin_capabilities_level_0.jpg){#fig:caplevel0}

This outline provides the container for each of the 60 Level 1 capabilities of the Digital Twin Capabilities Periodic Table.

### The Digital Twin CPT Level 1

Level 1 represents 60+ high level capabilities that are grouped based on the categories in Table 1 and the outline presented in Figure \ref{fig:caplevel0}.

Figure \ref{fig:caplevel1} is the Digital Twin Capabilities Periodic Table and provides an easy to use framework to describe the key capabilities required for digital twin use cases.

![The Digital Twin Capabilities Periodic Table.](./img/digital_twin_capabilities_level_1.jpg){#fig:caplevel1}

Each of these capabilities may be decomposed into Level 2 sub capabilities to provide more granular elements if the digital twin use case requires clarification.

### The Digital Twin CPT Level 2

Future versions of the Digital Twin CPT may provide specific Level 2 capabilities, but it is suggested that the Level 2 capability requirements are defined on a case-by-case basis in the short term. The machine learning capability may, for example, be decomposed into specific sub-capabilities. In certain instances, it may require a third level breakdown to describe the specific capability that will address the needs of a specific digital twin use case.

![Example of Level 2 and Level 3 breakdown.](./img/digital_twin_capabilities_level_2_example.jpg){#fig:caplevel23}

It is important to note that this is still at capability level and not technology. Each of the capabilities defined at Level 3 for machine learning classification can be achieved with multiple different technologies. This includes Python on Jupyter Notebooks, Azure Machine Learning, AWS Machine Learning and Google Cloud Platform, to name a few typical machine learning technology platforms.

### Capability Deployment Considerations

The requirements of a specific use case will determine the deployment environment for the different capabilities that address the use case.

Some use cases may require the digital twin capabilities at the IoT edge or fog nodes, while others may require cloud processing, and in some instances hybrid deployment models may be needed. It is important to consider the various deployment requirements as part of the digital twin capability specification. The Industry IoT Consortium (IIC), now part of the DTC, provides technical guidance on the characteristics of edge, fog and cloud computing in its [Industrial Internet Vocabulary Technical Report](https://www.iiconsortium.org/foundational-publications.htm).

The accompanying Excel CPT Toolkit makes provisions to identify the required deployment environment for a specific use case. This is demonstrated in the next section on how to use the Digital Twin Capability Periodic Table.

## How to use the Digital Twin Capability Periodic Table

The Digital Twin CPT Toolkit is an Excel template that accompanies this user guide and is aimed at assisting in requirements gathering and capability specification for a specific digital twin use case. The Digital Twin CPT Toolkit contains the template periodic table number, capability description, ability requirements and purpose.

The ability and purpose descriptions for each capability may be edited at an organizational level, but it is suggested to use this as template contained. The specific use case capability requirements, attributes and use case application environment is then completed for each use case. This is demonstrated by the following two use case examples for a wind farm digital twin.

### Windfarm Use Cases Examples

Figure \ref{fig:excel} shows an example of an energy prediction digital twin in a wind farm. The first few columns present the static information from the Digital Twin CPT and the columns marked in orange on the right represent the specific requirements of this use case. This is for illustrative purposes and will vary on the specific application of the digital twin for the end user.

![Example of wind farm Digital Twin CPT Toolkit in Excel.](./img/cpt_toolkit_excel_example.png){#fig:excel}

In this example, the data acquisition and ingestion capability requirement are for real time sensor readings with high frequency and low latency. The specific requirement is 50 tags at a 5 second frequency with a 10-kilobyte payload per message, for 10,000 wind turbines.

It also states that this capability is needed at the edge with potential use in a cloud environment as well. End users can further choose to provide a capability level description such as basic and advanced. It is suggested that each organization create a definition for each of the levels that is suited to the capability maturity management in the organization.

Different use cases will have different CPT representations, and this is illustrated with two simple wind farm examples in Figure \ref{fig:windmon} and Figure \ref{fig:windpredict}.

![Wind farm condition monitoring maintenance digital twin use case.](./img/example_wind_farm_monitoring.jpg){#fig:windmon}

![Wind farm energy prediction operations digital twin use case.](./img/example_wind_farm_prediction.jpg){#fig:windpredict}

The two periodic tables clearly show overlapping capabilities as well as unique requirements that are only applicable for a specific application.

### Digital Twin CPT Workflow Summary

The Digital Twin CPT provides an overall workflow process together and communicates requirements from internal stakeholders as well as outside stakeholders such as technology solution providers.

Figure \ref{fig:worklflow} outlines the suggested workflow, starting with using the periodic table in collaboration meetings and presentations to familiarize stakeholders with all the potential capabilities that can be used in composing digital twins. The single page CPT image is simple to present in executive presentations and demonstrate the specific requirements, as was shown in the wind farm example. It provides clarity and understanding that are especially useful in describing business cases to executives and technical managers. It can be further used to provide estimates for funding requirements.

![Digital twins CPT workflow summary.](./img/cpt_workflow.jpg){#fig:worklflow}

The output of the Toolkit describes all the capability requirements to successfully deliver a digital twin use case. This can be provided to digital twin technology solution providers to propose products and services, either in isolation, or as part of a broader ecosystem. Vendor solutions can be ranked and scored against the Digital Twins CPT Toolkit.

\newpage
# Part II: Updates and Evolution

## Version 1.1 Updates

The release of Version 1.1 in 2023 incorporated valuable insights gathered from a diverse range of organizations that applied the CPT framework in practice. As part of this update, the framework was streamlined from 62 to 60 elements, combining similar capabilities into more comprehensive capability groups. This refinement included the introduction of critical capabilities such as "Search" and "Responsibility," among other adjustments.

A significant enhancement in Version 1.1 was the transition to structured abbreviations for each capability, moving away from sequential numbering. This adjustment aimed to make the CPT not only quicker to reference but also more intuitive and user-friendly, aligning with the goal to enhance accessibility and ease of use.

Another noteworthy update was the redefinition of the "Temporal Data Store" to "Domain Specific Data Management." This change broadened the scope to encompass a variety of data types, including geo-location, image, sound, and temporal or time series data, offering extended support for geo-spatial and other domain-specific data types tailored to organizational needs.

### Change Log

1. Change numbering to descriptive abbreviations.
   - Example 2. Data Streaming to DS.ST Data Streaming

2. Consolidated "23. Edge AI & Intelligence", "31. Artificial intelligence", and "30. Machine Learning" into IC.AI Artificial Intelligence

3. Consolidated "43. Augmented Reality (AR)" and "44. Virtual Reality (VR)" into "UX.XR Extended Reality (XR)"

4. Introduced "IC.SR Search" in the Intelligence category

5. Introduced "TW.RP Responsibility" into the Trustworthiness category

6. Replaced "13. Temporal Data Store" with "DS.DS Domain Specific Data Store" to include lower level data types such as temporal data, geo-location and geospatial data, images, sounds, and other domain-specific data types.

7. Annex A removed from User Guide -- Refer to Excel spreadsheet for detailed descriptions.

### The Introduction of Domain-Specific Data Types

A key change to the Digital Twin Capabilities Periodic Table includes the expansion of the "Temporal Data Store" into a more encompassing "Domain Specific Data Management" capability. This strategic update not only maintains the essential functionality of managing time-series data but also widens the framework's utility by integrating additional data types such as geo-location, images, and audio.

By doing so, it offers a versatile foundation for handling specialized data types, particularly geo-spatial data, which is crucial for organizations needing precise location-based analysis. This shift gears the capability towards a more tailored approach, allowing organizations to leverage specific data types that are critical to their operational context and strategic objectives. Here are two examples of Domain-Specific Data Types that describe the intent of the overall capability.

#### Geospatial Data Including Geo-Location

Core to all digital twins is a virtual representation of the real world --- a digital representation of the real-world objects, entities, facilities, and conditions being modeled in the twin. For many digital twin use cases this includes understanding the location of the assets being represented. The question "where" is at the heart of many digital twins: Where are the rooms in the building? Where are individual buildings related to the larger site and context? Where are the buildings, roads, and other assets in the city, and how do they connect and relate to each other?

Geo-Location is therefore essential to understand the layout and context of the real-world entities being represented. Location intelligence --- the insight gained from visualizing and analyzing data in a locational context --- is an essential capability needed to realize value from digital twin investments.

Key characteristics of geospatial data that organizations should define with respect to their digital twins include the following:

1. Spatial extent
2. Fidelity and level of development (LOD)
3. Locational reference (coordinate) systems
4. Spatial units
5. Map scale and measurement units
6. File types and data storage
7. Content organization (standards and schema)
8. License and access restrictions
9. Privacy and security

By selecting the locational model(s) and describing the corresponding key attributes of those locational models, organizations will then be able to describe their digital twin locational capabilities in a detailed and structured fashion, in turn supporting digital twin design and solution development.

Regardless of the scope and scale of a digital twin or what lifecycle phase(s) the twin is focused on --- planning, design, construction, or operations --- location matters. Most digital twins are not possible, or are certainly less capable, without location. As a "mirror of the real world", there is no twin without location.

#### Temporal Data

Temporal (time-series) data plays a critical role in the operation of real-time operational digital twins by capturing and analyzing data points over time. This kind of data is essential for monitoring, controlling, and optimizing the performance and health of complex systems in real-time. A temporal data store, therefore, becomes a key capability, ensuring that this time-sensitive information is systematically stored and accessed. This capability allows digital twins to provide actionable insights and value, particularly in environments where timing and historical context are crucial for decision-making.

For example, consider a wind farm utilizing digital twins for both operational efficiency and predictive maintenance. The digital twin collects real-time telemetry data such as wind speed, yaw, and power generated. This operational data is crucial for adjusting settings in real-time to maximize power generation efficiency.

Concurrently, the digital twin also gathers asset performance data, including gearbox speed, temperature, and vibration. This information is vital for identifying patterns or anomalies that may indicate potential failures or maintenance needs before they escalate into more significant issues.

This scenario describes the use of a temporal (time-series) data store as a "Sub-Capability" under the broader "Domain Specific Data Store" capability. However, it's particularly relevant for users focused on real-time performance data. By capturing and analyzing both operational metrics and asset condition over time, stakeholders can optimize performance and pre-emptively address maintenance issues, leading to improved efficiency and reduced downtime.

This targeted application of the temporal data store capability demonstrates how domain-specific data management strategies can be tailored to meet the unique needs of different users and use cases for digital twins.

### Technology Showcases

The Digital Twin Consortium's [Technology Showcases](https://www.digitaltwinconsortium.org/initiatives/technology-showcase/) delve into the core technologies, methodologies, and strategies essential to the development and application of digital twins. These showcases not only present the practical benefits digital twins offer across a range of industries but also underscore their adaptability and transformative potential.

Each showcase is mandated to illustrate its alignment with the Capabilities Periodic Table, ensuring a comprehensive demonstration of its utility and integration.

## Future Work

With the introduction of the computable CPT format in Version 1.2, we see several exciting avenues for future development:

1. **Enhanced AI Integration** - Further development of generative AI tooling that leverages the computable CPT format for automated digital twin design and capability assessment.

2. **Extended Formats** - Development of additional generators for other useful formats beyond the current YAML, JSON, XLSX, and PowerPoint options.

3. **Level 2 Capabilities** - Detailed descriptions for each of the capability elements in the Digital Twins CPT, enhancing granularity for specific use cases.

4. **Capability Maturity Model** - Development of a comprehensive index that organizations can use to score progress towards more mature digital twins.

5. **Integration APIs** - Creating standardized APIs for integrating the computable CPT into digital twin platforms and development environments.

Other future work may include alignment with other DTC initiatives, including business maturity frameworks, interoperability models and reference architectures.

# Part III: Annexes

## Available CPT Formats

The CPT is now available in the following machine-readable formats:

1. **YAML** - The base format that serves as the source of truth for the CPT data structure
2. **JSON** - For integration with web applications and services
3. **XLSX** - Excel format for traditional spreadsheet analysis and reporting
4. **PowerPoint** - For presentation and communication purposes

The detailed descriptions of each capability are maintained in the YAML source file and available in all derived formats including the companion Excel spreadsheet.

## Authors and Legal Notice

Copyright &copy; 2025, Digital Twin Consortium&reg;, a program of Object Management Group, Inc. ("OMG&reg;"). All other trademarks in this document are the properties of their respective owners.

This document is a work product of the Composability Framework Subgroup, co-chaired by Pieter van Schalkwyk (XMPro), and Sean Whiteley (Axomem).

**Authors:** Pieter van Schalkwyk (XMPro), Sean Whiteley (Axomem), Marc Goldman (Esri).

**Contributors:** The DTC's Composability Framework Subgroup collectively provided input.

**Technical Editor:** Dan Isaacs (DTC CTO) oversaw the process of organizing the contributions of the above Authors and Contributors into an integrated document.

All copying, distribution and use are subject to the limited License, Permission, Disclaimer and other terms stated in the Digital Twin Consortium Use of Information -- Terms, Conditions & Notices. If you do not accept these Terms, you are not permitted to use the document.