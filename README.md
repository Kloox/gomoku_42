<h1>GOMOKU</h1><br />
<br />

<h2>Description</h2>
The goal of this project is to make an AI capable of beating human players at Gomoku with a 500ms constraint to play its turn.
This project IA using an alpha beta pruning algo with a homemade heuristic.
The GUI is made with a golang library named Pixel (based on OpenGL).
<br/>

<h2>Installation</h2><br />

Requirements: `Golang version >= 1.13.0`.<br/>

You must install the following dependencies : `libasound2-dev`, `libgl1-mesa-dev` and `xorg-dev`.</br>

<h3>On Linux:</h3><br/>

`make linux-deps`<br/>
`make goget`<br />
`make`<br />
<br />
You can now run gomoku. :)

<h3>On Windows:</h3>

You can use the precompiled executable in folder `gomoku-W64-1.0.0`.

or

Compiled the project on WSL and using a tool like Xlaunch to be able to launch the project.

or 

Compiled the project on Mingw-w64 with:

`make goget`<br/>
`make windows`<br/>

(You still nedd install the proper dependencies on Mingw-w64).<br/>

You can now run gomoku. :)

<h2>Parameters</h2><br />

`-d or --depth <int> :` Set the depth of the Alpha Beta pruning algo. (default: 5)<br/>
`-w or --width <int> :` Set the width of the Alpha Beta pruning algo. (default: 8)<br/>
`-r or --routine :` Disable go routine (Debug purpose).<br/>
`-ia:` An IA plays for you (Debug purpose)<br/>

Note: The default depth and width is a compromise between performance and efficiency. High values can lead to very long computation time.<br/>

<h2>Rules:</h2><br />

- To win you must do a 5-in-row.

- You can capture a pair of your ennemy stones, 5 capture lead to a win. If your 5-in-row is threatened by a capture, you won't win. (Can be disabled on the main menu)<br/>

- A double three is not allowed. (Can be disabled on the main menu)<br/>

- Detailed rules in the subject: [here](./en.subject.pdf)<br/>

<h2>Controls</h2><br />

The game can completely be play with the mouse, but here are some shortcuts:<br/>
`CTRL + Z`: Undo<br/>
`CTRL + R`: Reset game<br/>
`CTRL + H`: Gives you a hint<br/>
`CTRL + S`: Save game (you can load it on the main menu)<br/>
`CTRL + C`: Show the potential captures on board (cheating is bad :) )<br/>
`CTRL + V`: Activate vsync<br/>
`CTRL + F`: Fullscreen mode<br/>
`CTRL + A`: Activate AA (smooth mode)<br/>

<h2>Screenshots</h2>

<img src="screenshots/gomoku_main.png"
     alt="Main menu screenshot"
     style="float: left; margin-right: 10px;" />
<br/>

<img src="screenshots/gomoku_game.png"
     alt="Game screenshot"
     style="float: left; margin-right: 10px;" />
<br/>

<h2>Grade</h2>

`124/100`