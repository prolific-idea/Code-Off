#Code Off #6 - Shortest Coffee Run

##Premise
You're trapped in a maze and need to escape to get to the closest cup of coffee.

##Challenge
Your goal is to mark the shortest path (.) from the starting point (@) to the coffee (U)

##Legend
```
# = Wall
@ = Start point
U = Coffee
. = Path to exit
```
##Constraints
* The width and height of the grid will always be the same.
* The width and height of the grid may be sized between 21x21 and 1021x1021.
* The number of cups (U) may be between 1 and 10.

##Details

###Input
An example input text file:

```
###################U#
U             #     #
# # ### # # ### #####
# # # # # #       # #
# # # ### ##### ### #
# # # #       #   # #
##### # ######### # #
#         # #       #
# # # ### # #########
# # #   # #   #     #
# # # ####### ##### #
# # #     @         #
##### ####### # ### #
#   #       # # #   U
# ####### # ### ### #
# # # # # #   #   # #
# # # # ####### ### #
#       #       # # #
##### ##### # # # ###
#           # #     #
#####################
```

###Output
A text file in the following format.

```
###################U#
U             #     #
# # ### # # ### #####
# # # # # #       # #
# # # ### ##### ### #
# # # #       #   # #
##### # ######### # #
#         # #       #
# # # ### # #########
# # #   # #   #     #
# # # ####### ##### #
# # #     @.........#
##### ####### # ###.#
#   #       # # #  .U
# ####### # ### ### #
# # # # # #   #   # #
# # # # ####### ### #
#       #       # # #
##### ##### # # # ###
#           # #     #
#####################
```
Notice that the path from the starting location to the closest cup of coffee is marked using the "." symbol.
