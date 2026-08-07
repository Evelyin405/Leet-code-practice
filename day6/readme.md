PROBLEM STATEMENT: 7. Reverse Integer
Given a signed 32-bit integer x, return x with its digits reversed. If reversing x causes the value to go outside the signed 32-bit integer range [-231, 231 - 1], then return 0.

Assume the environment does not allow you to store 64-bit integers (signed or unsigned).

Example 1:
Input: x = 123
Output: 321

Example 2:
Input: x = -123
Output: -321

Example 3:
Input: x = 120
Output: 21
 

Constraints:
-231 <= x <= 231 - 1

Algorithm: 
1. Start.
2. Read integer x.
3. Store its sign (1 for positive, -1 for negative).
4. Convert x to its absolute value.
5. Initialize reverse = 0.
6. While x > 0:
   Find the last digit using digit = x % 10.
   Update reverse = reverse * 10 + digit.
   Remove the last digit using x = x // 10.
7. Multiply reverse by the original sign.
8. If the result is outside the range -2³¹ to 2³¹ - 1, return 0.
9. Otherwise, return the reversed number.
10. Stop.

Input:
x = 123
Output: 
321