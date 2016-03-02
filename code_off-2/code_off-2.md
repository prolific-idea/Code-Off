#Code Off #2

##Premise
You are given a number of liquids of different types and different quantities. You are also given a number of jars where each jar has a limited capacity and can only contain certain types of liquids. Liquids cannot be mixed. I.e. A jar can only contain one type of liquid.

##Challenge
Calculate the optimal distribution of liquids into jars such that the total remainder is minimised.

##Details

###Input
A text file in the following format:

```
3 //Number of available liquid types.
130	//Liters of type 0 liquid.
90 //Liters of type 1 liquid.
40 //Liters of type 2 liquid.
4 //Number of Jars
100,0,1 //Jar 0 can contain 100 liters of liquid type 0 and 1.
20,0 //Jar 1 can contain 20 liters of liquid type 0 only.
85,1,2 //Jar 2 can contain 85 liters of liquid type 1 and 2.
30,2 //Jar 3 can contain 30 liters of liquid type 2 only.
```

###Output
A text file in the following format:

```
40 //The total remainder liquid.
0,90 //Jar 0 contains 90 liters of liquid 0.
0,20 //Jar 1 contains 20 liters of liquid 0.
1,80 //Jar 2 contains 80 liters of liquid 1.
2,30 //Jar 3 contains 30 liters of liquid 2.
```
