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
|  Money_         | Manage the money component                   | TODO |
+-----------------+----------------------------------------------+------+
|  GameManager_   | Manage a game                                | TODO |
+-----------------+----------------------------------------------+------+
|  LevelManager_  | Manage enemies waves in a game               | TODO |
+-----------------+----------------------------------------------+------+
|  Health_        | Manage the health component                  | TODO |
+-----------------+----------------------------------------------+------+
|  Shield_        | Manage the shield component                  | TODO |
+-----------------+----------------------------------------------+------+
|  Purchase_      | Manage the shop                              | TODO |
+-----------------+----------------------------------------------+------+
|  AiManager_     | Manage the AIs intelligences                 | TODO |
+-----------------+----------------------------------------------+------+
|  Account_       | Manage the player's account                  | TODO |
+-----------------+----------------------------------------------+------+
|  MainMenu_      | GUI of the main menu                         | TODO |
+-----------------+----------------------------------------------+------+
|  GameMenu_      | GUI during a game                            | TODO |
+-----------------+----------------------------------------------+------+

.. _Money: Systems/Money
.. _GameManager: Systems/GameManager
.. _LevelManager: Systems/LevelManager
.. _Health: Systems/HealthManager
.. _Shield: Systems/ShieldManager
.. _Purchase: Systems/Purchase
.. _AiManager: Systems/AiManager
.. _Account: Systems/Account
.. _MainMenu: Systems/MainMenu
.. _GameMenu: Systems/GameMenu