Elixia::Component::Ammunition
=============================

Purpose
-------

This component represent all the ammunition available for an entity.

Code
----

.. code-block::cpp

    class Ammunition: public IComponent
    {
    private:
	    // Lasers
	    size_t _lcb10;
	    size_t _mcb25;
	    size_t _mcb50;
	    size_t _xvg75;
	    size_t _sab50;
	    size_t _rsb75;

	    // Rockets
	    size_t _r310;
	    size_t _plt2026;
	    size_t _plt2021;
	    size_t _plt3030;
	    size_t _eco10;
	    size_t _ubr100;
	    size_t _sar02;
	    size_t _hstrm01;

	    // Mines
	    size_t _acm1;
	    size_t _empm01;
	    size_t _sabm01;
	    size_t _ddm01;
    };

Data explanation
----------------

We're not gonna explicitly explain each attributes but as the comments say, this component is split in 3 parts :
- Lasers -> amount of each type of ammunition.
- Rockets -> amount of each type of basic rocket et rocket form rocket launcher.
- Mines -> amount of each type of mine.