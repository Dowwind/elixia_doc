Elixia::Component::Weapon
=========================

Protocol
--------

This component represent the current Weapon that are used by an entity.

Code
----

.. code-block:: cpp

    class Weapon: public IComponent
    {
    private:
        Elixia::Gameplay::LaserMunition _lasers;
        Elixia::Gameplay::RocketMunition _rockets;
        Elixia::Gameplay::MineMunition _mines;
    };


Data explanation
----------------

Each attribute represents a type of ammunition currently use.

``Elixia::Gameplay::LaserMunition`` -> enum that represent each laser ammunition.
``Elixia::Gameplay::RocketMunition`` -> enum that represent each rocket ammunition.
``Elixia::Gameplay::MineMunition`` -> enum that represent each mine ammunition.
