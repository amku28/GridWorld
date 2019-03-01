Part 1
1. No, the bug may use a step to rotate itself to the right if something is in its way in order to get around the obstacle.
2. The bug will always move in the direction it's facing.
3. It will rotate.
4. The bug leaves behind a flower.
5. When the bug is at the edge of the grid, if it's facing towards the edge the bug will rotate to the right until an open path is available at which point it will move until something else gets in the bug's way.
6. The bug will turn 45 degrees to the right each step until it finds an open path.
7. No.
8. The flower changes color each step once set from red until it's like a dark blue/black color. Once the bug overlaps the flower, the color turns red again and the process is restarted.
9. No, it's just a rock.
10. Yes, all the actors can be in the same location in the grid at the same time. However, if the bug is placed in the same place as a rock, the rock will be replaced with a flower.
Exercises
1. 
Degrees | Compass Direction
0       | North
45      | Northeast
90      | East
135     | Southeast
180     | South
225     | Southwest
270     | West
315     | Northwest
360     | North
2. The bug can be moved in any direction, within the bounds of the grid. When i try to move the bug outside fo the grid, an illegal argument exception shows up preventing the bug from moving.
3. setColor(java.awt.Color)
4. The bug goes poof.