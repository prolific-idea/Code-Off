![Code Off](http://www.prolificidea.com/assets/img/code_off-logo.png "Code Off")

Code Off is an initiative that challenges developers to take 30 minutes off a Friday afternoon to work on something interesting with their peers. Code Off also aims to help developers expand their Github portfolio and collaborate with the development community. Each Friday afternoon at 15:30 CAT a new problem will be released on Github. Fork the repository, and get started.
The automated leaderboard is still in development. We encourage you to collaborate with other developers on Github.

http://www.prolificidea.com/codeoff.html

# How to Participate?
Fork the Code Off repo and push your solution to your fork.

# Notice
The leaderboard is currently outdated and we're in the process of automating and updating it.
Please send through any suggestions to info[at]prolificidea[dot]com

# Code Off #12 - Card Hands

## Premise
You are analysing an obscure card game named Thunee. You would like to find all the variations of hands that each player could potentially get after the first deal.

## Challenge
The game uses only a subset of a deck of cards. The exact cards are listed below. Each player gets dealt 4 cards each, then an additional 2 cards each, starting at the same player as the first deal.

### Cards in Thunee Deck
C = Clubs
D = Diamonds
H = Hearts
S = Spades
J = Jack
K = King
Q = Queen
x = Ranked Card

* JC, 9C, 1C, 10C, KC, QC
* JD, 9D, 1D, 10D, KD, QD
* JH, 9H, 1H, 10H, KH, QH
* JS, 9S, 1S, 10S, KS, QS

### Input
The input file may contain any card in a 52 card deck of playing cards.

```
JC 
9C 
1C 
10C 
KC 
QC
JD
9D
1D
10D
KD
QD
JH
9H
1H
10H
KH
QH
JS
9S
1S
10S
KS
QS
```

### Output
The output file will contain each possibility of cards for each player after the first deal.
Cards are separated by "," and player's hands are separated by "|".

```
JC,1C,QC,JS|10H,QH,QS,QD|JH,JD,1S,1D|9S,KH,KC,9D
...
```
