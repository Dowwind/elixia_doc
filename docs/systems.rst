Elixia::Systems
===============

Introduction
------------

In those parts, we'll see all the systems thar **Project: Elixia** use for managing his components. For each systems the documentation will contains those parts :

Purpose
*******

In this part, we'll talk about the main purpose of each system. What they have to managed, on which component they work and with which events they react.

Implementation
**************

via C++ code snippets, we'll see `basically` how the System is.

Events
******

In this part, we'll see all the events that the system handle with a description of the behavior and we'll see the reaction lambda with C++ code snippets.

On initialization
*****************

This part will list all actions that a system do during his initialization.

During run
**********

In this part, we'll document what the system do during a call to his run method.

Destruction
***********

For this last part, we'll see what the system do before and during his destruction. Also, we'll document his **after_death** lambda.

List
----

So, here's a list of all **Systems** currently on the project.

+-----------------+----------------------------------------------+------+
|  Money          | Manage the money component                   | TODO |
+-----------------+----------------------------------------------+------+
|  GameManager    | Manage a game                                | TODO |
+-----------------+----------------------------------------------+------+
|  LevelManager   | Manage enemies waves in a game               | TODO |
+-----------------+----------------------------------------------+------+
|  Health         | Manage the health component                  | TODO |
+-----------------+----------------------------------------------+------+
|  Shield         | Manage the shield component                  | TODO |
+-----------------+----------------------------------------------+------+
|  Purchase       | Manage the shop                              | TODO |
+-----------------+----------------------------------------------+------+
|  AiManager      | Manage the AIs intelligences                 | TODO |
+-----------------+----------------------------------------------+------+
|  Account        | Manage the player's account                  | TODO |
+-----------------+----------------------------------------------+------+
|  MainMenu       | GUI of the main menu                         | TODO |
+-----------------+----------------------------------------------+------+
|  GameMenu       | GUI during a game                            | TODO |
+-----------------+----------------------------------------------+------+

.. toctree::
   :maxdepth: 2

   Systems/Money
   Systems/GameManager
   Systems/LevelManager
   Systems/Health
   Systems/Shield
   Systems/Purchase
   Systems/AiManager
   Systems/Account
   Systems/MainMenu
   Systems/GameMenu