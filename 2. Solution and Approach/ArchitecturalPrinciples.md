# Architectural Principles

This solution involves the following high-level Architectural Priniciples to address its concepts:

## Overall Architecture

* Modular Architecture - Modularity principle defines entities with their scope well-defined which is then used to scale and achieve complex solutions by a combination of several such independent modules.
    * Rationale: Modularity allows for a better maintenance and improved flexibility with neatness.
* Pattern-based Architecture: Patterns allow for relationship and generalization of context.
    * Rationale: Realizing patterns enhances understanding of the model and adds more detail on it.
* Polling Architecture - Polling continuously checks for gathering a required input. This may also be possible on a chosen interval.
    * Rationale: Polling method allows for continuous updation without having to queue for multiple requests as in case of event-driven architecture.

## Considerations

* Security: Incorporating security into the architecture is essential for prevention of any tampering with the information and execution. Reliance over the solution depends highly on its security ensured at every stage using authentication, encryption, access restrictions and similar strategies. 
* Integratibility: Interfaces for each entity have their endpoints and exchange mechanisms to allow seamless integratibility with each other.
* Extendability and Maintainability: Design prevents cluttering and defines processes completely to enable its maintainability and future extensibility.