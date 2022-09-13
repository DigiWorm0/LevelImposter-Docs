Colliders
=================

In order to enable collision between the player and walls and other objects, colliders must be built by the map developer.

Editing
-------

Most object in the game have a collider panel in the object inspector.
Colliders can be added, removed, and edited from this panel.

Each collider has the following properties:

- **Is Solid** - If this is checked, the inside of the collider will be completely solid and un-navigable. This is primarily used if the object cannot be walked inside of such as a table or a chair.
- **Blocks Light** - If this is checked, the edges of the collider will block the player's vision from passing through.
- **Points** - This is a list of points that make up the collider. The points are in local coordinates, so if the object is moved, the collider will move with it.

Points can be added by clicking on the collider's edge.
Points can be removed by right clicking on the point itself.
Points can be moved by dragging them around.

By default, the points will follow the map's grid, but this can be disabled by unchecking the "Snap to Grid" option or doing `Ctrl + G`.

Trigger Objects
---------------

Some objects such as rooms ``util-room`` and sounds ``util-sound*`` do not actually collide with the player itself.
Instead, they are used to detect the precense or absence of the player.
As a result, the solid and light blocking properties are not used for these objects.

Best Practices
--------------
For the best results, it is recommended that you follow :doc:`/mapdev/best-practices` when creating your colliders.