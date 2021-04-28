##General information:
  NAME EVERYTHING - this will make your life SO much easier when you have 20+ layouts with different textboxes, sprites, etc.
  Code in small chunks, it's much easier to de-bug in small bits rather than in one large go.
  You can copy and paste code, so once you get something working you just have to paste it to other layouts or other characters.

##Panels:
   Main Panel - this panel is in the middle. This is where you will do most of your work. Here, you will see the event sheet or layout that you have open. You can see which tabs you have open at the top of this panel. 
   Project Panel - this panel is on the upper right-hand side. This is where you can see everything you have for the project; layouts, event sheets, sprites, text, backgrounds, etc. I haven't used the families or timelines features, but this is where that information would also be held. 
   Properties Panel - This is where you will see the properties for the item you have selected. This is where you will change behaviors and instance variables for sprites. You can change font size, color, and style in this panel when text is selected. If you don't have anything selected, this panel will show you the properties of your layout or project as a whole. 
   
##Layouts vs. Event Sheets:
  Layouts are the User Interface of the game. This is where you will place text, shapes, backgrounds, sprites, etc. that you want the player to see. EVERYTHING that you've placed in the layout will show up here, even if you have it coded to show up only at certain times. For example, in the battles I have several different text boxes overlapping on the layout because I want them to show up in the same place, but I have them coded to show up only at certain times. The dotted line on the layout shows what shows up in one screen. 
  Event sheets are where you will do your coding. You will essentially set up If/then statements by clicking 'Add event'. You will select which object you want to refer to, and what situation you want it to be in when the next events occur. For example: 'If Macrophage collides with Bacterium'. You will then choose your 'then' statements, what you want to happen when your 'If' statement occurs. For example: 'Subtract 5 from bacterium health'. Your whole statement would be 'If macrophage collides with bacterium, then subtract 5 from bacterium health.'
   

##Getting Started:
  Open a cloud file (or open a new file) in Construct 3 using the Immunity Inc Gmail.
  After opening the file, log in to Construct 3 using the Immunity Inc log in information.
  Right click the 'Layouts' folder in the Project panel. Add  a new layout WITH and event sheet. Name the layout.

##Adding a background:
  Right click and 'Insert New Object'. Choose tiled background. 
  Drag your image of choice into the blank space, or use the file upload button in the top left-hand corner. 
  As is, your background likely isn't the right size for your layout and will show up as tiled repeats of your image. To remedy this, open the Tiled Background Editor and use the resize button or ALT + R. I haven't found a good way to figure out what size will be right, mostly just trial and error with different values.
  
##Adding a sprite:
  Right click on your layout and click 'Insert New Object'. Choose 'Sprite'.
  Put your image of choice or draw your sprite in the Animations Editor.
  If you would like to make this sprite animated, you can do this by adding frames in the bottom animation panel. To add a frame, right click on frame 0 and duplicate the frame. Now, make any changes you would like to this image to make the animation. Animations will automatically run continuously if you don't specify when to start and stop or what frame you'd like to show in the event sheet for each layout that the sprite is present in.
  Remember to name your sprite!
  