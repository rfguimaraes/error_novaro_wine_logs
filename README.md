# Error NovaRO's 2020 client with wine 5

Log files to aid in debugging an error with NovaRO's 2020 client on wine 5 

# Description of the problem

The new client crashes more often than the old one, and since it will become the
only one supported soon I think this could be looked into now.

Similar crashes happen more frequently during long dialog sections (with the
text boxes and buttons showing up). Next, is a list of portions of the game
where these crashes have been observed:

- Terra gloria quests: very frequently during the long dialogs involving Lazy. 
- Geffen Magic Tournament: sometimes when the Desert Wolf spawns during the
  trial to be allowed to register.
- Geffen Magic Tournament: very rarely during some matches.
- Monster Trivia at the Summer Event: right before the four options appear on
  the screen.

These issues also have been observed with wines 5.11, 5.12 and 5.13 (none of
them staging versions).

For some reason I could note use winedbg to trace this problem. 
As soon as the debbugger is attached, the program crashes.

In the future more log files may be added.

# Changelog

- Add log files from the crash at Geffen Magic Tournament in the match against
  Ju.
- Add log files and screeshot at Monster Trivia in Summer Festival (note that
  the screenshot shows that the menu with the options was not displayed, the
  game crashed when I pressed "Enter")
