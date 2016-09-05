![Code Off](http://www.prolificidea.com/assets/img/code_off-logo.png "Code Off")

Code Off is an initiative that challenges developers to take 30 minutes off a Friday afternoon to work on something interesting with their peers. Code Off also aims to help developers expand their Github portfolio and collaborate with the development community. Each Friday afternoon at 15:30 CAT a new problem will be released on Github. Fork the repository, and get started.
The automated leaderboard is still in development. We encourage you to collaborate with other developers on Github.

http://www.prolificidea.com/codeoff.html

# How to Participate?
Fork the Code Off repo and push your solution to your fork.

# Code Off #13 - Gravitational Waves

## Premise
Gravitational waves have been making news headlines on the internet recently, with the second gravitational wave detected. What's gravitational waves? Imagine the universe being a giant trampoline, and space-time is the fabric. There are differences in dropping a bowling ball on the trampoline versus dropping a tennis ball. Gravitational waves form when large objects collide (E.g. two black holes colliding would theoretically cause a huge ripple). Gravitational waves were created when the Big Bang happened, they are important because they may hold answers to the origins of the universe. This [comic](http://www.phdcomics.com/comics.php?f=1853) explains gravitational waves quite well.

## Challenge
One of the challenges is detecting gravitational waves.
Let's try create an extremely primitive simulation of how one could possible detect gravitational waves by measuring incoming waves here on Earth.

This is a naive interpretation of the science, and is completely for interest sake.

Assume that the Earth is at the center of this plane.
```
0 0 0 0 0
0 0 0 0 0
0 0 x 0 0
0 0 0 0 0
0 0 0 0 0
```
Assume that there are varying gravitational wave intensities propagating from the edge of the plane.
```
6 4 3 2 1
1 0 0 0 5
2 0 x 0 3
7 0 0 0 4
1 9 8 7 6
```
Assume that each layer within the outer edge is impacted by the gravitational wave intensity of it's outer neighbors. Neighbors are outer cells adjacent or diagonally adjacent to the cell in question.
In the example below, the cell marked with x will be impacted by it's neighbors marked with #.
```
# # # 2 1
# x 0 0 5
# 0 0 0 3
7 0 0 0 4
1 9 8 7 6
```
This example represents a cell that is not at the edge.
```
6 # # # 1
1 0 x 0 5
2 0 0 0 3
7 0 0 0 4
1 9 8 7 6
```
The following function will be used to calculate the intensity of a space based on it's neighbors:
```
(Sum of all neighbor wave intensity / Number of neighbors) - 1
```

It assumes that the cell will inherit the average intensity of it's neighbors, -1 to account for loss in intensity.

Only integers will be used for the sake of simplicity. Use simple rounding for integers where x.1 - x.4 rounds down, and x.5 - x.9 rounds up.

### Process

This is the original state.
#### Original
```
6 4 3 2 1
1 0 0 0 5
2 0 0 0 3
7 0 0 0 4
1 9 8 7 6
```
#### Iteration 1
The next layer of cells is calculated based on the function.
```
6 4 3 2 1
1 2 2 2 5
2 2 0 3 3
7 4 7 5 4
1 9 8 7 6
```
#### Iteration 2
Finally, the center intensity is calculated. It shows that even though there may be varying forces incoming, on Earth, we may not detect or feel much.
```
6 4 3 2 1
1 2 2 2 5
2 2 2 3 3
7 4 7 5 4
1 9 8 7 6
```
### Input
* The number of rows and columns in the input file will always be the same.
* The number of rows and columns in the input file will always be an odd number.
* The initial intensities may be any integer less than or equal to 100;

```
6 4 3 2 1
1 0 0 0 5
2 0 0 0 3
7 0 0 0 4
1 9 8 7 6
```
Feel free to make your own experiment input files and share them with the community.

### Output
The output will represent how gravitational waves could possible propagate to a center whilst diminishing in intensity.

```
6 4 3 2 1
1 2 2 2 5
2 2 2 3 3
7 4 7 5 4
1 9 8 7 6
```
