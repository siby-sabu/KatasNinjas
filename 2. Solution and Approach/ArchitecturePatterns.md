# Architecture Patterns
## Identified Key Architecture Characteristics
The key architecture characteristics identified are as follows:
- Availability
- **Scalability**
- **Integration**
- Data Integrity
- **Fault Tolerance**
- **Workflow**
- Security
- **Performance**

## Architecture Capabilities Comparision
The above characteristics in bold are used to compare betwen different architecture patterns

![Comparision of Architecture](../assets/compare.png)

## Architecture Capability Analysis  

From Above matrix we have shortlisted the below architectures for MonitorMe application 

### Event Driven Architecture 

 Fault Tolerance, Modularity, Performance and Scalability score highly, which makes it ideal for data analysis and data propagation scenarios. 

Workflow scores highly, important for sending notification details to medical staff. 

Interoperability and Integration has middling score. 

### Service Based Architecture 

Scores highly on Modularity, Fault-Tolerance and Testability, all three important to development of a new system and data manipulation and data analysis. 

Although it apparently scores low on scalability, these low scores can be raised by using event-driven architecture 

The low score for workflow can also be mitigated by using event-driven architecture. 

 

## Conclusion 

Above two architectures have trade-offs, but they can be mitigated by leveraging the high scoring features of each architecture. We would be using the best characteristics of both the architecture. 