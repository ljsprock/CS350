====================================================
Two Player Terminal-Based Implementation of Quoridor
====================================================

Especially in an environment as diverse as USAFA, cadets often find difficulty
in getting to know an acquaintance. Many people overcome this initial
awkwardness with a game. Whether it be chess, spoons, or Go, these games act to
break down interpersonal barriers and aid communication and camaraderie through
friendly competition. The game of Quoridor has great potential to aid these new
relationships and deepen the resulting friendships. The game's very few
rules are easy to learn and no two games are alike. This ensures continued
enjoyment and many friendships built around Quoridor.

Problem Description
===================

The problem that our software aims to solve is cadets not having a common game
to play together. Due to them coming from across the United States, they may
only know games specific to their region. Furthermore, many of these games are
difficult to teach another person. Thus, we need to develop an easy to learn,
engaging, and highly competitive for cadets to bond over.

Requirements
------------

**Functional Requirements**

* This implementation of Quoridor shall display a welcome screen when initially
  started and initialize a two-player game.
* This implementation of Quoridor shall use basic terminal-based graphics to
  display positions of pawns and walls.
* This implementation of Quoridor shall begin a player in the center of an
  end of the board.
* This implementation of Quoridor shall spawn only one player on each side of
  the board.
* This implementation of Quoridor shall adhere to the rules of Quoridor
  detailed below.
* This implementation of Quoridor shall cycle through each player's turn such
  that no player has two turns before each turn cycle resets.
* This implementation of Quoridor shall end when one player reaches the
  opposite side of the board.
* This implementation of Quoridor shall allow for the user to skip to the end
  screen at any point in the game. If the skip to end screen option is taken,
  the player who is the closest to their oponents side of the board is the
  "winner".
* This implementation of Quoridor shall shall have the win screen congratulate
  the winning player and display a thank you message for playing.

**Quoridor Rules (Functional Requirements)**

* This implementation of Quoridor shall allow a player to either move their
  pawn or place a wall each turn cycle.
* This implementation of Quoridor shall not allow a wall from being moved once
  it is placed.
* This implementation of Quoridor shall only allow a wall to be placed if it
  does not completely block an opponent from their opposite side of the board
  and the wall does not overlap with a previously placed wall.
* This implementation of Quoridor shall only allow a pawn to move vertically
  or horizontally one space when the adjacent spaces are not taken by a
  wall or pawn.
* This implementation of Quoridor shall allow a pawn to move two spaces in
  the direction of a pawn if it is adjacent to it and the space it is moving
  is unblocked by a wall.
* This implementation of Quoridor shall prevent a pawn moving one space
  in the direction of a wall if it is adjacent to it.
* This implementation of Quoridor shall allow a pawn to move diagonally to the
  relative right or left of an adjacent pawn if the space behind the opponents
  pawn is blocked by a wall.

**Non-Functional Requirements**

* This implementation of Quoridor shall display "X" and "Y" as the player's
  pawn pieces and display horizontal walls using "=", and vertical walls
  using "|".

Use Cases
---------

**Primary Actor**: Cadet who wants to know another cadet by playing a game.

**Secondary Actors**: Cadets who also want to meet new people through a fun
game.

**Preconditions**: Cadets are in a quiet area where they can all play around
a single computer.

**Scenario**: A cadet (cadet A) wants to play Quoridor with an acquaintance
or friend (cadet B). They are in an area where they can focus and strategize.
Cadet A runs the Quoridor program. The game begins and each cadet takes turns
moving their pawn or placing a wall. The game ends when a player
(either cadet A or cadet B) reaches their opponents side of the board. The
game displays a congratulations message to the winner and a thank you for
playing message and exits.


Proposed Change
===============

The proposed change is a two-player, terminal-based version of Quoridor.
The software system will allow two users to play Quoridor in a turn-based
fashion with both members playing from the same computer. This will be the
first implementation with later sprints introducing a graphical user interface
and a four player option. The basics of this sprint will include calculating
legal moves including moving pawns and placing walls, and printing a simple
board using spaces and lines in the terminal to show players where their pieces
are.

* The GameBoardClass will hold the information (including pawn placement and
  wall locations) for the 9x9 game board in a two-dimensional array of
  characters.
* The PawnClass will initialize the pawns locations and handle pawn movement
  functionality. The pawn symbols for will be X and Y, for player one and
  player two, respectively.
* A while loop will be used to play the game with the exit condition being a
  player's pawn reaching the opponents end of the board. In each iteration of
  the loop, player one will either move their pawn or place a wall, followed
  by player two.

Alternatives
------------

There are no alternative development methods for Quoridor. Agile software
development is the best for cadets with busy schedules and many
responsibilities; taking an agile approach allows small sprints of
development and implementation which allows cadets to focus on a smaller
task. The development of a two player terminal based game of Quoridor in a
month long sprint keeps the goal attainable while providing more freedom than
the waterfall method.

Additionally, Agile development helps us adjust to changing requirements.
Since, again, we do not know what our third specification will entail, we will
need to be able to react to requirements that may be changed.

Testing
=======

Unit testing for functions will be conducted to ensure that all the functions
work as intended before integration with the whole system. Edge cases for
each function will be tested as each change is developed. JUnit will be
utilized to ensure the functions perform as expected. Specific test cases
to guard against expected faults such as a pawn going outside of the playing
board.


Documentation
=============

None


Implementation
==============

Work Items
----------

This feature will indeed be implemented in phases! The phases that will
be implemented are as follows:

1. Basic game structure with start and end screens and turns implemented.
2. Basic board display. Board will display a 9x9 grid.
3. Basic board movement. Pawns will be able to move one square horizontally
   or vertically. Game ends when player pawn is within a range of spaces
4. Placement of walls on board. Walls will be able to be placed on the
   board at structured intervals.
5. Player collision rules. Players may not move through another player or
   walls.
6. Board placement rules. Walls may not be placed such that they block a
   player’s path completely.

Assignee(s)
-----------

C2C Wang will be the project lead, or “scrum master” for this project.
C2C Chwa will be the technical lead for implementing this specification.
He will both work on feature implementation and advise the other members
of the team on how to complete their tasks.

Primary assignee:
  C2C Jim “Scrum Master” Wang - c22jim.wang@afacademy.af.edu

Other contributors:
  Lead : C2C Christopher Chwa - c22christopher.chwa@afacademy.af.edu

  C2C Lauren Sprock - c22lauren.sprock@afacademy.af.edu

  C2C Grady Gills - c22grad.gills@afacademy.af.edu

  C1C Erin Leslie - c21erin.leslie@afacdemy.af.edu

References
==========

None
