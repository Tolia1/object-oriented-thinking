## UC-1: Print Digital Document from USB
### Background information:
- **System:** the printer/copier device
- **Primary actor:** person who needs to print document 
- **Secondary actor:** staff member
- **Goal:** create physical document for the user
- **Preconditions:** primary actor has the privilege to use the device; it is university working hours; user has USB device with a document to print
### Scenarios:
- **Basic flow:** User provides the USB device to the staff member. The member prints the document and gives it and USB back to the user. User leaves
- **Alternate flow 1:** User provides the USB device to the staff member. The desired file is corrupted. Printing is not possible, user has to leave

## UC-2: Print Digital Document via email
### Background information:
- **System:** the printer/copier device
- **Primary actor:** person who needs to print document
- **Secondary actor:** staff member
- **Goal:** create physical document for the user
- **Preconditions:** primary actor has the privilege to use the device; it is university working hours
### Scenarios:
- **Basic flow:** User sends the document to the specified email address. The member prints the document and gives it to the user. User leaves
- **Alternate flow 1:** User sends an email but the staff member does not receive it. Printing is not possible, user has to leave

## UC-3: Copy Physical Document
### Background information:
- **System:** the printer/copier device
- **Primary actor:** person who needs to copy a document
- **Secondary actor:** staff member
- **Goal:** create physical copy of the document for the user
- **Preconditions:** primary actor has the privilege to use the device; it is university working hours
### Scenarios:
- **Basic flow:** User brings a document to be copied and hands it over to the staff member. The document is scanned. Physical copy is created. User receives initial document and the copy and leaves