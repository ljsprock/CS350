================================================
Two Player GUI-Based Implementation of Quoridor
================================================

For the second sprint, we will focus on refining the game's fit and finish. We
will focus on implementing a graphical user interface (GUI) for the two-player
version of Quoridor so the gameplay feels more natural and flows.

Problem Description
===================

In a terminal-based version of Quoridor, players' enjoyment may be limited by
the graphics displayed by ASCII characters in the terminal window. A GUI
provides a visibly appealing way to display the game and have user interaction
beyond the keyboard.

Benefits of implementing Quoridor as a GUI include instant visual
feedback, clearer display information (drawing the game in the terminal creates
an unclean look with attempting to get characters to line up), and a more
intuitive way to play the game. The players do not have to enter commands
into the terminal, but can instead click on the GUI to make their moves,
simplifying the learning experience, while making it colorful.

Requirements
------------

**Functional Requirements**

* This implementation of Quoridor shall display a welcome screen when initially
  started and initialize a two-player, GUI version of the game.
* This implementation of Quoridor shall use a graphical user interface to
  display positions of pawns and walls, allowing players to click on positions
  on the game board they want to move to, and positions where they would like
  to place their walls.
* This implementation of Quoridor shall allow for the user to skip to the end
  screen at any point in the game using an "End Game" button, which will
  display the game winner.

**Non-Functional Requirements**

* This implementation of Quoridor shall display a 9x9 game board with pawns
  and walls in the GUI.
* This implementation of Quoridor shall display the players' pawns as red and
  blue circles on the game board.
* This implementation of Quoridor shall display the walls as black rectangles
  between grid square positions.

Use Cases
---------

**Primary Actor**: Jim.

**Secondary Actor**: Chris.

**Preconditions**: Chris and Jim want to play a game of Quoridor together.

**Scenario**: Jim and Chris meet each other at a predesignated spot, and Chris
brings his laptop. They are in an area where they can focus and strategize.
Cadet A runs the Quoridor program and the GUI version of Quoridor appears on
the screen with a welcome message. The game begins and each player takes turns
moving their pawn or placing a wall by clicking on the desired position on the
game screen. The game ends when either player reaches their opponents side of
the board. The game displays a congratulations message to the winner and a
thank you for playing message and exits.

Proposed Change
===============

To implement the GUI, we will utilize Java's Swing libraries. We experimented
with this library in CS 330. The GUI will be made using a DrawingPanel. The
GUI will be a single DrawingPanel that will display the game board and
utilize mouse listeners to see where the player clicked and record their
move, whether that be moving their pawn or placing walls.


Alternatives
------------

An alternative to a GUI would be to display the game board using a
DrawingPanel and keeping the pawn movement and wall placement terminal-
based. The disadvantage of this alternative is that the players might have
to switch back and forth between windows to see the game board and enter
their moves. Although windows may be resized, not every screen or monitor is
large enough to fit both at a comfortable viewing size, and users may not
enjoy that implementation.

Another alternative is to display the game board in a DrawingPanel and having
the GUI as a separate window. This alternative, although viable and satisfies
the requirements of a GUI, may cause issues for players if they are playing on
a small screen with little screen real estate. This alternative has the same
issue as the previously mentioned one. Therefore the single-window GUI
implementation of Quoridor is the most suitable implementation.

Testing
=======

To test this implementation of Quoridor, test cases will be written to
verify correct functionality of the GUI. The tests to be performed will be
written in a text document along with their expected responses/behaviors to
be verified.

Documentation
=============

The changes will be documented by in-line comments in the source code.

Implementation
==============

Work Items
----------

The phases that will be implemented are as follows:

1. Game setup with start and end screens and turns implemented.
2. Board display - 9x9 grid.
3. Pawn movement - Pawns will be moved by clicking on the desired
   position to move to.
4. Placement of walls on board - Walls will be able to be placed on the
   board at structured intervals by clicking on the position of desired
   placement.

Assignee(s)
-----------

C2C Wang will be the scrum master for this project.

Pair programming will be utilized for this sprint with the pairs as follows:
  C2C Sprock and C2C Wang
  C1C Leslie and C2C Gills
  C2C Chwa will assist as needed, review other's work, and code individually.

References
==========

None
