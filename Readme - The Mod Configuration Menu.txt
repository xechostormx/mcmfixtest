Name: The Mod Configuration Menu
Link: http://newvegas.nexusmods.com/mods/42507/
Author: Pelinor
Version: 1.5
Created: 06/22/2011
Modified: 05/29/2012

===============
Description:
===============

Allows any number of mods to be configured from a single menu.

===============
Details:
===============

The Mod Configuration Menu (MCM) is a resource for other mods to use which adds a "Mod Configuration" button to the Pause menu.
When you click on it, a window appears with a list of all of the mods using MCM. Each of these listed mods are then configured from within the same menu.

As can be seen in the screenshots, a very user-friendly menu allows you to quickly and confidently configure your mods. You won't have to use any items or press any special keys to use it.

For modders wanting to use MCM menus for their mods, a detailed guide is given explaining how.
Menus made for MCM only require MCM to be installed and activated; there is no master dependency to the system, so your mod will still work if the user doesn't have MCM installed.

(Note: MCM is not to be redistributed. Provide a link to the MCM mod page if your mod requires it.)


===============
Requirements:
===============

Fallout New Vegas
New Vegas Script Extender (NVSE) 2.0 beta 12 or higher from: http://nvse.silverlock.org/
Microsoft Visual C++ 2010 Redistributable Package (x86) for the plugin from: http://www.microsoft.com/en-us/download/details.aspx?id=5555
Fallout Mod Manager (FOMM) for the installer from: http://newvegas.nexusmods.com/mods/36901
-OR-
Nexus Mod Manager (NMM) for the installer from: http://newvegas.nexusmods.com/mods/modmanager/

===============
Installation:
===============

The preferred installation method is:
1. Extract The Mod Configuration Menu.FOMOD from the archive.
2. Launch FOMM
3. Select "Package Manager"
4. Select "Add FOMOD" and open to The Mod Configuration Menu.FOMOD
5. Highlight The Mod Configuration Menu and click "Activate"
6. Overwrite any existing files.

The alternative installation method is:
1. Extract the contents of "The Mod Configuration Menu.FOMOD" to \Fallout New Vegas\Data\
2. Include The Mod Configuration Menu in your mod list via the FNVLauncher's Data Files or with FOMM/NVMM.
3a. Use Unified HUD Project 2.6 or higher, or:
3b. Open Data\menus\options\start_menu.xml
3c. At the bottom, find </menu> and place <include src="includes_StartMenu.xml"/> before it . As so:
		<include src="includes_StartMenu.xml"/>
	</menu>

===============
Un-Installation:
===============

If you used the FOMM installation method:
1. Launch FOMM
2. Click "Package Manager"
3. Highlight The Mod Configuration Menu and click "Deactivate"

If you used the manual installation method:
1. Remove the edit to start_menu.xml
2. Delete the files included in the archive.

===============
F.A.Q.:
===============

Q. How do I use MCM?
A. Pause the game and select "Mod Configuration" to configure your mods. You must also have MCM-compatible mods installed.

Q. Does MCM work with DarNified UI?
A. Yes, they work very well together. (If DarNified UI is installed after MCM, you will need to either reinstall MCM or use Unified HUD Project.)

Q. MCM tells me to remove redundant menu entries. How do I do this?
A. You need to remove any duplicate <include src="MCM\MCM.xml"/> lines. There can be only one in either Data\menus\options\start_menu.xml or Data\menus\prefabs\includes_StartMenu.xml

Q. Will MCM be made for Fallout 3?
A. Probably not. FOSE doesn't have the capabilities of NVSE that make MCM possible.

Q. Why do none of my other MCM mods show up, even though I have Project Nevada installed with integrated MCM?
A. You need to use the stand-alone MCM. The integrated Project Nevada version only works for that mod.

Q. What do I do when my menu look weird after I updated Project Nevada to version 2.3?
A. Update your MCM to the official version 1.2 or higher.

===============
Compatibility:
===============

There should be no compatibility issues, and none are known so far.
Mods using MCM do not need to make it a master to use the menu, although MCM does need to be present and active in the user's mod list.

===============
Support:
===============
Please use the official MCM support thread at http://www.thenexusforums.com/index.php?showtopic=401942

===============
History:
===============

1.10 - Allow multiple menus per mod; fix freezing issues; fixed list width calculation
1.20 - Implementated controller navigation; faster start menu opening; improved visuals; improved scale interaction; added multiple scale options; added more debug information for users; packaged as FOMOD (thanks to schlangster)
1.30 - Implemented wrapping mod list names if too long; fixed sub-menu bug when at bottom of list; fixed mouse wheel scrolling issues; updated installer
1.40 - Corrected main plugin version; added NVSE plugin with new Get/Set INI functions; fixed mod list bug after GameMode; fixed missing menu on new game; added INI setting to control MCM tutorial messages
1.41 - Removed NVSE warning
1.50 - Restructured scripts; added Get/SetMCMFloat, SetMCMString, SetMCMFloatMass, SetMCMStringMass, SetMCMModList, GetMCMListWidth to NVSE plugin; improved gamepad navigation; improved mod list behavior; added max mod list width option; added version to MCM window; added version checks to menus files; adjusted highlight alpha; fixed info text wrap width; fixed option scrolling; fixed mod list stacking; added INI settings for list width and initial message; added setting details to INI file

===============
Contact:
===============

Send a private message to Pelinor at New Vegas Nexus or at the Bethesda forums.

===============
License/Legal:
===============

The contents of this package are not to be redistributed by anyone. If your mod uses MCM menus, provide a link to the MCM mod page for the users.

This file is provided as is and the author holds no responsiblity for anything that may come to happen from using this file. (...?)