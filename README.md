# CS240_CONNECT_FOUR

## Elevator Pitch


Connect Four is a classic two-player game of skill. Each player takes turns placing disks into columns. 
The first person to place four of their disks in a row, column, or diagonally wins. 
While the concept is simple, Connect Four requires calculations and skill in order to win. 
By creating a Connect Four website, people can play against a bot, or with a friend.

## Design

![Mock](connectFourUI.jpg)

Here is a diagram showing how players would interact with the backend to play:


```mermaid
sequenceDiagram
    actor Hayden
    actor Sarah
    Hayden->>Server: New Game request
    Sarah->>Server: New Game request
    Server-->>Hayden: Game ID
    Server-->>Sarah: Game ID
    Hayden->>Server: Move
    Server-->>Sarah: Move
    Sarah->>Server: Winning Move
    Server->>Database: Game
```