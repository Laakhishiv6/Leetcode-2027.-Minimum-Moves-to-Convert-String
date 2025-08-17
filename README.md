# Leetcode-2027.-Minimum-Moves-to-Convert-String
# Description
You are given a string s consisting of n characters which are either 'X' or 'O'.

A move is defined as selecting three consecutive characters of s and converting them to 'O'. Note that if a move is applied to the character 'O', it will stay the same.

Return the minimum number of moves required so that all the characters of s are converted to 'O'.
# Solution
In the given problem we have been given a string s which consists of 'X' and 'O' characters , we need to convert the given string in such a way that all the characters would be 'O'.

Rules:
1. If character =='X': Convert it to 'O'
2. If character =='O': It remains the same

Example 1:

Input: s = "XXX"

Output: 1

Explanation: XXX -> OOO

We select all the 3 characters and convert them in one move.

Example 2:

Input: s = "XXOX"

Output: 2

Explanation: XXOX -> OOOX -> OOOO

We select the first 3 characters in the first move, and convert them to 'O'.
Then we select the last 3 characters and convert them so that the final string contains all 'O's.

Example 3:

Input: s = "OOOO"

Output: 0

Explanation: There are no 'X's in s to convert.

Intuition:
a. Initialise a variable move for counting the number of steps to convert the given string.
b. If the character is X then we can increment the move by 1 and directly Skip the next 3 characters by doing i += 3.
c. If the current character s[i] is 'O', simply move to the next character by doing i += 1.
# Algorithm
1. 

