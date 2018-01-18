Elixia::System::Money
=====================

Purpose
-------

This system, has his name shows, is for manipulating the Money_ component on client and server side.

.. _Money: ../Components/Money

Implementation
--------------

.. code-block:: cpp

    namespace Elixia
    {
        namespace System
        {
            class Money: public ISystem
            {
            };
        }
    }

Events
------
The system is divided in two parts : server and client

Server
******

- React to the MoneyTransaction_ event.

.. code-block:: cpp

    addReaction<Elixia::Event::MoneyTransaction>([this](futils::IMediatorPacket &pkg) {
        auto &packet = futils::Mediator::rebuild<Elixia::Event::MoneyTransaction>(pkg);
        auto comp = packet.comp;

        if (packet.isPurchase)
            comp._money += packet.transaction;
        else
            comp._money += (packet.transaction * comp._multiplier);
    };

.. _MoneyTransaction: ../Events/MoneyTransaction

On initialization
-----------------
Do nothing particular.

During run
----------
This system only reacts to events, his run method is just a return;

Destruction
-----------
Do nothing particular.
