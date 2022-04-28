Mod Framework
===================

At the core of LevelImposter is the BepInEx Among Us mod that...

1. Downloads map data from the LevelImposter API
2. Deserializes and builds each map element
3. Syncronizes map data among all lobby members

Information on downloading and installing the mod is available at :doc:`getting-started`.

.. note::

   Source code for the mod is available on `GitHub <https://github.com/DigiWorm0/LevelImposter>`_.

Framework
-----------
The LevelImposter mod is made up of several namespaces that have different jobs:

* **LevelImposter.Shop** - Manages the map shop at the main menu
* **LevelImposter.DB** - Searches and maintains a database of Among Us sprites, prefabs, and components
* **LevelImposter.Core** - Builds the map from map data