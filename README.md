# Naming.scpt
## by Chris Sauvé of [pxldot](http://pxldot.com)


## Description
This script performs find-and-replace operations on all selected OmniFocus items. It searches through the project name and notes for the given strings and then replaces them with the replacement strings you specify. It can do multiple replacements simultaneously and can replace only a certain number of instances of the string, if you wish.

## Syntax
The general syntax is as follows: `[string1] > [replacementString1]`. This will replace every instance of the string `string1` with `replacementString1`. You can change the string/ replacement delimiter from its default of `>` by editing the `replaceDelimiter` property in the script. You can also use the following additions to this basic syntax:

- `//` separates replacement pairs. For example, `[string1] > [replacementString1] // [string2] > [replacementString2]` will replace both pairs. You can change this by editing the `pairDelimiter` property in the script.

- `*` designates the number of times you wish to make the give replacement. For example, `[string1] > [replacementString1] *3` will replace the first three instances of the replacement pair. You can change this by editing the `occuranceDelimiter` property in the script.


## Installation
Download the most recent version of the script. Once you have downloaded the script, navigate to your Application script folder located at `~/Library/Scripts/Applications/OmniFocus`. Apple hides the Library folder in Mac OS X 10.7 or later by default, so the easiest way to get to this folder is to select the menu item `Go > Go To Folder...` in Finder.app. You may have to manually create an OmniFocus folder in the `~/Library/Scripts/Applications` directory if you do not have any previous scripts for OmniFocus (you may have to create more of the folders in the directory; if you don't have an Applications folder or even a Scripts folder, you will have to create those as well).


## Using The Script
There are countless ways you can run the script. If you are a pro user, you likely know even more ways than I do: options like launching the script from FastScripts, Alfred, LaunchBar, or a Keyboard Maestro macro are all available to you. Below I'll explain two ways to run the script, primarily targetted at more novice users.

Your first option is to run the script from Apple's AppleScript menu. If you don't have a little script icon near the clock in your Mac's menubar, you need to turn this on manually. Open AppleScript Editor.app from your `Applications > Utilities` folder. Go to AppleScript's preferences by selecting `AppleScript Editor > Preferences...` from the menubar. On the "General" pane, you should check the checkbox to "Show Script menu in menu bar". Now, when in OmniFocus, select the new script menubar item and you will see the script at the bottom of the list, ready to be clicked and run.

OmniFocus has another way to run scripts, and it's even easier than the method described above. Once the script is installed, go to OmniFocus and right- (control-) click on the toolbar (the gray bar at the top of the window that shows icons for your inbox, projects, and more). Choose "Customize Toolbar..." from the contextual menu that pops up. You will then see a list of all items that can be put in your menubar, including (at the bottom) any scripts that you have installed. Drag the script anywhere on the toolbar and click "Done". You now have one-click access to run this script!


## Version History
- **0.1.1** (February 11, 2013): Now searches and replaces the notes field as well

- **0.1.0** (January 14, 2013): Initial release


## License
Use it, change it, repackage it, whatever. Try not to take credit for my work.