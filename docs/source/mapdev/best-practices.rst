Best Practices
==============

While LevelImposter will enable you to create just about anything, making a map that follows the same style as the original game is a good idea.
This will make it easier for players to understand the layout of the map, and will make your map blend in with the rest of the game.

Camera
------

Among Us's camera utilizes a `3/4 perspective <https://tvtropes.org/pmwiki/pmwiki.php/Main/ThreeQuartersView>`_. This means that the camera is set to a 45° angle, the sprites are drawn in 2D, and there is no "gravity".
This is traditional to classic JPRGs such as the original Pokemon and Zelda games.
In order to follow this style, rooms should display the front and tops of walls, but not the sides.

.. image:: https://i.imgur.com/bmAytTy.jpg
    :alt: Perspective Example
    :align: center

Art
---

.. image:: https://i.imgur.com/f6y1ew9.png
    :alt: Crewmate Example
    :height: 100px
    :align: left

Unlike Pokemon and Zelda, Among Us has a very cartoony art style.
More often than not, sprites are drawn with a very limited color palette, and are very simple in design.
In addition, sprites often have a very thick outline around them.
If shadows are present, they usually only use 1 or 2 colors and do not have any gradient.
An example of this is the crewmate sprite, which is only drawn with 6 colors.

Collision
---------

Room
^^^^

Colliders are the invisible boxes that are used to detect collisions between the player and other objects.
In Among Us, there are also used to block the player's vision.

In order to follow the original game's style, colliders on rooms and buildings should be drawn such that...
- 1 or more colliders that blocks vision follow along the top of the wall
- 1 or more colliders that doesn't block vision follow along the bottom of the wall

.. image:: https://i.imgur.com/ODpC02f.png
    :alt: Room Example
    :align: center

Short Objects
^^^^^^^^^^^^^

However, you may notice above that there aren't any colliders on the center table.
While you could throw a collider around it, the player won't be able to travel behind it.
In order to accomplish that, you must...

1. Separate the table into a dedicated sprite
2. Set it's Z to -5
3. Set it's collider area to where the bottom of the table would be

.. note::
    Z=-5 is used by the player. Anything more will be drawn behind the player. Anything less will be drawn in front of the player.

An example of this is shown below.

.. image:: https://i.imgur.com/jRfRXPp.png
    :alt: Table Example
    :align: center

Tall Objects
^^^^^^^^^^^^

This will work great, until you want a short object to block the player's vision.

.. figure:: https://i.imgur.com/y9pg0AF.png
    :alt: Bad Example
    :align: center
    
    If you attempt to enable vision block on a short object's collider, the shadow rays will make an ugly line over the object itself.

In order to remedy this, Among Us has a special property to disable shadow rays on a sprite called ``No Shadow``.

.. figure:: https://i.imgur.com/IeJwKYD.png
    :alt: Good Example
    :align: center

    Enabling ``No Shadow`` on the object will disable any shadow rays from being cast on it.

In addition, you may enable ``No Shadow Behaviour`` to dynamically enable/disable the ``No Shadow`` property based on the object's visibility.
A real-world examples of this can be seen in with large boxes in the storage on Skeld or the big rock in Polus.

Examples
--------

While it's one thing to list out the best practices, it's another to see them in action.
Below is an example map that we made to demonstrate these practices.

.. image:: https://firebasestorage.googleapis.com/v0/b/levelimposter-347807.appspot.com/o/maps%2FwiTQOndyAzcg4TQLYrEixnB5OBl1%2Fc1775d32-39f4-45d2-930d-5f6e3648313d.png?alt=media&token=3df74e34-e2fa-41bc-ac6f-724f59ea1a57
    :alt: Example Map
    :align: center
    :target: https://levelimposter.net/#/map/c1775d32-39f4-45d2-930d-5f6e3648313d