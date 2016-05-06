![Code Off](http://www.prolificidea.com/assets/img/code_off-logo.png "Code Off")

Code Off is an initiative that challenges developers to take 30 minutes off a Friday afternoon to work on something interesting with their peers. Code Off also aims to help developers expand their Github portfolio and collaborate with the development community. Each Friday afternoon at 15:30 CAT a new problem will be released on Github. Fork the repository, and get started.
The automated leaderboard is still in development. We encourage you to collaborate with other developers on Github.

http://www.prolificidea.com/codeoff.html

# How to Participate?
Fork the Code Off repo and push your solution to your fork.

# Notice
The leaderboard is currently outdated and we're in the process of automating and updating it.
Please send through any suggestions to info[at]prolificidea[dot]com

# Code Off #10 - Battle Distress Call

## Premise
You're competing in a battle on a far away planet and you're in some trouble. You need to send a distress call to your home base for reinforcements, however, enemy agents are listening. Luckily your team have a secret encoding for messages. It's Morse code with further obfuscation.

## Challenge
Translate the alphabet based sentence to Morse code, then, obfuscate the Morse code.
Below is the international Morse code translations. Separate letters with pipe (|), and separate words with forward slash (/).

### International Morse Code
* A .-
* B -...
* C -.-.
* D -..
* E .
* F ..-.
* G --.
* H ....
* I ..
* J .---
* K -.-
* L .-..
* M --
* N -.
* O ---
* P .--.
* Q --.-
* R .-.
* S ...
* T -
* U ..-
* V ...-
* W .--
* X -..-
* Y -.--
* Z --..
* 0 -----
* 1 .----
* 2 ..---
* 3 ...--
* 4 ....-
* 5 .....
* 6 -....
* 7 --...
* 8 ---..
* 9 ----.
* Fullstop .-.-.-
* Comma --..--

### Obfuscation
For obfuscation, your team decided to replace the number of consecutive dots with a number, and replace the number of consecutive dashes with the letter of the alphabet at that position. E.g. S = ... = 3, Q = --.- = b1a, F = ..-. = 2a1.

### Example
Sentence: I AM IN TROUBLE
Morse Code: ../.-|--/..|-./-|.-.|---|..-|-...|.-..|.
Obfuscated Morse Code: 2/1A|B/2|A1/A|1A1|C|2A|A3|1A2|1

### Input
An example input text file:

```
HELLO
I AM IN TROUBLE
```

### Output
A text file in the following format:

```
4|1|1A2|1A2|C
2/1Q|B/2|A1/A|1A1|C|2A|A3|1A2|1
```
