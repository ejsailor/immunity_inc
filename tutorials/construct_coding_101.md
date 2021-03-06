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
  
##Entering Code
  Enter code by clicking 'Add Event' on an event sheet. Use the code in Level 1 as a starting point for other levels.
    
  Maps - on the mmap layouts, you only need to have individual sprites that when the guiding character (ThCell) collides with them, they take you to a layout. Have a separate layout for each battle, quiz, etc. Also, tell the computer to destroy the battle or quiz icon sprite after collisoin. Make sure you give the sprites the behavior of 'persist' so that they don't reappear when you return to the layout after completing the quiz.
    
  Battles - Battles are turn-based. Set individual global variables for each battle. You should have both a pathogen damage and host damage global variable that will be added to throughout the level. Give each player and enemy a boolean variable through the 'instance variables' in the properties panel that indicates their turn. Give each player a 'number' instance variable that corresponds to their damage dealt, as well as one that corresponds to how much they damage the host. For each turn, you will set the attack value and the host damage value for the sprite using set attack round(random(1,15)) (or any set of numbers, depending on how much damage you want the sprite to deal). Using this phrase makes the computer set these values to a random, whole number. You'll want to have text boxes set to read the pathogen and host damage 'every tick' of the computer. Use the phrase "Pathogen Damage: &pathogen.damage& " which refers to your global variable (or "Host Damage: &host.damage&"). I also included a command that tells the computer to wait until all other actions have ended before moving on to the next sprite's turn. This helped keep the game from glitching or diferent sprites' turns from overlapping.
    
  
