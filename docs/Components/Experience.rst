Elixia::Component::Experience
=============================

Purpose
-------

This component represents the experience that an entity can have. Also, it will store a multiplier that can be applied when changing experience and the actual rank of the entity.

Code
----

.. code-block:: cpp

    class Experience: public IComponent
    {
    private:

  	    size_t _xp;
  	    Elixia::Meta::Rank _rank;
  	    size_t _multiplier;

    public:
  	    IEntity &getEntity() const;
    };

Data explanation
----------------

``_xp`` -> the amount of experience.
``_rank`` -> the actual rank.
``_multiplier`` -> the multiplier that have to be used when changing experience.