# Multiplayer-game

<img src="https://giphy.com/gifs/atatlfP16QKOEcrqBW/fullscreen" width="880" height="500" />

In week 7 of the Codaisseur Academy we were challenged to build a multiplayer game upon a Tic-Tac-Toe logic which was provided. What we did was:

- Extending the board from 9x9 to 12x22 and used this as a grid for the board.
- Added two players to the board which can move using different computers and keyboard arrows. 
- Changed the 'turn-based-play' into a asynchronous game, so both players are free to move.
- Added monsters to the board which move either randomly or structured each time a  player makes a move. 
- Adjusted the login and authorization to support our gameplay.
- Fixed additional bugs such as the possibility to walk off the board.
- Added styling with CSS.

## Gameplay
- Once setup two players on different computers can challenge each other. 
- One player creates a new game, the other joins it. 
- As a player you need to fly to the other side of the screen. Whoever reaches the opposite side first, wins the game. 
- But watch out for the flying monsters!! Once you get hit, you will be set back to your start position. 

## How to get started. 

To start our app:

1) git clone repro.
2) comment out line 55 and 56 in /client/games/entities.ts.
3) cd to /server and run 'npm install'
4) in same terminal, run 'npm run dev'. Leave open.
5) run a local Postgres DB.
6) make sure the server connects to the same port as the local postgres.
7) comment line 55 and 56 back in. 

8) cd to /client and run 'npm install'
9) in same terminal, run 'npm run start'. Leave open.
10) open a incognito window and browse to the same localhost.
11) you're good to go!

TO PLAY ON DIFFERENT COMPUTERS
1) run everything above on one computer.
2) change 'localhost' in /client/src/constants.js to your local IP address.
3) change 'localhost' in /server/src/db.ts to your local IP address.
4) on another computer browse to the {IP address}:{port}/games.

## Authors

* **Vincent de Graaf** - *Initial work* - [vdegraaf](https://github.com/vdegraaf)
* **Danielle Repko** - *Initial work* - [drepko](https://github.com/drepko)
