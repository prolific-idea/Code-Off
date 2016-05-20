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
