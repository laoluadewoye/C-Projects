# Welcome to My Battleship Game!

This code at is core is just me practicing how to use Object Oriented Programming, how to code in C/C++, and how to create public docker containers since I wanted to share it but my friends don't have all the coder software installed. It took two years, lots of struggling, three different IDEs, and a whole lot of Chat-GPT to help me set up VS Code's debugger but I finally got something together!

The structure of the program is as such-

* Main - the file used to test classes and start the game.
* Battleship - the class responsible for Top-level game management. Mainly a space where players can communicate with each other.
* Player - the class that holds all the functionality to allow the player to place ships.
* Computer - the class that builds on top of the Player class to add decision-making for CPUs to play relatively alright against someone.
* Ship - the class that is responsible for representing a ship's existence on the battlefield, including whether if its dead or not.
* Location - the class that acts as the API between the player and the battlefield, responsible for managing views of battlefields.
* Grid - the class responsible for storing and showing the state of a given battlefield. 

How this program works is that the main program will create a battleship object and start the game. The battleship object, in turn, manages two player objects. They place their ships then spend an undetermined amount of turns racing to destroy each other's battleships. To tell if there were hits or not are on the receiver's end of each attack, and they check with the ship objects to do this. Afterward, they then ask the location objects to modify the grids to reflect misses, hits, and all other changes.

# My proud AI

The AI was, for two years, the bane of my existence. It would be so simply if I was in Python and I can create all the data structures I want with ease, but C forced me to come up with something creative. A huge goal for this project was to use only basic arrays and data structures, and having a 2D structure felt weird, so instead, I created a stack!

The 