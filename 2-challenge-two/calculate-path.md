# Calculate Path

Sincerest apologies to those who aren't maths fans...

## Coordinates Primer

In order to calculate the distance (c) from one coordinate (A) to another (B)

<img src="https://www.mathsisfun.com/algebra/images/dist-2-points-b.gif">

(from https://www.mathsisfun.com/algebra/distance-2-points.html)

You can use the following formula:

`a² + b² = c²`

For example the distance from (0, 0) to (12, 5), breaking down the problem would be:

1. `12² + 5² = c²`
2. `144 + 25 = c²`
3. `169 = c²`
4. `c = √169` - the square root of 169
5. `13` - the distance is 13

In an example where the start point isn't as simple as (0,0), you will first need to calculate the difference between the two coords...

For example, the direct distance between (11, 19) and (3, 4), broken down would be:

1. `(11, 19) - (3, 4) = (8, 15)` - take both x coords from each other (11 - 3 = 8), and then y coordinates from each other (19 - 4 = 15)
2. `8² + 15² = c²`
3. `64 + 225 = c²`
4. `289 = c²`
5. `c = √289`
6. `17` - the distance is 17

## Task

Your function should accept an array of tuples representing the coordinates of points on a map. Your function should return a calculation of the distance from "home", assuming it can take a direct path to each coordinate in turn.

The position of "home" is [0, 0] which is the starting point.

`[[15, 9], [3, 4]]` - the coords in each tuple array will always be placed in order of x, y respectively. i.e. 15 is x and 9 is y in the first coord in this example

Your function should also be calculating the total distance it has to take to get to the final destination, passing through each point in turn.

### Example outputs

`calculatePath([[12, 5]]) => 13` - since there is just one coordinate, the output is just simply 13

`calculatePath([[3, 4], [15, 9]]) => 18` - the path should take the distance to (3, 4), then calculate the distance from there to (15, 9), 13 again for a total distance of 18.

`calculatePath([[3, 4], [5, 6]]) => 8` - Your function should round to the nearest integer. The output here would be 5 + 2.82... ~> 8

## Hints

- as always start with what you know - you can build the initial input type you need for this example from the get go!
- then you can work your way up in complexity with TDD
