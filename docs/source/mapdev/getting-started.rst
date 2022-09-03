Getting Started
=================

Using the Editor
--------------------------
LevelImposter utilizes `LevelImposter Editor <https://editor.levelimposter.net/>`_ to create and edit maps.
The editor is a web application that allows you to create maps and save them as .LIM files or publish them to the LevelImposter API.
The LIM files are parsed by the `LevelImposter Mod <https://github.com/DigiWorm0/LevelImposter/releases>`_ in order to load the map into the game.

Creating a Map
^^^^^^^^^^^^^^^^^^^^^

Launching the editor will create a new map for you.
Maps are local to your browser and are not saved to the server.
You can save your map to a file by clicking the ``Save`` button in the top right corner.

You may add objects to the map by clicking on the ``Add Object`` button.
The editor will then open a new window that allows you to select the object you want to add.

Object Types
^^^^^^^^^^^^

LevelImposter includes a variety of different types of objects including...

- Tasks ``task-*``
- Utilities ``util-*``
- Sabotages ``sab-*``
- Decorations ``dec-*``
- Room Backgrounds ``room-*``

Each object has a name (``Admin Table``) and a unique type ID (``util-admin``).
The ID is used to identify the object in the map file and is used by the mod to load the object into the game.
You can either search for objects, by their type or their name.

Alternatavely, you can also add ``util-blank`` objects by just typing your own object name into the search bar.

.. note::

    Right click will move your camera, left click will move/select an object.

Inspector Panel
^^^^^^^^^^^^^^^

Once an object is selected, the inspector panel will open on the right side of the screen.
Depending on the object selected, this panel allows you to edit the properties of the selected object including...

- Name
- Position
- Rotation
- Scale
- Sprite
- Collider
- Others (depending on the object type)

In addition, you may lock the object to prevent it from being moved accidentally.
For more information about the various object properties, you can view :doc:`edit-properties`.

Scene Panel
^^^^^^^^^^^

The scene panel is located on the left side of the screen and allows you to view and edit each object in the map.
Each object is represented by a small icon, a name, and an icon to show or hide the object.