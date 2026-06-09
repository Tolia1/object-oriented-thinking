### Interface: ChessPiece
| Collaborators | Responsibilities                    |
|:--------------|:------------------------------------|
| ChessTable    | Is moved on the table by the player |
| Player        | Can capture opponents pieces        |

### Class: ChessTable
| Collaborators | Responsibilities            |
|:--------------|:----------------------------|
| ChessPiece    | Is displayed to the players |
| Player        | Contains chess pieces       |
| Game          | Exists within a game        |

### Class: Game
| Collaborators | Responsibilities         |
|:--------------|:-------------------------|
| ChessTable    | Is played by the players |
| Player        | Has a chess table        |

### Class: Player
| Collaborators | Responsibilities               |
|:--------------|:-------------------------------|
| Game          | Plays the game                 |
| ChessTable    | Observes the table with pieces |
| ChessPiece    | Moves his pieces on his turn   |

### Class: Turn
| Collaborators | Responsibilities                         |
|:--------------|:-----------------------------------------|
| Game          | Players take a turn while playing a game |
| Player        |                                          |
