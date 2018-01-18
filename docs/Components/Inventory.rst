Elixia::Component::Inventory
============================

Purpose
-------

It's a set of List of all items that can be bought or loot owned by the associated entity.

Code
----

.. code-block:: cpp

    class Inventory: public IComponent
    {
    private:
	    bool _inBoard;
	    std::list<Elixia::Gameplay::Laser> _lasers;
    	std::list<Elixia::Gameplay::Shield> _shields;
	    std::list<Elixia::Gameplay::Protocol> _protocols;
	    std::list<Elixia::Gameplay::Ship> _ships;
	    std::list<Elixia::Gameplay::Design> _designs;
    };

Data explanation
----------------

``_inBoard`` -> This boolean tell if the inventory is a global one or if it represents the inventory of a ship.

``_lasers`` -> List of all lasers.

``_shield`` -> List of all shields.

``_protocols`` -> List of all protocols.

``_ships`` -> List of all ships.

``_designs`` -> List of all designs.
