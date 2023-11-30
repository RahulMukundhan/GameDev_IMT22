                                                      "Sands of Time"
Track 2: Quest for the lost artifact 

Motivation: Retrieve the "Artifact" in a pyramid, lost in the desert

Codes:
      Player movement: It allows the player to move (WASD) and space for jump, along with mouse for camera control
      
      Open Chest : Chest user interaction, and gives artifact when opened.
      
Game objects:

      "Player movement" is attached to player prefab

      
Packages:
        TextMeshPro-> TextMeshPro (also known as TMP) uses Advanced Text Rendering techniques along with a set of custom shaders,delivering substantial visual quality improvements while giving users incredible flexibility when it comes to text styling and texturing.
                (https://docs.unity3d.com/Packages/com.unity.textmeshpro@3.0/manual/index.html)

Run and Install:
             open "Asset creation.exe" ,
              
              Click host(server+client) and the game starts


Details:
        for the code structure, inside the player movement code, there are different values/ variables for speed, gravity,and so on. There is also a isGrounded variable which tells whether the player is on the terrain/ground or not.
        
        the onEnable class-> called when the game starts <acts as a master control for all the movements>
        
        for the end of the game, we use the onDisable class
        
        the start class-> assign the player as a variable, which can be controlled. The mouse is locked here to avoid issues.
        
        update -> class which is called on everyframe. It takes inputs, and performs necessary actions (like change player velocity in different directions), move, jump, etc.
        
        jump class -> allows the player to jump, when the space bar is pressed, and on the terrain <no double jumps>
