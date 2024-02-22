# Security in MonitorMe

MonitorMe is fully on premise solution for hospitals to track their patients and monitor their health on a real time basis. 

## Key Considerations

1. No external entity or stakeholder with the exception of Nurses or Doctors will be able to interact with the system due to the nature of the architecture.
2. All API and Route calls made will strictly be done by the sub modules or services itself without any opportunity of an external interaction.


## Identity and Access Management

- When it comes to medical data, authentication and authorization is paramount to determine which actors have access to which data.
- Single Sign On ( SSO ) can be utilized to restrict users based on their identity or level of access. These restrictions will apply on the mobile application as well as the MonitorMe frontend application ( For example: Only users with a doctor level of access will be able to access the patient history record)
- The OIDC (OpenID Connect) protocol makes it really simple to implement a login module that can be used across platforms ( mobile and web ) and provides great flexibility around developement. It also provide an ability to authorize users to the right level of access that can be configured and controlled easily at a single user id level.


## Data Security

- To decouple critical patient data and their health readings, two databases have been utilized in MonitorMe. The InfluxDb is solely used to store health readings without a direct corelation of patient data in the same system.
- Memgraph is used to store patient data and their doctor, nurse, nursing station mappings. Besides this, the database server will be independent of the webapp servers to prevent loss in case of a system down or attack.
- A tiered level of access to the database also gurantees security of the data.
- Passwords for all systems can be be tracked and secured using a password manager ( NAPS ) to prevent breaches.
- Encrypt data during transmissions between systems.


## Future Scope

- Have Disaster Recovery strategies in place with adequate access levels in case the infrastructure were to down.
- 




