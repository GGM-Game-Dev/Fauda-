## Fauda
We Implemented basic First Person Shooter mechanics without animations.
We have the ability to move, look and fire object include detection and activate a function at the object that got hit.
# Player Controller
Will control the player using a player controller component and inputs of WASD keys and mouse.
We added the ability to jump by adding velocity to our player.
Movement and gravity script:

![image](https://user-images.githubusercontent.com/88790441/234091589-0d075a08-b580-465a-a58f-2531db68e812.png)

 
Player look script:
![image](https://user-images.githubusercontent.com/88790441/234091615-8a09d16c-be32-4602-8247-9401b12d4307.png)

 
# The Gun
We used Raycasthit class and calculated if we hit something when we shoot.
We raycast from our FPS camera position in the forward direction.
If we hit an Enemy – we will activate his takeDamage function.
We also will Instantiate Impact effect on the hit position and muzzle flash at the gun barrel.

![image](https://user-images.githubusercontent.com/88790441/234091658-d820cdfa-73ec-4add-9926-6969cd987d3b.png)

 
# Enemy
Each enemy have health and public takeDamage() function that will be called when we hit him with the gun shoot, the function will decrease his health.
When health is less then 0 – we will destroy the enemy object by calling Die() function.

![image](https://user-images.githubusercontent.com/88790441/234091686-7d1ed2ec-9e0a-4be9-ae6b-926fbe3cc475.png)

 
