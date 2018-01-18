Elixia::Component::Shoot
========================

Purpose
-------

This component tell if an Entity can shoot and the data behind.

Code
----

.. code-block::cpp

    class Shoot: public IComponent
    {
    private:
        size_t _baseDamage;
        double _attackSpeed;
        double _shotSpeed;
    };

Data explanation
----------------

``_baseDamage`` -> Minimum damage that can be deal.

``_attackSpeed`` -> Fire rate (Shot / Second).

``_shotSpeed`` -> Speed of the projectile fired.

