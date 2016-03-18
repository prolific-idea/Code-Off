#Code Off #5 - Maze Runner

##Premise
You're trapped in a maze and need to escape to get to your coffee.

##Challenge
Your goal is to mark a path (.) from the starting point (@) to the coffee (U)

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

##Details

###Input
An example input text file:

```
###################U#
#             #     #
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
#   #       # # #   #
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
#        ...  #.....#
# # ### #.#.###.#####
# # # # #.#.....  # #
# # # ###.##### ### #
# # # #...    #   # #
##### #.######### # #
#    ...  # #       #
# # #.### # #########
# # #.  # #   #     #
# # #.####### ##### #
# # #.....@         #
##### ####### # ### #
#   #       # # #   #
# ####### # ### ### #
# # # # # #   #   # #
# # # # ####### ### #
#       #       # # #
##### ##### # # # ###
#           # #     #
#####################
```
Notice that the path from the starting location to the coffee cup is marked using the "." symbol.
