# Entry 5
##### 4/21/23

### Context 
The past month my partner and I worked toward finishing our MVP plan for the [project](https://chanryc9471.github.io/sep11-freedom-project-kaboom/). Before I began to explain our process, I want to inform the ones reading this blog that we changed our main sprite and enemy sprite. 

##### Main Sprite
![char](https://user-images.githubusercontent.com/91750525/233732573-9f4f5e0a-d448-49b4-ae58-b5ca906f4dea.png)

##### Enemy Sprite
![toto (2)](https://user-images.githubusercontent.com/91750525/233731654-19e01b52-81c0-483f-b3d0-a15ac2c8a52a.png)

#### First Step: Building our scene 
We first created a folder for our sprites in our repo and began setting up our kaboom. link The code was just the basic setup for kaboom to function. We make the game to take up the full screen size, give it a background color, and etc. 

![image](https://user-images.githubusercontent.com/91750525/233733221-a1bab8b3-356f-4aeb-b27d-3950ca9fe534.png)


Then we start to load the sprite into the asset manager with their name and resource url so that we can later apply those sprites in our game. `loadSprite('name','image link or pathway to the image')`

![image](https://user-images.githubusercontent.com/91750525/233734034-dad14282-35bd-45ff-9e56-9b8cc1922099.png)

Afterward we gave each sprite their assigned symbol which we can later apply in our scene map. We made each sprite to have a width of 45 and height of 50. 

![image](https://user-images.githubusercontent.com/91750525/233734752-3757b950-d186-462d-b192-298645a822c4.png)

We then make our game map in which we put symbols inside of it so that the sprite that was given that symbol will show up on the screen. 

![image](https://user-images.githubusercontent.com/91750525/233735086-f7e10fb6-0746-4905-a4e1-18a69048060e.png)

At first our sprite was overlapping with each other because the pixel size was either too big or too small and there was also empty space around the sprite making the sprite look like it was flowing in the air. Therefore, we search up [image resizer](https://imageresizer.com/) to resize the image and crop the empty white spots

![image](https://user-images.githubusercontent.com/91750525/233736160-fce0799b-a2d4-4470-8bbf-86d92e4efa5a.png)

#### Second Step: Making the main sprite move 
First we add the main sprite to the page by giving it a position. We gave it a value of `body()` so that it will respond to gravity, allowing it to jump and move around. 

 ![image](https://user-images.githubusercontent.com/91750525/233737540-f9831c77-9cfe-498e-be6c-cd2b378088a2.png)
 
 Afterwards we give the main sprite the ability to move left and right and jump using event components such as `keyDown`. The first event will allow the user to move left by a given speed that was declared previously when the left arrow was pressed down. The following events are basically the same concept but with different movements. 
 
 ![image](https://user-images.githubusercontent.com/91750525/233737739-7353af0d-b558-4a9a-8f71-cb73a6b2c4db.png)
 
 #### Third Step: Keeping track of score and level 
 We make a text that appear on the scene to keey track of how many coins the user collects and what level the user is on. The first set of code tells you the score of the user and placing it at a position of (0,300). The second one adds the text level + : current level the user is on (in number) at a position of 20, 300 so that the score and level will be on the same line but have space between them. 
 
 ![image](https://user-images.githubusercontent.com/91750525/233741714-5060602f-d76c-404b-9598-122311021464.png)
 
 The player will increase their sore if they collide with the collides. The coin will disappear and the score will increase by one. The `scoreLabel.value` which contain the current score of the user will be increase by one and set it into `scoreLabel.text` which is the text that will appear on the screen. 
 
 ![image](https://user-images.githubusercontent.com/91750525/233742134-d47acef2-0963-48ce-8f57-22f9f2a10308.png)


 #### Fourth Step: New levels and death 
 We added more levels to the game by making the game map into an array inside of an array. 
 
 ![image](https://user-images.githubusercontent.com/91750525/233738666-6b5b10c6-1ccb-466b-8451-41e3d5ee814c.png)

 
 Then we start to loop the level. We learn that since we used start to declare the game we can pass in the starting value of level which is zero. Then we created an event in which when the player collides with the door it will go to the next game level and take their current score with them. The event will add one to the game level value making it increase every time it collides with the door. 
 
 ![image](https://user-images.githubusercontent.com/91750525/233739249-8d32f368-51c7-4fa3-8406-caa71ffc5e7b.png)

![image](https://user-images.githubusercontent.com/91750525/233739348-f1376bab-7ddb-4d7d-a69b-4e07bdc36cba.png)


We made two ways for the user to lose the game. The user will go the lose scene either by colliding with the enemy or fall between the gaps of the block. We set a death value of 800. So if the y position for the player exceeds 800, the player will go to the lose scene. Additionally we add a `camPos` so that the screen will follw where the player is. For our next step, we will be learning how to allow the user to kill the enemy for our beyhond MVP plan. 

![image](https://user-images.githubusercontent.com/91750525/233741012-b0f4290d-951b-4443-8fc0-5069570fd403.png)

![image](https://user-images.githubusercontent.com/91750525/233741056-fd395759-644e-447b-b8dc-14da04687117.png)


 







### Engineering Design Process and Skills 

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)

