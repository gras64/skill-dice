# skill-dice skill

Dice rolling skill for the mycroft assistant.
This skill rolls dice in RPG notation.

Command syntax: <wake word> roll 3d6

## Current state

Working features:
 - rolls dice when spoken in RPG notation

Known issues:
 - Sometimes commands are misinterpreted. "4d6" is heard as "46" or "40 6"
 - Sometimes dice notation is interpreted with an extra space which breaks the split("d") code. Ex: "4d6" is interpreted as "4d 6" and the code tries to roll 4 null side dice instead of 6 sided dice.

TODO:
 - "roll <number> <number>-sided dice" syntax
 - Fix issue with split()
