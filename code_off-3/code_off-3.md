#Code Off #3 - Water Source for Barry

##Premise
You are given a grid of characters representing walls and water.
The walls divide the water sources into differently sized sections.
You would like to find the largest water source section for your pet shark, Barry.

##Challenge
Your goal is to find the largest water source in the grid and mark it as the largest.
If there are two or more water sources of the same size, mark all of them.

##Legend
```
# = Wall
. = Water
* = Marked as part of the largest water source section
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
By looking at the above example, it's clear that the top most portion of the grid contains the largest water source.

###Output
A text file in the following format.
The output file should be titled, "code_off-3-x.out", where x is the input text case number.

```
 ####*******#####
 #************#.#
 ####********####
 ###**###*****###
 ########*****###
 #.#.#####****#*#
 #.#.#.##***#***#
 ########*###****
 ######.#####***#
 #####..###..####
 ###......#######
 #.#.....########
 #..##...######.#
 #...########...#
 #.....####.....#
 ###.########.###
```
Notice that the largest section of water is marked by replacing the '.' character with '*'.
