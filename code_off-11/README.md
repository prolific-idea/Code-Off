# Code Off #11 - Battle Distress Call Decoding

## Premise
You and your team have received a message from one of your soldiers from a distant planet. Your team have a secret encoding for messages. It's Morse code with further obfuscation. You need to decode the message received and figure out what your soldier is trying to tell you.
See Code Off 10 for encoding the message.

## Challenge
Decode the message from an obfuscated string to Morse code, and then to an alphabet based sentence.
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
* Obfuscated Morse Code: 2/1A|B/2|A1/A|1A1|C|2A|A3|1A2|1
* Morse Code: ../.-|--/..|-./-|.-.|---|..-|-...|.-..|.
* Sentence: I AM IN TROUBLE

### Input
An example input text file:

```
4|1|1A2|1A2|C
2/1Q|B/2|A1/A|1A1|C|2A|A3|1A2|1
```

### Output
A text file in the following format:

```
HELLO
I AM IN TROUBLE
```
