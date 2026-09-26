PROBLEM STATEMENT : CONTAINS DUPLICATE

Given an integer array nums, return true if any value appears at least twice in the array, and return false if every element is distinct.

Example 1:
Input: nums = [1,2,3,1]
Output: true

Explanation:
The element 1 occurs at the indices 0 and 3.

Example 2:
Input: nums = [1,2,3,4]
Output: false

Explanation:
All elements are distinct.

Example 3:
Input: nums = [1,1,1,3,3,4,3,2,4,2]
Output: true

Constraints:

1 <= nums.length <= 105
-109 <= nums[i] <= 109

ALGORITHM: 
Step 1: Start with the given integer array nums.
Step 2: Convert the array into a set. A set stores only unique elements.
Step 3: Compare the length of the original array with the length of the set.
Step 4:
If both lengths are different, a duplicate exists → return True.
If both lengths are the same, all elements are distinct → return False.
Step 5: Stop.

Sample I/O: 
Input:
nums = [1, 2, 3, 1]
Output:
True

Input:
nums = [1, 2, 3, 4]
Output:
False