# HF Breakout
> Play, Design, and Share Breakout Levels

<p align='center'>
  <a href="https://xadamxk.github.io/hf-breakout/">Click Here to Play</a>
</p>

Starting as a basic tutorial for programming games, [Jake Gordon](https://github.com/jakesgordon) created this game to teach about game physics and utilizing HTML5 canvas to build fun and creative games. I've built on his work by adding a custom level generator, game powerups, additional levels, level names, online user counter, and more.

<p align='center'>
  <img src='https://github.com/xadamxk/hf-breakout/blob/master/Promo/levels.gif?raw=true' alt='HF Breakout'></img>
</p>

## Level Generator

<p align='center'>
  <a href="https://codepen.io/xadamxk/pen/XoyPbq">Click here to access the editor</a>
  
  <details> 
  <summary>Screenshot</summary>
  <img src='https://github.com/xadamxk/hf-breakout/blob/master/Promo/editor_demo.gif?raw=true' alt='Level Generator'></img>
</details>
</p>

The level generator allows anyone to draw pixel art to create custom breakout levels. The code for this editor was inspired by [gelstudios/gitfiti](https://github.com/gelstudios/gitfiti), which allows users to create pixel art in their Github contribution history. To create levels, simply open the codepen project and get to drawing. When you are happy with your creation, don't forget to name your level, copy the contents of the Code and head on over to the breakout game. Click upload, paste the level code in the prompt window, and enjoy playing your level.

To add your level to the publicly available game, please submit levels via the release thread, Github issue/pull request, or contact me privately.


## Powerups
`Powers have a 1 in 40 (2.5%) drop rate upon destroying blocks`

* Big Paddle
    * Makes your paddle 2x longer
* Small Paddle
    * Shrinks your paddle in half
* Extra Life
    * `You probably guessed it.` Gives an extra life
* Fireball
    * Turns the ball into molten lava, melting every brick in its path
* Multiball `(Work in Progress)`
    * Multiplies your ball into 3 smaller balls
* Sticky Paddle `(Work in Progress)`
    * Catches the ball on each paddle hit
    
It was my intention to have powerups drop from blocks when destroyed, but after attempting this I broke the game physics. I've reverted this feature but do plan on implementing it in the future.

## Release History
* 0.3.1 - 1/21/2019
    * Added users online script to show many users are currently playing
    * Bugfix: Now encode generated levels in base64 to prevent whitespace errors caused by `window.prompt()`
* 0.3.0 - 1/20/2019
    * Added level upload functionality to game
    * Added name field to level generator
    * Changed how levels were parsed when generated via editor to be compatible with upload feature
* 0.2.2 - 1/19/2019
    * Added 2 new powerups (Fireball & Small Paddle)
    * Powerups now stack rather than override eachother
    * Bugfix: Fixed error caused by using white as an eraser in the editor
* 0.2.1 - 1/17/2019
    * Bugfix: Powerups now reset on ball loss and level completion
    * Bugfix: Balls no longer mysterically slide through the paddle's edge when against walls
    * Bugfix: Added more community made levels - now 17 total
* 0.2.0 - 1/15/2019
    * Implemented powerups (Big Paddle & Extra Life)
* 0.1.1 - 1/13/2019
    * Bugfix: Fixed level index glitch on page refresh
    * Bugfix: Now gives a life rather than taking one on level completion
* 0.1.0 - 1/12/2019
    * Added custom levels
    * Implemented level names
* 0.0.1 - 1/12/2019
    * Initial Release

## Meta

This project wouldn't be possible without the following people:

[Gel Studios](https://github.com/gelstudios): [Gitfiti Project](https://github.com/gelstudios/gitfiti)

[Jake Gordon](https://github.com/jakesgordon): [Breakout Project](https://github.com/jakesgordon/javascript-breakout)

The HF community for submitting levels, bug reports, and general game suggestions.
