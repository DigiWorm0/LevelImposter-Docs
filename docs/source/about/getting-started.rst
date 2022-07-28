Getting Started
=================

Install the Among Us Mod
--------------------------
If you just want to play maps, all you need to do is install the mod.
If you are insterested in making maps, you can check out Map Development's :doc:`mapdev/mapdev-start`.
Either you can let a mod loader do the work for you, or you can manually install the dll yourself.

Automatic Method
^^^^^^^^^^^^^^^^^^

**1. Download a mod loader** (if you haven't already)

Various mod loaders are available such as `Mod Manager <https://github.com/MatuxGG/ModManager>`_ by Matux.

**2. Download LevelImposter**

Once you have the mod loader downloaded and installed, you can select LevelImposter among it's list of mods.
Everything else will be done automatically.

**3. Profit?**

If LevelImposter is successfully installed, you should see the LevelImposter logo in the top left corner as well as a "Maps" button on the main menu screen.
Once you have successfully installed, you may :ref:`select-map`.

Manual Method
^^^^^^^^^^^^^^^

**1. Verify your Among Us version**

LevelImposter will only support the version it is currently built for. You can view *(as well as download)* the latest build of LevelImposter is available `here <https://github.com/DigiWorm0/LevelImposter/releases>`_.

**2. Download the latest BepInEx** (if you haven't already)

The latest build of BepInEx is available `here <https://builds.bepinex.dev/projects/bepinex_be>`_.
Download the version that lists ``BepInEx_UnityIL2CPP_x86_....zip`` and unzip it into your Among Us folder.

- **Steam** - ``C:/Program Files (x86)/Steam/steamapps/common/Among Us/``
- **Epic** - ``C:/Program Files/Epic Games/Among Us/``

**3. Launch Among Us then close it again**

Among Us will take longer than usual while BepInEx does it's thing

**4. Download the latest LevelImposter**

The latest build of LevelImposter is available `here <https://github.com/DigiWorm0/LevelImposter/releases>`_.
Download the file that lists ``LevelImposter-x.x.x.dll`` and drop it into the BepInEx plugins folder.

- **Steam** - ``C:/Program Files (x86)/Steam/steamapps/common/Among Us/BepInEx/plugins/``
- **Epic** - ``C:/Program Files/Epic Games/Among Us/BepInEx/plugins/``

**5. Profit?**

If LevelImposter is successfully installed, you should see the LevelImposter logo in the top left corner as well as a "Map Shop" button on the main menu screen.

.. _select-map:

Play on a Map
---------------

Once you have installed LevelImposter, you can open the Maps menu on the main menu screen.
The Maps menu will display 3 tabs: ``Downloaded``, ``Latest``, and ``Search``.

    - ``Downloaded`` - A list of maps that you have downloaded.
    - ``Latest`` - A list of maps that are available on the server.
    - ``Search`` - A search bar that allows you to search for maps.

Once you have a map downloaded, you can either launch the map in freeplay or start a new lobby to play your map with friends.
You may select any downloaded map within the lobby menu. The map will automatically download and syncronize to all players.

.. note::

    Using LevelImposter in public lobbies requires all members of the lobby to have the LevelImposter mod installed.
