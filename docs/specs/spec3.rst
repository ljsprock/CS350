====================================================
AI Player Addition to the Implementation of Quoridor
====================================================

For the third and final sprint, we will focus on creating an Artificial
Intelligence (AI) computer-player so that single players may play Quoridor by
themselves. The AI will have basic functions such as placing walls and
moving the pawn.


Problem Description
===================

Individuals may not always have someone around them to play Quoridor with
or have someone who wants to play Quoridor. By implementing an AI player,
individuals can play a game of Quoridor by themselves and still enjoy the
game.

Requirements
------------

**Functional Requirements**

The AI shall follow all rules of Quoridor.

* The AI shall only play when it is its turn.
* The AI shall move its pawn or place a wall as its turn.

**Non-Functional Requirements**

* The AI shall have a turn time of less than 5 seconds.
* The AI shall be a selectable option from the start screen.

Use Cases
---------

**Primary Actor**: Lauren.

**Secondary Actors**: None.

**Preconditions**: Lauren wants to play a game of Quoridor during a study
break.

**Scenario**: Lauren, following a two-hour study session for her CS350 Software
Engineering final exam, opens up Quoridor on laptop; she is alone in her room
and does not have anyone around her to play with. Lauren runs the Quoridor
program and the GUI version of Quoridor appears on the screen with a welcome
message. Lauren selects the option to play against a “Computer”, which is the
AI. The game begins and Lauren and the AI take turns moving their pawns or
placing walls by clicking on the desired position on the game screen. The game
ends when Lauren or the AI reaches the opponents side of the board. The game
displays a congratulations message to the winner, thanks Lauren for playing,
and exits.

Proposed Change
===============

The AI will be implemented by building a basic set of moves that will be tested
for legitimacy based off the game’s current state. If an action is legal, then
the AI’s pawn is moved, or a wall is placed.

Alternatives
------------

An alternative would be to create a server where individual players can find
an opponent online, however, this is beyond the scope this class and would
not easily be accomplished in a three-week sprint.

Testing
=======

To test this implementation of Quoridor, unit tests will be written to verify
correct functionality of the AI.

Documentation
=============

The changes will be documented by in-line comments in the source code.

Implementation
==============

Work Items
----------

The phases that will be implemented are as follows:

1. Add an option to play against an AI player on the start screen.
2. Analyze the current game board to build a database build a database of
   moves and assign certain moves a higher priority to be executed if they
   are legal.
3. Write unit tests.


Assignee(s)
-----------

C2C Wang will be the scrum master for this project.

Pair programming will be utilized for this sprint with the pairs as follows:
  C2C Sprock and C2C Wang
  C1C Leslie and C2C Gills
  C2C Chwa will assist as needed, review other's work, and code individually.

References
==========

None.
