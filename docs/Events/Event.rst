Elixia::Event
=============

MoneyTransaction
----------------

What it represent
*****************

The purpose of the event is to tell the **Money** system that a transaction need to be done. A `transaction` is a simple action on an Money_ component.

.. _Money: ../Components/Money

Code
****

.. code-block:: cpp

    struct MoneyTransaction
    {
        int64_t amount;
    };


ShootRequest
------------

What it represent
*****************

Raise by the Shoot_ system to ask if an Entity can shoot.

.. _Shoot: ../Systems/Money

Code
****

.. code-block:: cpp

    struct ShootRequest
    {
        IEntity *from;
    };


IncreaseExperience
------------------

What it represent
*****************

Trivial.

Code
****

.. code-block:: cpp

    struct IncreaseExperience
    {
        size_t amount;
        Elixia::Component::Experience &to;
    };

RankChanged
-----------

What it represent
*****************

Trivial.

Code
****

.. code-block:: cpp

    struct RankChanged
    {
        Elixia::Gameplay::Rank newRank;
        Elixia::Component::Experience &to;
    };

PurchaseRequest
---------------

What it represent
*****************

Represent a purchase request.

Code
****

.. code-block:: cpp

    struct PurchaseRequest
    {
        IEntity *for;
        Elixia::Gameplay::Item *what;
    };

SuccessfulPurchase
------------------

What it represent
*****************

Trivial.

Code
****

.. code-block:: cpp

    struct SuccessfulPurchase
    {
        IEntity *for;
        Elixia::Gameplay::Item *what;
    };

BadPurchase
-----------

What it represent
*****************

Trivial.

Code
****

.. code-block:: cpp

    struct BadPurchase
    {
        IEntity *for;
        Elixia::Gameplay::Item *what;
    };

ChangeLaserWeapon
-----------------

What it represent
*****************

Raise when user changes which laser ammunition he wants to use.

Code
****

.. code-block:: cpp

    struct ChangeLaserWeapon
    {
        Elixia::Gameplay::LaserMunition newLaser;
        IEntity *for;
    };

ChangeRocketWeapon
------------------

What it represent
*****************

Raise when user changes which rocket ammunition he wants to use.

Code
****

.. code-block:: cpp

    struct ChangeLaserWeapon
    {
        Elixia::Gameplay::RocketMunition newLaser;
        IEntity *for;
    };

ChangeMineWeapon
----------------

What it represent
*****************

Raise when user changes which mine ammunition he wants to use.

Code
****

.. code-block:: cpp

    struct ChangeLaserWeapon
    {
        Elixia::Gameplay::MineMunition newLaser;
        IEntity *for;
    };