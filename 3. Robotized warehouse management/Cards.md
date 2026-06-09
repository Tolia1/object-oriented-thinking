### Class: Robot
| Collaborators   | Responsibilities                                      |
|:----------------|:------------------------------------------------------|
| Package         | Carries the package to destination cell               |
| StorageCell     | Receives package and destination data from dispatcher |
| RobotController |                                                       |

### Class: RobotController
| Collaborators | Responsibilities                |
|:--------------|:--------------------------------|
| Robot         | Manages robots                  |
| Dispatcher    | Receives tasks from dispatcher  |
| Database      | Provides the database with data |

### Class: Scanner
| Collaborators | Responsibilities                        |
|:--------------|:----------------------------------------|
| Package       | Receives input package                  |
| Dispatcher    | Scans the package                       |
|               | Provides dispatcher with retrieved data |

### Class: Package
| Collaborators | Responsibilities      |
|:--------------|:----------------------|
| Scanner       | Is scanned by scanner |
| Robot         | Is moved by robot     |

### Class: Dispatcher
| Collaborators   | Responsibilities                     |
|:----------------|:-------------------------------------|
| Scanner         | Receives data from scanner           |
| RobotController | Provides robot controller with tasks |
| Database        | Provides the database with data      |
| Storage         | Gets available storage data          |

### Class: API
| Collaborators | Responsibilities                 |
|:--------------|:---------------------------------|
| Database      | Retrieves data from the database |

### Class: StorageCell
| Collaborators | Responsibilities |
|:--------------|:-----------------|
| Package       | Stores a package |

### Class: Storage
| Collaborators | Responsibilities             |
|:--------------|:-----------------------------|
| StorageCell   | Contains storage cells       |
| Dispatcher    | Gives data to the dispatcher |

### Class: Task
| Collaborators | Responsibilities                            |
|:--------------|:--------------------------------------------|
| Package       | Has data about the package                  |
| StorageCell   | Has data about the destination storage cell |
| Robot         | Is assigned to a robot                      |
