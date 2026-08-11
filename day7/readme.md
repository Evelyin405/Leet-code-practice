PROBLEM STATEMENT: Length of Last Word
Given a string s consisting of words and spaces, return the length of the last word in the string.
A word is a maximal substring consisting of non-space characters only.

 
Example 1:
Input: s = "Hello World"
Output: 5
Explanation: The last word is "World" with length 5.

Example 2:
Input: s = "   fly me   to   the moon  "
Output: 4
Explanation: The last word is "moon" with length 4.

Example 3:
Input: s = "luffy is still joyboy"
Output: 6
Explanation: The last word is "joyboy" with length 6.
 
Constraints:
1 <= s.length <= 104
s consists of only English letters and spaces ' '.
There will be at least one word in s.

Algorithm: 
Input: A string s containing words and spaces
Output: Length of the last word

1. Start
2. Read the string s.
3. Split the string into separate words using split().
4. Find the last word using [-1].
5. Find the length of the last word using len().
6. Return the length.
7. Stop

Input: 
s = "   fly me   to   the moon  "
Output: 
4