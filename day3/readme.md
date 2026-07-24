 PROBLEM STATEMENT: 
 Longest Substring Without Repeating Characters

Given a string s, find the length of the longest substring without duplicate characters.

 Example 1:
Input: s = "abcabcbb"
Output: 3
Explanation: The answer is "abc", with the length of 3. Note that "bca" and "cab" are also correct answers.

Example 2:
Input: s = "bbbbb"
Output: 1
Explanation: The answer is "b", with the length of 1.

Example 3:
Input: s = "pwwkew"
Output: 3
Explanation: The answer is "wke", with the length of 3.
Notice that the answer must be a substring, "pwke" is a subsequence and not a substring.


ALGORITHM:
1. Start.
2. Create an empty set to store unique characters.
3. Initialize:
     left = 0
     maxLength = 0
4. Traverse the string using right.
5. If s[right] is already in the set:
    Remove s[left] from the set.
    Increment left.
    Repeat until the duplicate is removed.
6. Add s[right] to the set.
7. Calculate the current window length:
    right - left + 1
8. Update maxLength.
9. Return maxLength.
10. Stop.

Input:
s = "abcabcbb"
Output: 
3
 