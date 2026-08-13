PROBLEM STATEMENT : PLUS ONE

You are given a large integer represented as an integer array digits, where each digits[i] is the ith digit of the integer. The digits are ordered from most significant to least significant in left-to-right order. The large integer does not contain any leading 0's.
Increment the large integer by one and return the resulting array of digits.

Example 1:
Input: digits = [1,2,3]
Output: [1,2,4]
Explanation: The array represents the integer 123.
Incrementing by one gives 123 + 1 = 124.
Thus, the result should be [1,2,4].

Example 2:
Input: digits = [4,3,2,1]
Output: [4,3,2,2]
Explanation: The array represents the integer 4321.
Incrementing by one gives 4321 + 1 = 4322.
Thus, the result should be [4,3,2,2].

Example 3:
Input: digits = [9]
Output: [1,0]
Explanation: The array represents the integer 9.
Incrementing by one gives 9 + 1 = 10.
Thus, the result should be [1,0].
 
Constraints:
1 <= digits.length <= 100
0 <= digits[i] <= 9
digits does not contain any leading 0's.

ALGORITHM:
1. Start from the last index of the array.
2. Add 1 to the last digit.
3. If the digit becomes less than 10, return the array.
4. If the digit becomes 10, make it 0 and carry 1.
5. Move to the previous digit.
6. Continue until you find a digit that is not 9.
7. Increase that digit by 1.
8. If all digits were 9, create a new array with 1 at the beginning and 0s after it.

Sample I/O:
1. Input:
digits = [1,2,3]
Output: [1,2,4]
2. Input:
digits = [4,3,2,1]
Output:
[4,3,2,2]
 
