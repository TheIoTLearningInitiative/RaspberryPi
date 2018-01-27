# User Directory

## Command tree

```
TREE(1)                     General Commands Manual                    TREE(1)

NAME
       tree - list contents of directories in a tree-like format.

SYNOPSIS
       tree  [-acdfghilnpqrstuvxACDFQNSUX]  [-L  level [-R]] [-H baseHREF] [-T
       title] [-o filename] [--nolinks] [-P pattern] [-I  pattern]  [--inodes]
       [--device] [--noreport] [--dirsfirst] [--version] [--help] [--filelimit
       #]  [--si]  [--prune]  [--du]  [--timefmt  format]  [--matchdirs]  [--]
       [directory ...]

DESCRIPTION
       Tree  is  a  recursive  directory listing program that produces a depth
       indented listing of files, which is  colorized  ala  dircolors  if  the
       LS_COLORS  environment  variable  is set and output is to tty.  With no
       arguments, tree lists the files in the current directory.  When  direc‐
       tory  arguments  are given, tree lists all the files and/or directories
       found in the given directories each in turn.  Upon completion of  list‐
       ing all files/directories found, tree returns the total number of files
       and/or directories listed.
...
```

```sh
pi@raspberrypi:~ $ tree
.
├── Desktop
├── Documents
│   ├── BlueJ Projects
│   │   ├── appletdemo
│   │   │   ├── CaseConverter.java
│   │   │   ├── package.bluej
│   │   │   └── README.TXT
│   │   ├── debugdemo
│   │   │   ├── Car.java
│   │   │   ├── Demo.java
│   │   │   ├── package.bluej
│   │   │   └── README.TXT
│   │   ├── file-reader
│   │   │   ├── FileReader.java
│   │   │   ├── package.bluej
│   │   │   ├── README.TXT
│   │   │   └── test.txt
│   │   ├── hello
│   │   │   ├── Hello.java
│   │   │   ├── package.bluej
│   │   │   └── README.TXT
│   │   ├── LED-Button
│   │   │   ├── Button.ctxt
│   │   │   ├── Button.java
│   │   │   ├── LED.ctxt
│   │   │   ├── LED.java
│   │   │   ├── LEDTester.ctxt
│   │   │   ├── LEDTester.java
│   │   │   ├── package.bluej
│   │   │   ├── README.TXT
│   │   │   ├── StringToMorse.ctxt
│   │   │   └── StringToMorse.java
│   │   ├── LICENSE.txt
│   │   ├── people
│   │   │   ├── Database.class
│   │   │   ├── Database.ctxt
│   │   │   ├── Database.java
│   │   │   ├── package.bluej
│   │   │   ├── Person.class
│   │   │   ├── Person.ctxt
│   │   │   ├── Person.java
│   │   │   ├── README.TXT
│   │   │   ├── Staff.class
│   │   │   ├── Staff.ctxt
│   │   │   ├── Staff.java
│   │   │   ├── Student.class
│   │   │   ├── Student.ctxt
│   │   │   └── Student.java
│   │   ├── people2
│   │   │   ├── Address.java
│   │   │   ├── Database.java
│   │   │   ├── package.bluej
│   │   │   ├── Person.java
│   │   │   ├── README.TXT
│   │   │   ├── Staff.java
│   │   │   └── Student.java
│   │   ├── picture
│   │   │   ├── Canvas.java
│   │   │   ├── Circle.java
│   │   │   ├── package.bluej
│   │   │   ├── Picture.java
│   │   │   ├── README.TXT
│   │   │   ├── Square.java
│   │   │   └── Triangle.java
│   │   ├── README.TXT
│   │   ├── shapes
│   │   │   ├── Canvas.java
│   │   │   ├── Circle.java
│   │   │   ├── package.bluej
│   │   │   ├── README.TXT
│   │   │   ├── Square.java
│   │   │   └── Triangle.java
│   │   └── THIRDPARTYLICENSE.txt
│   ├── Greenfoot Projects
│   │   ├── API
│   │   │   ├── allclasses-frame.html
│   │   │   ├── allclasses-noframe.html
│   │   │   ├── constant-values.html
│   │   │   ├── deprecated-list.html
│   │   │   ├── greenfoot
│   │   │   │   ├── Actor.html
│   │   │   │   ├── Greenfoot.html
│   │   │   │   ├── GreenfootImage.html
│   │   │   │   ├── GreenfootSound.html
│   │   │   │   ├── MouseInfo.html
│   │   │   │   ├── package-frame.html
│   │   │   │   ├── package-summary.html
│   │   │   │   ├── package-tree.html
│   │   │   │   ├── UserInfo.html
│   │   │   │   └── World.html
│   │   │   ├── help-doc.html
│   │   │   ├── index-all.html
│   │   │   ├── index.html
│   │   │   ├── overview-tree.html
│   │   │   ├── package-list
│   │   │   ├── resources
│   │   │   │   ├── background.gif
│   │   │   │   ├── tab.gif
│   │   │   │   ├── titlebar_end.gif
│   │   │   │   └── titlebar.gif
│   │   │   └── stylesheet.css
│   │   ├── GREENFOOT_LICENSES.txt
│   │   ├── LICENSE.txt
│   │   ├── README.txt
│   │   ├── scenarios
│   │   │   ├── ants
│   │   │   │   ├── AntHill.java
│   │   │   │   ├── Ant.java
│   │   │   │   ├── AntWorld.java
│   │   │   │   ├── Counter.java
│   │   │   │   ├── Creature.java
│   │   │   │   ├── Food.java
│   │   │   │   ├── images
│   │   │   │   │   ├── ant.gif
│   │   │   │   │   ├── anthill.png
│   │   │   │   │   ├── ant-with-food.gif
│   │   │   │   │   ├── Counter.png
│   │   │   │   │   ├── Food.png
│   │   │   │   │   ├── Pheromone.png
│   │   │   │   │   └── sand.jpg
│   │   │   │   ├── Pheromone.java
│   │   │   │   ├── project.greenfoot
│   │   │   │   ├── README.TXT
│   │   │   │   └── sounds
│   │   │   ├── LTA
│   │   │   │   ├── Car.java
│   │   │   │   ├── Ground.java
│   │   │   │   ├── images
│   │   │   │   │   ├── car01.png
│   │   │   │   │   ├── ground2.png
│   │   │   │   │   └── ground.png
│   │   │   │   ├── project.greenfoot
│   │   │   │   ├── README.TXT
│   │   │   │   └── sounds
│   │   │   └── lunarlander
│   │   │       ├── Explosion.java
│   │   │       ├── Flag.java
│   │   │       ├── images
│   │   │       │   ├── explosion.png
│   │   │       │   ├── flag.png
│   │   │       │   ├── moon.jpg
│   │   │       │   ├── rocket.png
│   │   │       │   └── thrust.png
│   │   │       ├── Lander.java
│   │   │       ├── Moon.java
│   │   │       ├── project.greenfoot
│   │   │       ├── README.TXT
│   │   │       └── sounds
│   │   │           └── Explosion.wav
│   │   ├── THIRDPARTYLICENSE.txt
│   │   └── tutorial
│   │       ├── tutorial-files
│   │       │   ├── decor2-1.jpg
│   │       │   ├── greenfoot.jpg
│   │       │   ├── kent.png
│   │       │   ├── tutorial.css
│   │       │   ├── wombat-menu.png
│   │       │   └── wombats.png
│   │       └── tutorial.html
│   └── Scratch Projects
│       ├── Asteroid Blaster.sb
│       ├── Pacman for Scratch.sb
│       └── Scratch Invaders.sb
├── Downloads
├── Music
├── Pictures
├── Public
├── python_games
│   ├── 4row_arrow.png
│   ├── 4row_black.png
│   ├── 4row_board.png
│   ├── 4row_computerwinner.png
│   ├── 4row_humanwinner.png
│   ├── 4row_red.png
│   ├── 4row_tie.png
│   ├── badswap.wav
│   ├── beep1.ogg
│   ├── beep2.ogg
│   ├── beep3.ogg
│   ├── beep4.ogg
│   ├── blankpygame.py
│   ├── boy.png
│   ├── catanimation.py
│   ├── catgirl.png
│   ├── cat.png
│   ├── drawing.py
│   ├── flippybackground.png
│   ├── flippyboard.png
│   ├── flippy.py
│   ├── fourinarow.py
│   ├── gameicon.png
│   ├── gem1.png
│   ├── gem2.png
│   ├── gem3.png
│   ├── gem4.png
│   ├── gem5.png
│   ├── gem6.png
│   ├── gem7.png
│   ├── gemgem.py
│   ├── grass1.png
│   ├── grass2.png
│   ├── grass3.png
│   ├── grass4.png
│   ├── Grass_Block.png
│   ├── horngirl.png
│   ├── inkspilllogo.png
│   ├── inkspill.py
│   ├── inkspillresetbutton.png
│   ├── inkspillsettingsbutton.png
│   ├── inkspillsettings.png
│   ├── inkspillspot.png
│   ├── launcher.sh
│   ├── match0.wav
│   ├── match1.wav
│   ├── match2.wav
│   ├── match3.wav
│   ├── match4.wav
│   ├── match5.wav
│   ├── memorypuzzle_obfuscated.py
│   ├── memorypuzzle.py
│   ├── pentomino.py
│   ├── pinkgirl.png
│   ├── Plain_Block.png
│   ├── princess.png
│   ├── RedSelector.png
│   ├── Rock.png
│   ├── Selector.png
│   ├── simulate.py
│   ├── slidepuzzle.py
│   ├── squirrel.png
│   ├── squirrel.py
│   ├── Star.png
│   ├── starPusherLevels.txt
│   ├── starpusher.py
│   ├── star_solved.png
│   ├── star_title.png
│   ├── tetrisb.mid
│   ├── tetrisc.mid
│   ├── tetrominoforidiots.py
│   ├── tetromino.py
│   ├── Tree_Short.png
│   ├── Tree_Tall.png
│   ├── Tree_Ugly.png
│   ├── Wall_Block_Tall.png
│   ├── Wood_Block_Tall.png
│   └── wormy.py
├── Templates
└── Videos

36 directories, 212 files
pi@raspberrypi:~ $ 
```