# Guide to Software Architecture Design Docs

> [!TIP]
> - Architecture is about intent.
> - A good architecture allows major decisions to be deferred.
> - Allows you to make decisions late, decisions about UI, database, and framework, because you can implement all the use cases without them
> - A good architect maximizes the number of decisions not made.
> - Later is always better when you're making decisions, you have more information later.
> - Create an **easy to maintain, test, and extend** system.
> - This is for designing a new system
>
> Reference: [The Clean Architecture](../learning-resource/the-clean-architecture.md)

## Context and scope

Provide an overview of the product and user journeys

**Goals**

- Requirements and specifications
- Describe the user-driven impact of your project — where your user might be another engineering team or even another technical system
- Specify how to measure success using metrics — bonus points if you can link to a dashboard that tracks those metrics

**Non-Goals**

- Non-goals are equally important to describe which problems you won't be fixing so everyone is on the same page.

## System building blocks

**System Overview**: Provide a general description and functionality of the software system.

**System Architecture**: This section should provide a high-level overview of how the functionality and responsibilities of the system were partitioned and then assigned to subsystems or components.

**Relationship to other systems**

**Detailed System Design**: Most components described in the system architecture section will require a more detailed discussion. Other lower-level components and subcomponents may need to be described as well.

## Software architecture

<ins>Software stack diagram</ins>

Architectural Strategies: Describe the strategies that will be used that will affect the system.

Diagram: A software stack diagram to highlight all the layers and modules

<ins>Interfaces and data structure</ins>

Describe every layer and module, and indicate the inputs and outputs of each module

<ins>Procedures, object lifecycle, and data pipeline</ins>

Indicate how the modules across layers process the data, including handler/data lifecycle

## Design considerations

Design Considerations: Describe the issues that need to be addressed before creating a design solution:

- Assumptions and Dependencies: Describe any assumptions that may be wrong or any dependencies on other things.
- General Constraints: Describe any constraints that could have an impact on the design of the software.
- Goals and Guidelines: Describe any goals and guidelines for the design of the software.
- Development Methods: Describe the software design method that will be used.

Policies and Tactics: Describe any design policies and/or tactics that do not have sweeping architectural implications (meaning they would not significantly affect the overall organization of the system and its high-level structures).

Glossary: An ordered list of defined terms and concepts used throughout the document.

## Sample structure

- Building block
- Software stack
- Implementation: Interface and data structure
- Implementation: Procedure and lifecycle
- Design considerations
