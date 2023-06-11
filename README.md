# EXP-05---AMMO-COLLECTION
## AIM:
To create ammo to increase the bullet count and increase the bullet spawn count.

## ALGORITHM:
For Adding Bullet Count:
### STEP 1: Create a HUD Blueprint:
i)In the Content Browser, right-click in the desired folder.
ii)Select Create Basic Asset > Blueprint Class.
iii)In the Class Settings window, search for "HUD" and select it as the parent class. Name the Blueprint (e.g., "GameHUD") and click Create.
### STEP 2: Open the GameHUD Blueprint:
i)Open the GameHUD Blueprint you just created.
ii)In the Blueprint editor, find the Canvas panel on the left.
iii)Add a Text block widget to the Canvas panel to display the bullet count.
iv)Position the Text block widget on the canvas as desired.
### STEP 3: Create a reference to the player character:
i)In the GameHUD Blueprint, create a variable of the player character's class to store a reference to it.
ii)To do this, go to the Variables panel and click the "+" button.
iii)Set the variable type to the class of your player character (e.g., ThirdPersonCharacter).
iv)Name the variable (e.g., PlayerCharacter).
### STEP 4: Update the bullet count display:
i)In the GameHUD Blueprint, locate the Event Tick event.
ii)Drag off the PlayerCharacter variable and search for "Get Bullet Count" (assuming you have a bullet count variable in your player character Blueprint). Connect the output of the Get Bullet Count node to the Text block widget's Text property.
iii)You may need to format the bullet count value as a string before connecting it to the Text property.
### STEP 5: Set the GameHUD as the active HUD:
Open your player character Blueprint.
i)In the Blueprint editor, locate the Event Begin Play event.
ii)Drag off the execution line and search for "Create Widget".
iii)In the Create Widget node, select the GameHUD Blueprint you created.
iv)Drag off the return value of the Create Widget node and search for "Add To Viewport".
v)Compile and save the player character Blueprint.
### STEP 6: Test the bullet count display:
i)Play the game in the editor.
ii)Ensure that the bullet count is displayed on the screen as you interact with the game, such as firing bullets or picking up ammo.
## Output
### Before Collection

![g2](https://github.com/Shobika187/EXP-05---AMMO-COLLECTION/assets/94508142/38f82ede-64ee-471a-8ae3-f9ae87f0b77a)

### After Collection
![g3](https://github.com/Shobika187/EXP-05---AMMO-COLLECTION/assets/94508142/8b85a3b4-1433-470a-908f-dbd096760bc7)

### Canvas
![image](https://github.com/Shobika187/EXP-05---AMMO-COLLECTION/assets/94508142/f48da627-f2a4-48f4-ad79-8df959fa7f52)

### Bullect COunt Graph
![image](https://github.com/Shobika187/EXP-05---AMMO-COLLECTION/assets/94508142/e2bd8e43-6bc0-4bb8-bf0f-5183359434cb)
## ALGORITHM:
## For Adding Ammo:
### STEP 1: Create an ammo actor:
i)In the Content Browser, right-click in the desired folder.
ii)Select Create Basic Asset > Blueprint Class.
iii)In the Class Settings window, search for "Actor" and select it as the parent class. Name the Blueprint (e.g., "AmmoActor") and click Create
### STEP 2: Set up the ammo actor:
i)Open the player's character Blueprint.
ii)In the Blueprint editor, locate the event that handles the collision or overlaps with the ammo actor.
iii)Add a new custom event node to handle the interaction.
iv)Implement logic to increase the bullet count for the player:
v)Access the player's character or controller reference.
vi)Increment the bullet count variable or property. Play a sound or visual effect to indicate the pickup.
vii)Destroy the ammo actor after it has been collected.
### STEP 3: Implement the player's interaction with the ammo actor:
i)In the GameHUD Blueprint, create a variable of the player character's class to store a reference to it.
ii)To do this, go to the Variables panel and click the "+" button.
iii)Set the variable type to the class of your player character (e.g., ThirdPersonCharacter).
iv)Name the variable (e.g., PlayerCharacter).
### STEP 4: Place the ammo actor in the level:
i)Drag and drop the AmmoActor Blueprint into the level where the player can interact with it.
ii)Adjust its position and orientation as n
### STEP 5: Test the ammo pickup functionality:
i)Compile and save the AmmoActor Blueprint and the player's character Blueprint. Play the game and navigate the player character to the ammo actor.
ii)Ensure that when the player character overlaps or collides with the ammo actor, the bullet count increases, and the ammo actor disappears
## OUTPUT
### EVENT GRAPH
![image](https://github.com/Shobika187/EXP-05---AMMO-COLLECTION/assets/94508142/d410cf69-e165-4a74-b4d0-6e040e2f42ab)
### Increase Bullet Count in Ammo Actor:
![image](https://github.com/Shobika187/EXP-05---AMMO-COLLECTION/assets/94508142/df8fd00e-4f0b-4fad-8364-27cc26919d0a)
## RESULT:
Thus, added ammo to increase the bullet count and displayed it in play-mode


