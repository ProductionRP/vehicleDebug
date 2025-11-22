## Description
This is a utility for FiveM that allows the live editing of vehicle handling and some basic performance statistic tracking for top speed, acceleration, and deceleration.

## Installation and Use
- Download the GitHub repository code.
- Add to the `resources` folder.
- Ensure `vehicleDebug` in the server.cfg, or `ensure vehicleDebug` in <kbd>F8</kbd>.
- Press <kbd>Right Alt</kbd> to open the handling editor while in a vehicle (configurable in `cl_config.lua`).
- Use the command `vehdebug` to toggle the debugger on/off if needed.
- Enjoy!

**Note:** The `vehdebug` command is unrestricted by default. If you're running this in a live environment, you may want to modify the command registration in `cl_debugger.lua` (line 264) to change `false` to `true` to restrict it to ACE permitted individuals only or modify the code how you see fit for you. You can also set `EnabledByDefault = false` in `cl_config.lua` to have the debugger disabled by default.

## Editor
Press Right Alt (default) while in a vehicle to bring up the menu. You can change the keybind in `cl_config.lua` - see the [FiveM keybind reference](https://docs.fivem.net/docs/game-references/input-mapper-parameter-ids/keyboard/) for available key names. Click the input boxes for whichever value you would like to modify, and change it. That's it! The handling will immediately update as you type. Hover over the fields for a little more information on what that particular field does.

You can save the handling by clicking "Copy Handling" near the top. You will need to paste that over the handling file for the vehicle. Make sure you're replacing everything from **mass** to **monetary value**, nothing more, and nothing less.

![LiveHandling1](https://user-images.githubusercontent.com/8594390/113525001-6b17b380-9580-11eb-8411-5a7076a4514e.png)

## Statistics
In the top-middle of the screen, there are numbers to represent some "tops" for the vehicle. Falling or crashing will lead to irrelevant values. Reset the values within the editor by clicking "Reset Stats."
* Top speed - The fastest speed, in miles per hour, that the vehicle has reached.
* Top acceleration - An arbitrary value to represent how quickly the vehicle has accelerated.
* Top deceleration - An arbitrary value to represent how quickly the vehicle has decelerated.

![LiveHandling2](https://user-images.githubusercontent.com/8594390/113525004-6e12a400-9580-11eb-8ad2-a5fd70aef41d.png)

---

### 🎮 Join ProductionRP - An Allowlisted FiveM Roleplay Server
Experience high-quality roleplay at **[ProductionRP.org](https://ProductionRP.org)**

![ProductionRP](https://i.gyazo.com/947c5cdb1dbb9d47322262745d85f864.gif)

---

## Credits
Thanks to the post by V4D3R on 5Mods for describing the handling fields a little more:

https://forums.gta5-mods.com/topic/3842/tutorial-handling-meta
