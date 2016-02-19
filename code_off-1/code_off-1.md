#Code Off #1

##Premise
* For this problem you're given a list of strings.
* An uppercase character is equal to its position in the alphabet (e.g. A = 1, B = 2, Z = 26)
* A lowercase character is equal to its position in the alphabet - 1 (e.g. a = 0, b = 1, z = 25)
* A string's value is determined by summing the characters of the string (e.g. Hi = 16)

##Challenge
* Determine which strings are equal in value.
* Determine which strings are palindromes.

##Details

###Constraints
* Each input string contains character between A-Z and a-z.

###Input
* A text file where the first line is an integer n. n indicates the number of strings in the list.
* Thereafter, each string is listed on a new line.

####Example
2

Hi

dbbbbd

###Output
* A text file in the following format:

for each string:

String

Is Palindrome?

List of equal strings

####Example
Hi

false

dbbbbd

dbbbbd

true

Hi