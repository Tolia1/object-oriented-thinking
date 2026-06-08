### Class: User
| Collaborators  | Responsibilities                                 |
|:---------------|:-------------------------------------------------|
| StaffMember    | Provides the document source to the staff member |
| DocumentSource | Receives the result                              |
| Result         |                                                  |

### Class: StaffMember
| Collaborators  | Responsibilities                           |
|:---------------|:-------------------------------------------|
| User           | Receives the document source from the user |
| DocumentSource | Extracts the document from the source      |
| Document       | Provides the document to the printer       |
| Result         | Receives the result                        |
| Printer        | Provides the user with the result          |

### Class: Printer
| Collaborators | Responsibilities    |
|:--------------|:--------------------|
| Document      | Receives document   |
| Result        | Produces the result |

### Class: DocumentSource
| Collaborators | Responsibilities    |
|:--------------|:--------------------|
| Document      | Produces document   |