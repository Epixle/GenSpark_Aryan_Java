CONSOLE BASED PROGRAMMING PROJECT

This project creates a turn-based video game system that allows the user to
interact by being able to create their own characters, choosing the number of
enemies, and then being able to attack with user input (up until one opponent
is left in which case the program auto attacks and finished). The program is
split into a few different packages with their own purposes. There is the
characters package which includes the parent class Fighter along with a couple
child classes that extend the parent to become the characters in the game.
There is also an RNG mechanic determining goblin attacks and crit rates. The
packages all are imported into each other and primarily the Encounter class
which runs the main game.

To run Main.java, you can either open a new project into IntelliJ/another IDE and copy the
files and packages into the src folder to
run the program; or export the files into a location accessible by a terminal with JDK
configured (with no other Java files containing a main method) and run:

1. javac StudentManagementSystem.java
2. java StudentManagementSystem

Inputting these lines into the CLI or starting the project in the IDE should start up the program.


ASSUMPTIONS AND DESIGN DECISIONS

Here as well, the user can name their characters (not goblins which are auto
generated numeric names) as whatever they want as long as it is not blank.
Another admittedly large assumption is that when the user chooses an enemy to
attack, that they properly choose the index of the enemy instead of the name.
Since both are numeric, it might be a little confusing for the user. Instead of
doing something like choosing between 1-3 if there are 3 goblins fighting, the
user might try to input 7 if the goblin is named Goblin 7.