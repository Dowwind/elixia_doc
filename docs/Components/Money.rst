Elixia::Component::Money
========================

Purpose
-------

This component represent the money that a Entity can have. Also, it will store multipliers that can be applied on transaction.

Code
----

.. code-block:: cpp

    class Money: IComponent
    {
    private:
	    size_t _money;
	    size_t _addMultiplier;
        size_t _removeMultiplier;
    };

Data explanation
----------------

``_money`` -> is the amount of money.

``_addMultiplier`` -> is the multiplier that have to be used when adding money.

``_removeMultiplier`` -> is the multiplier that have to used when removing money.
