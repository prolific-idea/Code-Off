#Code Off #9 - Bomberman: Aftermath

##Premise
With reference to the [Entelect Challenge](http://challenge.entelect.co.za).
You're bomberman. You're given a block of walls that have been exploded. You need to determine the sequence of bombs used to destory the walls.
Please see Code Off #8 as a reference.

##Challenge
The radius of walls destroyed by a bomb is specified by the number on the bomb. Each bomb explodes verically and horizontally, but never diagonally. If a bomb is adjacent to another bomb (vertically, horizontally, or diagonally) it's radius increases by 1 for each adjacent bomb.
Determine the position and radius of the bombs by marking them on the map.

##Legend
```
# = Wall
x = A number indicating the radius of the bomb
* = Destroyed wall
```
##Constraints
* The width and height of the grid will always be the same.
* The width and height of the grid may be sized between 16x16 and 1021x1021.

##Details

###Input
An example input text file:

```
################
################
#####*####*#####
#####*####*#####
###*****##*#####
#####*#*******##
#####**###*#####
###*****##*#####
####*****#*#####
#####**#########
######*#########
################
################
################
################
################
```

###Output
A text file in the following format:

```
################
################
################
################
#####2##########
##########3#####
################
#####1##########
######1#########
################
################
################
################
################
################
################
```
Notice that the bombs are placed in positions and with radius' that will result in the final explosion.
