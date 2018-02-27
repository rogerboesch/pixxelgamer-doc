---
layout: post
title:  "Language & Scripting Reference"
date:   2018-02-23 16:00:00 +0100
categories: manual scripting
---

The scripting language used in piXXelgamer is used for 2 purposes:

 - Automate the creation process
 - Scripting the elements in the game

The language is Pascal like and easy to learn. You don't have to use scripts at all, but with them you can
create your prototype much faster and also use some functions otherwise not available.

You can download piXXelgamer here: **https://rogerboesch.itch.io/pixxelgamer**

### Language

The language reference is coming soon. In the meantime see the Quickstart and Tutorial section.


### Reference

#### A
**ADDLEVEL** Create's a new empty level in the project.  
*Parameters: none*

**ADDOBJECT** Create a new object at the current cursor position. Use *SELECTOBJECT* to choose between the available object types and catalogs.  
*Parameters: none*

#### C
**CENTERMODEL** Center the entire model around the the coordinate *0,0,0*. The same can be done when you press *SHIFT RETURN* in the Scene View.  
*Parameters: none*

**CLEAR** Clears the console window.  
*Parameters: none*

#### D
**DELETEALLOBJECTS** Delete all objects in the scene. Use carefully.  
*Parameters: true|false* (Parameter must be true to make the call more secure.)

#### E
**EXPLODE** Let all objects in the scene explode.  
*Parameters: none*

#### F
**FOLLOWME** Let the camera follow the object. *Can only be used in object event.*   
*Parameters: none*  

**FULLSCREEN** Switch to fullscreen mode.  
*Parameters: none*

#### H
**HELP** Displays the available commands.  
*Parameters: none*

#### K
**KEYDOWN** returns *1* if the *Down Arrow* key is pressed.  
*Parameters: none*

**KEYLEFT** returns *1* if the *Left Arrow* key is pressed.  
*Parameters: none*

**KEYRIGHT** returns *1* if the *Right Arrow* key is pressed.  
*Parameters: none*

**KEYUP** returns *1* if the *Up Arrow* key is pressed.  
*Parameters: none*

#### M
**MOVE** Move object to the absolute coordinate *x,y,z*. *Can only be used in object event.*  
*Parameters: x,y,z*

**MOVEBY** Move object relative by *x,y,z* units. *Can only be used in object event.*  
*Parameters: x,y,z*

**MOVEOBJECT**  Move **selected** object to the absolute coordinate *x,y,z*.  
*Parameters: x,y,z*

**MOVEOBJECTBY** Move **selected** object relative by *x,y,z* units.  
*Parameters: x,y,z*

#### P
**PRINTLICENSE** Validate and print license information to console.  
*Parameters: none*

#### R
**RANDOM** Get a random number.  
*Parameters: n* (Maximum of random number)

**ROTATE** Rotate the object to the absolute angle *x,y,z* (In degrees). *Can only be used in object event.*  
*Parameters: x,y,z*

**ROTATEBY** Rotate the object relative by angle *x,y,z* (In degrees). *Can only be used in object event.*  
*Parameters: x,y,z*

#### S
**SELECTOBJECT** Select a object by it's id.  
*Parameters: n* (ID of an object)

**SETCATALOG** Select an object *#n* from catalog ·*name*.  
*Parameters: name,number*

**SETCURSOR** Set the cursor to position *x,y,z*.  
*Parameters: x,y,z*

**SETCURSORBY** Set the cursor relative to position *x,y,z*.  
*Parameters: x,y,z*

**SETLICENSE** Save the license key.  
*Parameters: e-mail, key* (Verify and activate the license key)

**SETLOGSEVERITY** Set the log/console severity level.  
*Parameters: 'debug'|'info'|'warning'|'error'*

**SETOBJECTCHAMFER** Set the chamfer radius of the **selected** object. (Must be a box)  
*Parameters: n* (Set the radius from 0.0 to 0.5)

**SETOBJECTCOLOR** Set the color of the **selected** object.  
*Parameters: color* (Color in hex format. Ex. '#FF0000')

**SETOBJECTPATTERN** Set the pattern of the **selected** object.  
*Parameters: n* (Set the pattern to 1-n)

**SETOBJECTPOSITION** Set the position of the **selected** object.  
*Parameters: x,y,z*

**SETOBJECTROTATE** Set the rotate of the **selected** object.  
*Parameters: x,y,z*

**SETOBJECTSCALE** Set the scale of the **selected** object.  
*Parameters: x,y,z*

**SHOWCONSOLE** Show/hide the console window.  
*Parameters: true|false*

**SPEED** Set the speed of the object. *Can only be used in object event.*  
*Parameters: x,y,z*

**SPEEDBY** Set the relative speed of the object. *Can only be used in object event.*  
*Parameters: x,y,z*

**SPOTLIGHT** Assign a spotlight to the object. *Can only be used in object event.*  
*Parameters: none*
