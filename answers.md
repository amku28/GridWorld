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


Part 2
1. The sideLength is the length of the box that the bug makes + 1.
2. The steps are used to count the amount of places the bug has traveled.
3. The turn method is called twice because one turn of the bug turns the bug 45 degrees to the right while a full turn requires a 90 degree turn.
4. The move function is able to be called because the BoxBug class extends the Bug class.
5. No, we can control the size of the square pattern with an input into the constructor.
6. No, it will always move North first, then East, then South, then West because the bug is defaulted to turn to the right. The only way to make it travel differently is to make it turn to the left through six turns rather than two.
7. The value will be zero when the bug has finished one side of the square pattern.

Exercises
1. The CircleBug runs in circles rather than boxes.
5. To add another BoxBug to the actor grid, I would have to first construct it using the basic constructor: Boxbug name = new BoxBug(sidelength of box). After, if I wanted to, I can set the color using the method: name.setColor(Color.ORANGE). To put the bug on the grid, I call the method: world.add(new Location(x, y), name).


Part 3
Location
1. loc1.getRow();
2. false
3. loc3 = new Location(4, 4);
4. int dir = 135
5. The getAdjacentLocation method requires a direction in the input. For example, you would need to input getAdjacentLocation(Location.Direction), where the direction is a direction on the compass.

Grid
1. Arraylist<Location> getEmptyAdjacentLocations(Location loc);
2. boolean isValid(Location 10, 10);
3. Grid implements comparable. These can be found in the complarable class.
4. It depends. Arrays can be better when integers are being used however, if the data type is unpredictable then ArrayList would be better.

Actor
1. Color, Direction, and Location
2. North, blue
3. Because there are other objects that extend the Actor class.
4. No, an actor must remove itself before putting itself back into a grid. No an actor cannot removes itself from a grid twice. Not exactly, once the actor is removed, a new actor must be placed therefore, once an actor is removed it is essentially erased.
5. setDirection(int newDirection);

Extending Actor
1. The canMove method uses the getAdjacentLocation method to check if it is next to the edge of the grid. If the bud is on the edge, the method will then return false.
2. The last line where it checks the neighboring actor. If the actor is anything other than a flower or empy location then it will return false.
3. It calls the getGrid().
4. getLocation(), getAdjacentLocation().
5. The getDirection().
6. The bug will remove itself from the grid.
7. No it's not needed but it makes things more organized and easier to read.
8. In the move method, the flower that is dropped gets the color from the bug using the getColor method.
9. No.
10. flower.putSelfInGrid(gr, loc);
11. It should be called four times because each turn is 45 degrees.

Group Activity
1) 
a. The jumper will jump to the location in front that is empty.
b. The jumper will only jump to the location in front.
c. The jumper will turn 90 degrees to the right until it finds an open location.
d. It would check if the cell in front is empty then jump one cell then it would skip the actor.
e. It would treat the jumper like any other actor.
f. No.

2)
a. It would extend the bug class
b. Yes the bug class.
c. Yes it would need a color and direction
d. No.
e. canJump() & jump() & turn90();
f. Test all scenarios.
