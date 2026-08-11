PROBLEM STATEMENT: Valid Parentheses
Given a string s containing just the characters '(', ')', '{', '}', '[' and ']', determine if the input string is valid.

An input string is valid if:
Open brackets must be closed by the same type of brackets.
Open brackets must be closed in the correct order.
Every close bracket has a corresponding open bracket of the same type.
 
Example 1:
Input: s = "()"
Output: true

Example 2:
Input: s = "()[]{}"
Output: true

Example 3:
Input: s = "(]"
Output: false

Example 4:
Input: s = "([])"
Output: true

Example 5:
Input: s = "([)]"
Output: false

Constraints:
1 <= s.length <= 104
s consists of parentheses only '()[]{}'.

ALGORITHM:
1. Start.
2. Create an empty stack.
3. Go through each character in the string.
4. If the character is an opening bracket:
    Push it into the stack.
5. If the character is a closing bracket:
    Check whether the stack is empty.
    If empty → return False.
    Take the top opening bracket.
    Check whether it matches the closing bracket.
    If it doesn't match → return False.
    Otherwise remove the opening bracket.
6. After checking all characters:
    If the stack is empty → return True.
    Otherwise → return False.
7. Stop.

OUTPUT:
1. Input:
s = "()"
Output:
true
2. Input:
s = "(]"
Output: 
false