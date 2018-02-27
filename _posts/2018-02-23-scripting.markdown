---
layout: post
title:  "piXXelgamer Scripting Reference"
date:   2018-02-23 16:00:00 +0100
categories: manual scripting
---

The scripting language used in piXXelgamer is used for 2 purposes:

 - Automate the creation process
 - Scripting the elements in the game

The language is Pascal like and easy to learn. You don't have to use scripts at all, but with them you can
create your prototype much faster and also use some functions otherwise not available.

### Reference

**ADDLEVEL** Create's a new empty level in the project.

**ADDOBJECT** Create a new object at the current cursor position. Use *SELECTOBJECT* to choose between the available object types and catalogs.

**CENTERMODEL** Center the entire model around the the coordinate *0,0,0*. The same can be done when you press *SHIFT RETURN* in the Scene View.

**CLEAR** Clears the console window.

**DELETEALLOBJECTS** Delete all objects in the scene. Use carefully.

**EXPLODE** Let all objects in the scene explode.

**FOLLOWME** Let the camera follow the current object.

**FULLSCREEN** Switch to fullscreen mode.

**HELP** Displays the available commands.

**KEYDOWN** returns *1* if the *Down Arrow* key is pressed.

**KEYLEFT** returns *1* if the *Left Arrow* key is pressed.

**KEYRIGHT** returns *1* if the *Right Arrow* key is pressed.

**KEYUP** returns *1* if the *Up Arrow* key is pressed.

**MOVE** Move object to the absolute coordinate *x,y,z*.

**MOVEBY** Move object relative by *x,y,z* units.

**MOVEOBJECT**  Move **selected** object to the absolute coordinate *x,y,z*.

**MOVEOBJECTBY** Move **selected** object relative by *x,y,z* units.

**PRINTLICENSE** Validate and print license information to console.

**RANDOM** Get a random number.

**ROTATE** Rotate the object to the absolute angle *x,y,z* (In degrees).

**ROTATEBY** Rotate the object relative by angle *x,y,z* (In degrees).

**SELECTOBJECT** Select a object by it's id.

**SETCATALOG** Select an object *#n* from catalog ·*name*.

**SETCURSOR** Set the cursor to position *x,y,z*.

**SETCURSORBY** Set the cursor relative to position *x,y,z*.

**SETLICENSE** Save the license key.

**SETLOGSEVERITY** Set the log/console severity level.

**SETOBJECTCHAMFER** Set the chamfer radius of the **selected** object. (Must be a box)

**SETOBJECTCOLOR** Set the color of the **selected** object.

**SETOBJECTPATTERN** Set the pattern of the **selected** object.

**SETOBJECTPOSITION** Set the position of the **selected** object.

**SETOBJECTROTATE** Set the rotate of the **selected** object.

**SETOBJECTSCALE** Set the scale of the **selected** object.

**SHOWCONSOLE** Show/hide the console window.

**SPEED** Set the speed of the object.

**SPEEDBY** Set the relative speed of the object.

**SPOTLIGHT** Assign a spotlight to the object.
