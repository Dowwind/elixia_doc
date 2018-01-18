Elixia::Component::Damage
=========================

Purpose
-------

This component contain data about a projectile.

Code
----

.. code-block:: cpp

    class Weapon: public IComponent
    {
    private:
        size_t _damage;
        IEntity &_from;
    };

Data explanation
----------------

``_damage`` -> how much damage the projectile will deal.
``_from`` -> the entity that have launched the projectile.