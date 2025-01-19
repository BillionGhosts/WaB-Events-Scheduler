# WaB-Events-Scheduler

[Warlock And Boobs](https://boobsgames.itch.io/warlock-and-boobs) - Event Scheduler mod

# WARNING:

MAKE BACKUP SAVE OF YOUR PLAYTHROUGH JUST IN CASE. MOD HAVE A FEATURE
THAT CAN PURGE ITSELF FROM YOUR SAVE FILE SO THAT YOU COULD TRANSFER IT TO NEWER VERSION OF
THE GAME. BUT STILL, BE CAREFUL.

# Description and contents

This mod adds event scheduler and widget for it. The scheduler itself is an item that you can find in "key items" menu.
It tells you what events are happening in what day and time (one page - one day divided by time).
The widget by press of a button shows you what events happening in current day/time combo and goes away when you trigger
that event. Widget is refreshed every day. But first you'll have to trigger events by yourself so that they become
enabled
(so Krowly could write it down in his scheduler). Also, when you see "I should write it down" line of dialog that means
that event is remembered and will appear in scheduler and widget.

# Acquire

Scheduler lies in Krowly's basement to the right of red magic book.
Widget activates when you pick it up also.
To open widget press W (by default, that is same button that shows Krowly), and to
navigate Scheduler use arrows to change page and Z (by default) to exit.

# Emergency actions

You can also put down your scheduler in same place. You will be given two options:

- Put it back: because all events are checking if you have scheduler, you safely can return scheduler if you encounter
  any bugs with events. Your progress will be saved though.
- Update Entries: if and when this mod will be updated there maybe will be some new entries/removed/modified entries in
  scheduler. In order to  "update" your scheduler you can use this option. Your progress will be saved
- Purge mod from save: it nulls out all variables and switches in your save (also remove scheduler from the player) so
  that this save could be used in newer version of the game. I tested this feature and it worked for me on clean modless
  version of the game.

# Cheat

You can use cheat room to just enable all events. The sword, stuck in the floor, will appear there if you have scheduler
on you. Activate it to enable all events. Deactivate to erase your progress and start again.

# Known issues

- Be advised that "purge mod from save" may not completely purge your save. I tested feature myself but who knows what
  else can be contaminated apart from variables and switches and whatnot

- Always close your widget screen if you don't need it. It draws on screen almost all the time until deactivated.
  Although i added forced close of widget to the save screen (otherwise it tried to 'save' widget graphics as well and
  corrupted the save),
  i didn't add this forceful closure to all places in game.
- The widget button is rather finicky to press. Case RPG Maker don't listen to button WAS PRESSED and listen's to BEING
  PRESSED. And because of that it just almost constantly listen to button being pushed and it checks it every N frames.
  For now it listens to it every 7 frames. So what happens is - you gently press the button and widget will appear but
  standard Krowly's showcase will appear also. Problem is - they appear to check button press in different timings. So
  you can press widget button once and widget will appear and Krowly's graphic not. Then you press it again and widget
  disappears but Krowly appears and so on. You can try to double tap button to avoid this but it needs getting used to.

# Installation

- Get rpg maker decrypter from github [uuksu/RPGMakerDecrypter](https://github.com/uuksu/RPGMakerDecrypter/releases)
  Also you can see instructions on [F95Zone](https://f95zone.to/threads/rpg-maker-unpacker.50/)
- Make a backup of your save files and Game.rgss3a file.
- Unpack Game.rgss3a data file with decryptor:
- - Move RPGMakerDecrypter-cli to the game folder, then open your cmd, navigate to the game folder via 'CD' command.
- - Then do "RPGMakerDecrypter-cli Game.rgss3a" command, and it should extract 'Data' folder to your game's folder.
- Copy mod's content (the Data folder) in your game folder
- Delete encripted archive of game data (Game.rgss3a). Otherwise, it will be prioritized over your modded game folder

