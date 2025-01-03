# Introduction to Sociotechnical Architecture Maps

Sociotechnical Architecture Maps (STA-Maps) offer open and adaptable elements for the visualization of sociotechnical systems and architectures. They are able to provide a holistic overview of the building blocks and espcially their dynamics and dependencies for complex and adaptive systems. STA-Maps aim to be flexible and help in visualizing and discussing the trade-offs of complex sociotechnical systems and their evolution. Explicitly STA-Maps offer no best practices or one-size-fits-all solutions.

## Why would I use STA-Maps

STA-Maps help you to visualize and discuss topics like:

- Aligments between domains, teams, bounded contexts, software modules and deployment units (like monoliths or microservices)
- Depth of coupling between various elements of a system
- Cross-team coordination and requirements processes
- Technical Integration and manual organizational solutions
- Power dynamics between teams and their responsibilities
- Cognitive load of teams

## Inspiration for STA-Maps

STA-Maps were not invented from the ground up, instead they were heavily inspired by visualization techniques for software architectures (such as C4, Arc42 or 4+1), Context Maps from Domain Driven Design and Team Topologies.

STA-Maps don't aim to replace any of these approches. Instead they offer some more opinionated interpretations of these ideas and a connection between them towards a more holistic perspective.

## Principles of STA-Maps

### Flexibility

STA-Maps refrain from having a structure of fixed views. You can build your own views. In order to get you started they offer some views that may come in handy but you should not treat them as the "official STA-Maps views", they are just ideas and proposals.

### Open for extension

You are missing something? No problem: just add your building block, team dependency or -relationship. Don't hesitate for open a pull request if you think that others can benefit from your idea.

### Trade-Offs instead of templates

STA-Maps don't tell you what is right or wrong. Instead they help you to visualize trade-offs in order to better discuss them. STA-Maps don't propagate patterns or anti-patterns. Neither do they offer "best practices".

### Collaborative

STA-Maps are collaborative. They should not be used in an ivory tower telling others what to do. STA-Maps are there for modeling and reasoning about sociotechnical systems in a collaborative fashion.

## Elements of STA-Maps

### Building Blocks
- Value Stream 
- Domain
- Sub-Domain
- Bounded Context
- Software Architecture Module
- System (aka. Deployment Unit)
- Team

![Building Blocks](resources/STA-Maps-BuildingBlocks.jpg "STA-Maps Building Blocks")

### Relationships
- Integration
  - API
  - UI-based Integration
  - Manual or Organizational
- Model Propagation
  - Model-to-Model Transformation
  - Cloned Model
  - Shared Model
- Team Interaction
  - Collaboration
  - Customer-Supplier (limited / unlimited)
  - Facilitation
  - Veto-based
- Team Dependencies
  - Mutual
  - Upstream / Downstream
  - Free
  
## Possible Perspectives of STA-Maps

### Alignments

With STA-Maps you are able to visualize various aligment scenarios for the building blocks like:

- How are bounded contexts aligned to subdomains?
- How are modules bundled into systems (aka deployment units)?
- Which modules are aligned to bounded contexts and how good is their aligment?
- Which teams have an end-to-end responsibility for which systems or modules or bounded context

This list could go on forever. STA-Maps don't impose a fixed structure, they offer building blocks which you can arrange how you see fit.

### Cross-Team Dynamics

STA-Maps enable you to visualize and reason many settings for cross-team dynamics like:

- Where is long lived, purpose-less collaboration between teams?
- Does one team raises requirements against another team?
- Does a team have veto rights against changes of other teams?
- Is a team facilitating for other teams?
- Do we have a clear self-service, no-communication-neccessary X-as-a-Service dynamic between teams
- Are there organizational, manual business processes between teams? 

### Coupling on APIs and Models

With STA-Maps you can take a deep dive look into the topic of coupling at the level of APIs and Models:

- Where are APIs tailored to many consumers without having "special features" for specific consumers?
- Where are consumer-specific Point-To-Point APIs / Connections between modules or systems?
- Is the model, which is provided by an API based on a standard (such as vCard or iCalendar) or is it proprietary?
- Where do systems or modules share artifacts such as database schemas or shared libraries?
- Does a system or module copy an external model into their own domain model?
- Does a system or module transform the model of an external API towards it's own model?
