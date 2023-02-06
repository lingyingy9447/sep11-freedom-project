# Entry 2: Tinkering with Kaboom
##### 12/12/2022
### Content
For the past month, I have been tinkering with [Kaboom](https://kaboomjs.com/) using the documentation and [youtube tutorials](https://youtu.be/2nucjefSr6I). I tinker with Kaboom in two ways. The first way is done during class where my partner and I will explore the components, game objects, assets, and etc for Kaboom. The second way is done at home where I will follow and code along with the tutorial I found. [Link to where I have been tinkering with](https://replit.com/@lingyingy9447/mario-kaboomjs#game.js)
 
#### 10/31/22
```js
var SPEED = 120
onKeyDown("left", () => {
   player.move(-SPEED, 0)
})
 
onKeyDown("right", () => {
   player.move(SPEED, 0)
})
```
* `onKeyDown` registers an event that runs every frame when a key is held down. They are use for movement that deals with the x-axis (left and right)
* Speed (it could be other names you want as long as you declare the variable with a certain speed) is how fast it is moving, you can assign the speed by creating the variable or just replace it with a number like `player.move(120,0)`. 0 is the y axis because you are moving along the x-axis and not the y-axis when you want to move the user move left and right.
* left = negative speed and right = positive
#### 11/7/22
```js
var SPEED = 120
onKeyDown("up", () => {
   player.move(0, -SPEED)
})
 
onKeyDown("down", () => {
   player.move(0, SPEED)
})
```
* Everything is the same as the explanation above except the sign of the speed.
* Up = negative speed and down = positive speed. It was still confusing for me because normally going up is positive and down is negative.
```js
onKeyPress("space", () => {
       if (player.isGrounded()) {
           player.jump(JUMP_FORCE)
       }
   })
```
* `onKeyPress` register an event that runs when the user presses any key or when they press the key that was assigned (`"space"` is an example of the assigned key).
* The code above means that whenever the user presses the space key, the sprite will jump if it is grounded.
 
#### 11/14/22
```js
gravity(200)
var JUMP_FORCE = 200
```
* Gravity force and jump force (or any name you assign the variable to be the force when the user jumps) functions oppositely from each other
* The smaller the gravity is, the higher the user can jump and the faster it takes the user to fall down vice versa for larger gravity.
* The larger the `Jump_Force` is the higher the user can jump

#### 11/21/22
```js
addLevel = [
   '                                    ',
   '                                    ',
   '                                    ',
   '                                    ',
   '                                    ',
   '      %   =*=%=                     ',
   '                                    ',
   '                            -+      ',
   '                   ^    ^   ()      ',
   '==============================  ====',
 ]
 
 '=': [sprite('block')],
 '$': [sprite('coin')],
 '%': [sprite('surprise)],
 '*': [sprite('surprise')],
 '}': [sprite('unboxed')],
 '(': [sprite('pipe-bottom-left')],
 ')': [sprite('pipe-bottom-right')],
 '-': [sprite('pipe-top-left')],
 '+': [sprite('pipe-top-right')],
 '^': [sprite('evil-shroom')],
 '#': [sprite('mushroom')],
}
```
* `addLevel` constructs a level based on symbols. It is basically the map of each level.
* `'symbol': [sprite('spritename')]` is the base structure that assigns a particular sprite aka character to a symbol such as `! # $ % ^ & *` . You can assign more functionality to the sprite as you increase the complexity of your game but the code basically acknowledges the fact that anytime the symbol appears it will perform the duties inside the brackets.
#### 11/28/22
```js
player.onCollide("coin", (coin) => {
   destroy(coin)
   })
```
* `destroy(name)` will make the coin disappear (or any thing associated with the name coin will disappear)
* `.onCollide` enters an event that runs when 2 game objects with certain tags collide. The code above is an example of the user or player object collides with the coin object
#### 12/5/22
```js
loadRoot ('https://i.imgur.com/')
loadSprite('coin', 'wbKxhcd.png')
loadSprite('evil-shroom', 'KPO3fR9.png')
```
* `loadRoot` sets the root for all subsequent resources urls
* `loadSprite` loads a sprite into asset manager, with name and resource url and optional config.
* Basically the first line of code tells the computer the website the images are combing from and the remaining lines of code set the name of the image and declare the id of the image.
#### [Link to what I have made so far](https://replit.com/@lingyingy9447/mario-kaboomjs#game.js)

#### Goal for winter break
My goal for winter break is to finish the youtube tutorial and try to add more complexity to the game by adding more levels to it. Additionally, if I have more time, I will look for more youtube tutorials to enhance my understanding of Kaboom Js.

### Engineering Design Process and Skills
I'm currently  on **creating a prototype** of the engineering design process (EDP). Throughout this process, I tinker with Kaboom while making my own platformer game with the help of the tutorial listed above. The next stage of EDP process for me will still be **creating a prototype** because during the next few weeks I will still be tinkering kaboom and strengthening my understanding of it by creating mini platformer games. The skills I have developed are **how to learn** and **communication**. I need learn Kaboom by myself through documentations and tutorials, so I need to develop the skill in how to learn to make my learning process more efficently. I need to know what is the best way I learn new things.  
 
 
[Previous](entry01.md) | [Next](entry03.md)
 
[Home](../README.md)
 
