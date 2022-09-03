Object Properties
=================

By selecting an object in the map, the properties panel will be populated with the properties of the selected object.
Different types of objects have different panels of properties.

Transform
--------------------------
All objects have a transform property that can be used to move, rotate, and scale the object.
You may also rename the object so it is easier to identify.

In addition, the transform panel provides a lock button that can be used to prevent the object from being dragged in the map.

Sprite
--------------------------
Most objects have a sprite property that can be used to change the image that is displayed on the object.
By hitting the ``Upload`` button, you can select an image to upload to the object.
If you hit the ``Reset`` button, the image will be reset to the default sprite.

Collider
--------------------------
Most objects have a collider property that can be used to change the shape of the object's collision.
By hitting ``Add Collider``, you can add a new collider to the object.
Selecting the collider from the list will edit the collider.

.. note::
    Depending on the object, some colliders may not interact with the player.
    For more information on collision, you may view :doc:`colliders`.

Task / Sabotage
--------------------------
Task and sabotage objects have a panel that can be used to view/edit some task/sabotage properties of the object.
Selecting a ``Room Utility`` from the dropdown will link the object to the ``Room Utility``.
In addition, you may change the task or sabotage's description that is displayed in-game.

For more information on ``Room Utilities``, you may view :doc:`custom-objs`.

Console
--------------------------
Tasks, sabotages, and other console objects have a console property that can be used to view/edit the player interaction with the object.
In addition, objects with a console will also have an orange ring displayed on the map to indicate the object's interaction zone.
You may increase/decrease the console's interaction range or make it only usable from below.

