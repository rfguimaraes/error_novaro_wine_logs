# Errors in NovaRO's 2020 client with wine 5

Log files to aid in debugging an error with NovaRO's 2020 client on wine 5 

# Description of the problem

The new client crashes more often than the old one, and since it will become the
only one supported soon I think this could be looked into now.

Similar crashes happen more frequently during long dialog sections (with the
text boxes and buttons showing up). Next, is a list of portions of the game
where these crashes have been observed:

- Terra gloria quests: very frequently during the long dialogs involving Lazy (I
  could not finsh the questline with the beta client). 
- Geffen Magic Tournament: sometimes when the Desert Wolf spawns during the
  trial to be allowed to register.
- Geffen Magic Tournament: very rarely during some matches.
- Monster Trivia at the Summer Event: right before the four options appear on
  the screen.
- Half-moon in the Daytime: either during the second dialog with the Pope, or
  in the long dialog with Pope and Lumin near the end (I could not finish the
  instance a single time with the 2020 beta client).

These issues also have been observed with wines 5.01, 5.11, 5.12 and 5.13 (none
of them staging versions) and 5.15 (staging version from Fedora 32's
repository).

For some reason I cannot use winedbg to trace this problem. 
As soon as the debbugger is attached, the program crashes.

In the future more log files may be added.

# Changelog

31 Aug 2020

- Added log files for one occurrence during the instance Half-moon in the
  Daytime.

07 Aug 2020

- Add logs files of crashes during the main quest of the Illusion of the
  Vampire. One when talking to Jubilee and the other when talking to Dracula.

06 Aug 2020

- Add log files and screenshot from Monster Trivia in Summer Festival (note that
  the screenshot shows that the menu with the options was not displayed, the
  game crashed when I pressed "Enter").

- Add log files of the very common crash when the Desert Wolf spawns in GMT
  (inside the instance, but before the actual tournament).

Initial commit

- Add log files from the crash at Geffen Magic Tournament in the match against
  Ju.
