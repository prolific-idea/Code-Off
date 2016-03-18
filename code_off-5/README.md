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
The output file should be titled, "code_off-5-x.out", where x is the input text case number. The file should be located in the root of that specific code off directory.

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
