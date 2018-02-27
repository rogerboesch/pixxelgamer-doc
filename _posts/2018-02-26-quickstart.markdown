---
layout: post
title:  "Quickstart"
date:   2018-02-26 16:00:00 +0100
categories: tutorial
---

#### Introduction

If you don't like read manuals and want have a quick intro to piXXelgamer then you have here the perfect start.
It shows in few easy steps how you create a level where you can test the gameplay.

### Create a level

This quickstart is not about creating a complete game. It just shows the main concept
behind piXXelgamer by creating a small, playable scene. I hope it inspire's you to try out more.
A comprehensive tutorial will follow.

#### Add the floor

![Screenshot 1]({{"/pixxelgamer-doc/images/addfloor.png"}})

In most levels you will first need a floor. A ground on where the level is playing.
You can do this by simply choose *Add floor* from the *Element* menu.  By default, the floor
is placed on Y=0. But of course you can change this in the *Object properties view* on the right.

#### Add objects

![Screenshot 1]({{"/pixxelgamer-doc/images/addobjects.png"}})

At next we place objects in the level. In piXXelgamer, several libraries with different *Themes* are available.
You can change between them, by click on the *Library name* between the two arrows. Currently, the following libraries are available:

- Primitive: 10 default primitives to use
- Voxel: 40 Voxel type block models
- Iso: Not yet implemented
- Vehicle: A plane and a boat (Much more coming)
- Character: 1 Human, 2 Monsters (Much more coming)
- Model: 1 Door model (Much more coming)

The active object you can see in the *Object preview* directly below the arrows. when you press the *SPACE* key
then this active object is placed at the cursor position in the scene.
Other important keys are:

- *Arrow left*: Move the cursor to the left
- *Arrow right*: Move the cursor to the right
- *Arrow up*: Move the cursor up
- *Arrow down*: Move the cursor down (You cant go below 0)
- *Backspace*: Delete the selected object, when you press together with *SHIFT*, then the last added object will be deleted

**Camera**
Of course you can also change the camera view and position with your Touchpad (or keys)

- Pan: To zoom in or out (You can also press *z* and *SHIFT-z*)
- Rotate: To change camera angle (You can also press *c* and *SHIFT-c*)
- Press: To change camera height (You can also press *h* and *SHIFT-h*)

Try to add something simple like seen in the Screenshot above.


#### Add player object

![Screenshot 1]({{"/pixxelgamer-doc/images/addplayer.png"}})

Now we add an object we use as a *Player object*. Choose the *Plane* from the *Vehicle* menu and add it by pressing *SPACE*.
To make something playable we will add now a small script.  
*Important: This will change later, so for the most used actions there will be a default behaviour without the need for use scripts.*

But for now select the *Events Tab* on the right side and write the following script in the *OnInit()* Script:

```
followMe();  
speed(0,0,-0.1);  
spotLight();
```

And press *Validate* to check the script. For details read chapter *Scripting*, but in easy words:
With this 3 statement we let the camera follow the object, set the speed and also add a Spotlight to the object so it looks better.

At next we need to write a sort script (Remember that is no longer needed in next version) to fly the plane by pressing the specified keys.
For this you enter the following script into the *OnUpdate()* script:

```
if (keyup() = 1) then begin
	moveby(0,-0.2,0);
end;
if (keydown() = 1) then begin
	moveby(0,0.2,0);
end;

if (keyleft() = 1) then begin
	moveby(-0.1,0,0);
	rotate(0,0,10, true);
end
else begin
	if (keyright() = 1) then begin
		moveby(0.1,0,0);
		rotate(0,0,-10, true);
	end
	else begin
		rotate(0,0,0, true);
	end;
end;
```

Press *Validate* again to check if all is correct.  
Now we can press the *Play Button* from the Toolbar to switch to *Play mode*. Be sure that the *Scene view* has the focus.
This can be easiest done by touch with the mouse in it. In the *Play mode* you will now see, that the *Plane* flies and we can change it's direction
by using the arrow keys. It's that simple :)  
That was just touching the surface of piXXelgamer, but you should now be able to start.
Much more in-depth infos and a real full-feature Tutorial is coming soon!
