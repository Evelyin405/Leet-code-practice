PROBLEM STSTEMENT: 
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
You may assume that each input would have exactly one solution, and you may not use the same element twice.
You can return the answer in any order.

 Example 1:
Input: nums = [2,7,11,15], target = 9
Output: [0,1]
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].

Example 2:
Input: nums = [3,2,4], target = 6
Output: [1,2]

Example 3:
Input: nums = [3,3], target = 6
Output: [0,1]
 

Constraints:

2 <= nums.length <= 104
-109 <= nums[i] <= 109
-109 <= target <= 109

ALGORITHM : 
1. Start.
2. Traverse the array using the first loop (i).
3. For each element, use a second loop (j) starting from the next index (i + 1).
4. Check if the sum of nums[i] and nums[j] is equal to the target.
5. If the sum matches the target, return the indices [i, j].
6. Stop after finding the required pair.