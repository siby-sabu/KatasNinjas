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

