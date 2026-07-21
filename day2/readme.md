PROBLEM STATEMENT:  Palindrome Number
    Given an integer x, return true if x is a palindrome, and false otherwise.

 
Example 1:
Input: x = 121
Output: true
Explanation: 121 reads as 121 from left to right and from right to left.

Example 2:
Input: x = -121
Output: false
Explanation: From left to right, it reads -121. From right to left, it becomes 121-. Therefore it is not a palindrome.

Example 3:
Input: x = 10
Output: false
Explanation: Reads 01 from right to left. Therefore it is not a palindrome.
 

 ALGORITHM: 
1. Start.
2. Read the integer x.
3. If x is less than 0, return False.
4. Store the original number in a variable original.
5. Initialize reverse = 0.
6. Repeat while x > 0:
   Find the last digit using digit = x % 10.
   Append the digit to reverse using reverse = reverse * 10 + digit.
   Remove the last digit from x using x = x // 10.
7. Compare original and reverse.
8. If they are equal, return True.
9. Otherwise, return False.
10. Stop.

Input:
x = 121
Output:
true