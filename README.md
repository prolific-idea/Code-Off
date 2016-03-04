# Code-Off
Code Off is an initiative that challenges developers to take 30 minutes off a Friday afternoon to work on something interesting with their peers. Code Off also aims to help developers expand their Github portfolio and collaborate with the development community. Each Friday afternoon at 15:30 CAT a new problem will be released on Github. Fork the repository, and get started.
The automated leaderboard is still in development. We encourage you to collaborate with other developers on Github.

#How to Participate?
Fork the Code Off repo and push your solution to your fork.

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

```
 ####*******#####
 #************#.#
 ####********####
 ###**###*****###
 ########*****###
 #.#.#####****#*#
 #.#.#.##***#***#
 ########.###****
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
