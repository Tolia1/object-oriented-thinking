## UC-1: Restock Warehouse
### Background information:
- **System:** warehouse management system
- **Primary actor:** the system
- **Goal:** distribute, and store incoming products
- **Preconditions:** products have arrived to the warehouse
### Scenarios:
- **Basic flow:** Package of products is delivered to the receiving zone. The package weight is measured, codes are scanned. 
System receives the info and makes decisions for the storage destination and robot responsible for the job.
System notifies the robot. Robot moves the package and returns to the pit. Info about the task, package and other information is written to the database

## UC-2: Report Generation
### Background information:
- **System:** warehouse management system
- **Primary actor:** the system
- **Secondary actor:** staff member
- **Goal:** generate a report
- **Preconditions:** staff member is successfully authorized in the system, frontend system is used to communicate with API
### Scenarios:
- **Basic flow:** Staff member enters input data and submits it using fronted app. API receives the call. The system checks access token. 
In case of success database is queried and report is generated. Report is returned to the frontend app
- **Alternate flow 1:** Staff member enters input data and submits it using fronted app. API receives the call. The system checks access token.
Token appears to be invalid. Error code is returned to the frontend app
