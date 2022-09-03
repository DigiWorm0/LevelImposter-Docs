Other Objects
=================

In order to employ common features within Among Us, LevelImposter employs a variety of custom objects for you to use.
Unless otherwise specified, none of these objects are visible to the player in-game.

Room Utility
------------

.. image:: https://editor.levelimposter.net/sprites/util-room.png
    :alt: Room Utility
    :align: left

Room utilities ``util-room`` are used to create and manage rooms on the minimap and admin table.
Creating a room utility will result in the following behaviours:

- A name will be displayed on the minimap
- Entering the room's collider will display a popup with the room's name
- Players within the room's collider will be displayed on the admin table.

Each of these behaviours can be manually disabled by unchecking the appropriate checkbox in the inspector.

In addition to the above, the room utility can be used to link a task or sabotage to a specific room.
This will cause the task or sabotage to display the correct room name in the players' task list.

Star Field
----------

.. image:: https://editor.levelimposter.net/sprites/util-starfield.png
    :alt: Star Field
    :align: left

Star fields ``util-starfield`` allows you to create a star or cloud field in the background of your level.
It is particle system that spawns the current sprite at a random height within it's bounds.
The sprite will then move at a random speed between the min and max speed values.
A preview of the star field can be seen in the editor when the object is selected.

Ambient Sound
-------------

.. image:: https://editor.levelimposter.net/sprites/util-sound1.png
    :alt: Ambient Sound
    :align: left

Ambient sounds ``util-sound1`` are used to play a sound effect in the background of your level.
The sound will play continuously while the player is within the object's collider.
The sound will fade in and out as the player enters and exits the collision area.

Due to limitations in Unity, uploaded sounds must be mono or stereo WAV files in PCM format.

Step Sound
----------

.. image:: https://editor.levelimposter.net/sprites/util-sound2.png
    :alt: Step Sound
    :align: left

Step sounds ``util-sound2`` are used to play a stepping sound effect while the player is walking.
The sound will play a random step variant from the list of sounds provided while the player is walking.
Sound will only play if the player is within the object's collider.

The editor also provided a list of common sound presets used in the other Among Us maps including...

- Carpet
- Dirt
- Grass
- Metal
- Plastic
- Snow
- Tile
- Wood

Due to limitations in Unity, uploaded sounds must be mono or stereo WAV files in PCM format.

Spawnpoint
----------

.. image:: https://editor.levelimposter.net/sprites/util-spawn1.png
    :alt: Initial Spawnpoint
    :align: left

.. image:: https://editor.levelimposter.net/sprites/util-spawn2.png
    :alt: Meeting Spawnpoint
    :align: left

Spawnpoints ``util-spawn1`` and ``util-spawn2`` are used to set the initial spawnpoint and meeting spawnpoint respectively.
The initial spawnpoint is the location where players will spawn when they first start the game.
The meeting spawnpoint is the location where players will spawn after they are called to a meeting.

Players are spawned in a circular pattern around the spawnpoint as seen in the editor preview.

.. note::
    When using freeplay, the player will teleport to the meeting spawnpoint.

Minimap
-------

.. image:: https://editor.levelimposter.net/sprites/util-minimap.png
    :alt: Minimap
    :align: left

Minimaps ``util-minimap`` are used to set the minimap background image.
By default, the minimap will be completely blank with the exception of room names.
The minimap background image can be set to any image file supported by Unity.
Minimap scaling and position can be adjusted by moving the object or adjusting the minimap size in the inspector.

.. figure:: https://i.imgur.com/n8fFnd3.png
    :alt: Minimap Example
    :align: center

    Minimap Example

Uploaded image files should be primarily red and look like the impostor's sabotage map.
In order to properly scale each room, a download button of the minimap's current view is provided in the inspector.
The red, green, and blue channels will be swapped depending on whether the player is viewing their minimap, the sabotage map, or the admin table.

Dummy
-----

.. image:: https://editor.levelimposter.net/sprites/util-dummy.png
    :alt: Dummy
    :align: left

Dummies ``util-dummy`` are used as placeholder players in freeplay mode.
The game must contain at least 2 dummies in order to play as impostor in freeplay without automatically winning.
Dummies are automatically named and colored ``Player *``, regardless of what is set in the inspector.