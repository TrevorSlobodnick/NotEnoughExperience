## Description

This is a simple mod that adds a multiplier to the xp that is dropped by mobs and mined ores.

## Commands

`nexp` - use this command to display the current multipliers while in game

## Config Options

**Debug Mode**

The only reason to have debug mode enabled is if you want to make sure the xp multipliers are working correctly.
When enabled, Every time you kill a mob or mine an ore that drops xp,
it will send a message in the chat displaying the following information:

- the current multiplier being applied
- the xp that would have been dropped in vanilla minecraft 
- the xp that was actually dropped
- the players xp before adding the dropped xp

**Ore Multiplier**

- Minimum Value: 0.1
- Maximum Value: 100.0
- Default Value: 1.0

The multiplier for the xp dropped when mining ore. 
Any number above 1 will increase the amount of xp dropped,
and any number below 1 will decrease the amount of xp dropped.

**Mob Multiplier**

- Minimum Value: 0.1
- Maximum Value: 100.0
- Default Value: 1.0

The multiplier for the xp dropped when killing mobs.
Any number above 1 will increase the amount of xp dropped,
and any number below 1 will decrease the amount of xp dropped.

**Changing Config Values (File)**

If you *don't* have access to the client, you will need to edit the config file directly.
It is fairly straightforward, just look for the file named **notenoughxp-common.toml** in your config directory.
Once you open it there will be 3 things you can change:

- `debug`
- `ore_multiplier`
- `mob_multiplier`

To update these values, just change the value after the "**=**"

`debug` can be set to either **true** or **false**.
(**Ex.** debug = false)

`ore_multipler` can be set to **any number between 0.1 and 100.0**.
(**Ex.** ore_multipler = 4.3)

`mob_multipler` can be set to **any number between 0.1 and 100.0**.
(**Ex.** mob_multipler = 10.0)

**Changing Config Values (GUI)**

If you *do* have access to the client, You can edit the options in the mod config screen, otherwise known as a GUI.
To access this screen/GUI: 

1. In the main menu, underneath the Singleplayer and Multiplayer buttons, there is a button titled **Mods**, click on it
2. This should bring up a list of all your installed mods. Find **Not Enough XP** and click on it
3. On the bottom left of the screen, the **Config** button should be lit up, click on it
4. This will launch the config screen, where you can easily change your settings.

## Changelog (Forge)

##### Version 1.1.1 - November 27, 2022

- In the config gui (Mods &gt; Not Enough XP &gt; Config), the Debug value used to be displayed as "True" or "False", now it is displayed as "ON" or "OFF"

##### Version 1.1.0 - April 25, 2022

- Fixed issue where mod would crash if ran on dedicated server
- Added "nexp" command, which can be used to quickly check your xp multipliers while in game

##### Version 1.0.0 - September 3, 2021

- Initial Release

## Changelog (Fabric)

##### Version 1.0.0 - December 29, 2022

- Initial Release 
