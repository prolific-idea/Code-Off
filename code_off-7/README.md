#Code Off #7 - Delivery Man

##Premise
You're a delivery man whose about to face a tough day in a maze.
You need to fetch an item from point marked with 1 and deliver it to the point marked with 2.

##Challenge
Your goal is to mark the path (.) from the starting point (@) to the first point (1), then mark the path (.) from the first point (1) to the final destination point (2).

##Legend
```
# = Wall
@ = Start point
1 = First destination
2 = Final destination
. = Path
```
##Constraints
* The width and height of the grid will always be the same.
* The width and height of the grid may be sized between 21x21 and 1021x1021.

##Details

###Input
An example input text file:

```
###################U#
2             #     #
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
#   #       # # #   1
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
2             #     #
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
#   #       # # #  .1
# ####### # ### ### #
# # # # # #   #   # #
# # # # ####### ### #
#       #       # # #
##### ##### # # # ###
#           # #     #
#####################

###################U#
2.........    #     #
# # ### #.# ### #####
# # # # #.#       # #
# # # ###.##### ### #
# # # #...    #   # #
##### #.######### # #
#    ...  # #       #
# # #.### # #########
# # #.  # #   #     #
# # #.####### ##### #
# # #...............#
##### ####### # ###.#
#   #       # # #  .1
# ####### # ### ### #
# # # # # #   #   # #
# # # # ####### ### #
#       #       # # #
##### ##### # # # ###
#           # #     #
#####################
```
Notice that the path from the starting location to the first destination is marked using the "." symbol, and in a second rendering, the path from the first destination to the final destination is marked with the "." symbol.
