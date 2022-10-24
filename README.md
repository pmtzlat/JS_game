##Description##

This game is a sidescroller where you’re an X-wing pilot fighting tie fighters. The aim is to
achieve the highest score possible or last the longest until you die.
The arrow keys are used to move the X-wing on all directions, and the spacebar is used to shoot
lasers.
At the beginning of the game a few tie fighters will appear, but as the score gets higher, more tie
fighters appear, and they move faster.
There is a main menu and a game over screen, where your score is displayed.
______________________________________________________________________________________________________________

##Issues##

First of all, getting the basic skeleton for the game was hard, as the movement and rendering of
the objects was hard to get used to. I had to get used to the canvas, and the mechanics of
updating everything using intervals.
Once the basic game was created, player movement was implemented. At first, the ‘keypress’
event was used to handle input, but it wasn’t optimal as multiple keypresses couldn’t be handled
by the program. So the controller array was created, and using ‘keydown’ and ‘keyup’ events
was far more successful and provided smoother player controls.
The generation of enemies was also a problem, as they needed to be generated and destroyed.
The spawn rate and the direction/movement of them had to be tweaked constantly through the
development process to make the game fun and progressively harder.
Then, the shots were implemented. Enemy shots were created first and getting them to
randomize who shoots was hard to do. Then the player shots were created using arrays, which
made their rendering and movement easier than expected. The main issue was input handling, as
whenever the player held the spacebar down, the laser went full auto. To handle this, the
controller was tweaked so that once the laser was shot once, the player had to lift their finger
from the spacebar to fire again.
The hardest part by far was handling collisions and what happened afterwards. Getting the shots
to register took a long while of trial and error where some shots wouldn’t register, or others
wouldn’t disappear after a collision. After getting collisions to register properly, getting enemies
to change to explosions and disappear took a while, as sometimes explosions wouldn’t want to
disappear.
At the end of the development, music was added, as well as the background stars and the menus
