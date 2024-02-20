# Architecture Analysis
## Key Architecture Characteristics
We have identified the key architecture characteristics best suited for the problem statement as per requirements.
|Characteristic|Source|
|--------------|------|
|Availability|MonitorMe should be up and running at all times|
|Scalability|Additional vital sensors are likely to be incorporated in the future|
|Integration|Integration with **MyMedicalData** (Cloud based platform) to upload snapshots of patient's vital data analysis|
|Data Integrity|Generate analysis on the medical data and generate alerts based on rules on the same. Data must be accurate as it is patient's vital records|
|Fault Tolerance|If any service faces a downtime, that should not stop the softeare from functioning|
|Workflow|Consolidated vitals' information has to be sent to nurse's station. It should also generate analysis and alerts|
|Security|Patient records as well as staff information should be secured.|
|Performance|MonitorME must be efficient in generating analysis and rendering consolidated data to medical staff|

Apart from the above characteristics , the architecture would also have the below features: 
- Maintainability
- Authentication and Authorization

## Architectural Quanta
We have identified the following Quanta and corresponsing architecture characteristics:

|Quanta|Consideration|Architecture Characteristics|
|------|-------------|----------------------------|
|Security|Patient admission for medical care|Authorization, Authentication|
|Sensor Recognition|Reading patient's vital sensor data and persisting the data for further manipulation|Fault Tolerance, Data Integrity, Scalability|
|Analytics|Encompasses providing an interface for medical staff to analyze recorded data|Availability, Data Integrity, Fault Tolerance, Performance|
|Monitoring|Must analyze each patient's vital data and provide consolidated view|Availability, Performance|
|Notification Service|Must analyze patient data based on certain rules, and alert medical professional in case of any issue| Workflow, Performance, Authorization, |
|Snapshot Data Upload|Generate holistic patient vital sign snapshots for uploading to MyMedicalData|Integrity|

