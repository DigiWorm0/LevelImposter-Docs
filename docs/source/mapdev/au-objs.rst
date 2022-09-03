Among Us Objects
=================

This is a variety of objects within the Among Us game as well as details on how to use them.

Vent
----

.. image:: https://editor.levelimposter.net/sprites/util-vent1.png
    :alt: Normal Vent
    :align: left

.. image:: https://editor.levelimposter.net/sprites/util-vent2.png
    :alt: Polus Vent
    :align: left

Vents ``util-vent*`` are used by impostors to discretly transport throughout the map.
If there is more than one vent in a map, you may connect them in the object inspector.
Due to limitations within Among us, each vent may have up to 3 connections to other vents.

.. image:: https://i.imgur.com/nJVhbaG.gif
    :alt: Vent animations
    :align: center

By default, vents will animate their default sprite.
However, custom vent animations can be provided by uploading a custom GIF as the vent's sprite.
The first frame of the GIF will be used as the default sprite, and the remaining frames will be used as the animation.
It is recommended to have a 1s long animation.

Cameras
-------

.. image:: https://editor.levelimposter.net/sprites/util-cam.png
    :alt: Camera
    :align: left

Cameras ``util-cam`` are used by players to surveil the map from a camera panel ``util-cams*``.
All cameras will automatically be connected to any camera panel ``util-cams*`` within the map.
The camera's zoom and offset can be viewed and adjusted in the object inspector.

Admin Table
-----------

.. image:: https://editor.levelimposter.net/sprites/util-admin.png
    :alt: Admin Table
    :align: left

Admin Tables ``util-admin`` are used by players to view which player is in which room.
In order to operate, the map must contain at least one room ``util-room`` with the admin table enabled.
Any players within the room ``util-room`` will be counted and displayed on the admin table automatically.

For more information on room objects, see :doc:`/mapdev/custom-objs`.

Moving platform
---------------

.. image:: https://editor.levelimposter.net/sprites/util-platform.png
    :alt: Moving Platform
    :align: left

Moving platforms ``util-platform`` are used to float players across the map and is used in the Airship map.
The platform's direction and offset can be viewed and adjusted in the object inspector.

.. note::

    When stepping on or off the platform, the player's collision is temporarily disabled to pass through walls.