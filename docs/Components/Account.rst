Elixia::Component::Account
==========================

Purpose
-------

This component will store all the useful information about a player's account.

Code
----

.. code-block:: cpp

    class Account: public IComponent
    {
    private:
	    std::string _username;
	    std::string _email;
    };


Data explanation
----------------

`_username` -> represent the username that will be display in the game. Also, other players can search a player with his username.
`_email` -> trivially, represent the email.

