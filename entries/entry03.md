# Entry 3 Tinkering with Kaboom 
##### 2/6/23
### Content 
For the past few weeks, I have been tinkering with [Kaboom](https://kaboomjs.com/) using the documentation. I finished the [youtube tutorials](https://youtu.be/2nucjefSr6I) during the winter break as one of my goals. I started to add more levels to the Mario game that I was working on and learned more game objects, assests, components, and events. 
#### 1/9/23
* Spend my time on building the third level on [replit](https://replit.com/@lingyingy9447/mario-kaboomjs#game.js) 
#### 1/16/23
<img width="559" alt="Screenshot_20230207_064753" src="https://user-images.githubusercontent.com/91750525/217393074-57eb0292-f46b-49cd-8e66-8169399a3247.png">

* `camPos(player.pos)` is use so that the camera will follow the player 
* `go()` goes to a scene and ignores/passes other scenes.
*  Basically the code above means that the camera will follow the player to the lost scene if the player falls below the y limit. 


#### 1/23/23
<img width="289" alt="Screenshot_20230207_090559" src="https://user-images.githubusercontent.com/91750525/217410397-42600e7f-fea0-4e94-b727-2f34d0fc609e.png">

* `action()`  define what the assign sprite will do 
*  `m.move(-30,0)` moves the mushroom to the left at a speed of 30 . If it is (30,0) it will move the mushroom to the right at a speed of 30  

#### 1/30/23
* `pos(#,#)` The first number is for the x-axis, the greater the number is the more it goes to the right. The second number is the y-axis, the greater it is the downward it goes

<img width="346" alt="Screenshot_20230207_093208" src="https://user-images.githubusercontent.com/91750525/217413858-12f29aaa-b37d-488d-9cef-0efeefc1b94e.png">

* `gameLevel.spawn` or `_.spawn` will make the assigned sprite appear 
* The first one was (0,1) because the coin need to be above the unboxed sprite. (0,1) gives the coin a position of y that is one increment higher than the surprise sprite 
* Second one is (0,0) because unboxed sprite replaced surprise sprite in the same position

#### 2/2/23
<img width="307" alt="Screenshot_20230208_095954" src="https://user-images.githubusercontent.com/91750525/217706919-fd7a5cd1-35af-4cb3-9453-29b06abcfdcb.png">

<img width="480" alt="Screenshot_20230208_100048" src="https://user-images.githubusercontent.com/91750525/217706929-64563210-1823-4d8f-a81c-c773ab7865e7.png">

* scene () - define a scene 
* Example above will go to the scene lost and display the score in the position stated if the player did not destroy the enemy by jumping 

#### What I plan on learning next about my tool 
I personally think that I learn basically everything needed to create a platformer game for my freedom project. Therefore, my next step would be creating a mini platformer game that will use the concepts I learned from the past few months of tinkering with Kaboom. I also plan on learning about `loadSound` which can be used to incorprate game sounds into the game

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
