# CS2's Render Settings Config
This render_settings.cfg file lets you tweak the main render settings of CS2 through console with a GUI.

# WARNING
- If you don't understand what this config does, you probably shouldn't use it !
- The settings used in that file will only apply on the Workshop Tool Build of CS2 atm.
- It is currently impossible to use aliases through the console on that specific build, so you will have to bind the commands listed on the interface, or ask valve to fix that issue.
- By default, ENTER will be bound to display the GUI, and BACKSPACE will reset the vars to their default values. 

# Installation
1. Open the archive and extract its content into the following path folder : 
"...\Steam\steamapps\common\Counter-Strike Global Offensive\game\csgo\cfg\"

2. Launch the game (Workshop Tool Build), boot up a practice server where you can turn on sv_cheats 1 and type in the console the following command: "exec render_settings.cfg".

3. Your console should display the GUI and a sound will be played in-game; otherwise you must have a path issue and the file did not load correctly.

# Usage
- A set of bindings using kp_keys is commented, feel free to remove the "//" in that specific section.
 
- A self explanatory documentation will be displayed into the GUI in your console under this format :
VARS (STATUS) | ToggleCmd / ToggleOnCmd / ToggleOffCmd

For example :
- Toggle Viewmodel Rendering ON and OFF by simply typing "render_drawviewmodel" in your console.
- Toggle Viewmodel Rendering ON by simply typing "render_viewmodel_on" in your console.
- Toggle Viewmodel Rendering OFF by simply typing "render_viewmodel_off" in your console

The GUI stores the current values in memory for the toggle command, so if you turn off viewmodel with "render_viewmodel_off", it takes only one usage of "render_drawviewmodel" to bring it back on.

- Type helprender or renderhelp to display the GUI in order to see the current status of the vars.
- Type render_reset to reset the GUI to its default setup.


- If you change map, the GUI will not remember previous changes, so you will need to "exec render_settings.cfg" since the render convars will not be updated.
- The GUI will not keep in memory any var that is changed manually in the console.
