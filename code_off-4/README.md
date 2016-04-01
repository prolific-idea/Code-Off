#Code Off #4 - Water Source for Barry's Friends

##Premise
Based on Code Off #3 - we tried to find the largest water source for Barry. If you haven't looked at the previous code off, we strongly suggest you fork it and try solve it first.
Barry became lonely, he needs his friends with him. We need to try create a large enough water source for Barry and his friends.
You are given a grid of characters representing walls and water.
The walls divide the water sources into differently sized sections.
You would like to find the least number of walls to break to connect all water sources.

##Challenge
Your goal is to find the least number of walls to break to connect all water sources and mark those walls.

##Legend
```
# = Wall
. = Water
* = Marked as a broken wall to connect all water sources
```
##Constraints
* The width and height of the grid will always be the same.
* The width and height of the grid may be sized between 16x16 and 1024x1024.

##Details

###Input
An example input text file:

```
 ####.......#####
 #............#.#
 ####........####
 ###..###.....###
 ########.....###
 #.#.#####....#.#
 #.#.#.##...#...#
 ########.###....
 ######.#####...#
 #####..###..####
 ###......#######
 #.#.....########
 #..##...######.#
 #...########...#
 #.....####.....#
 ###.########.###
```

###Output
A text file in the following format. The output file should be titled, "code_off-4-x.out", where x is the input text case number. The file should be located in the root of that specific code off directory.

```
 ####.......#####
 #............#.#
 ####........####
 ###..###.....###
 ###*####.....###
 #.#.#####....#.#
 #.*.*.##...#...#
 ######**.###....
 ######.####*...#
 #####..###..##*#
 ###......#####*#
 #.#.....######*#
 #..*#...######.#
 #...########...#
 #.....####.....#
 ###.########.###
```
Notice that the walls to be broken to connect all sections of water is marked by replacing the '#' character with '*'.
