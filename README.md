# Day25-50-days-coding-challenge

🔸 Problem 1: Implement Stack using Queues
📌 Problem Statement:
Design a stack (LIFO) using two queues (FIFO). Only standard queue operations are allowed:

enqueue (push to back)

dequeue (pop from front)

peek

size

isEmpty

📌 Constraints:

1 <= x <= 9

At most 100 operations on the stack

All pop() and top() calls are valid

📌 Implemented Methods:

push(x)

pop()

top()

empty()

📌 Approach:

Use two queues (q1 and q2)

On push, enqueue to q2, and move all from q1 to q2, then swap queues

top() and pop() always from front of q1

📌 Example:

text
Copy
Edit
MyStack myStack = new MyStack();
myStack.push(1);
myStack.push(2);
myStack.top();    // returns 2
myStack.pop();    // returns 2
myStack.empty();  // returns False
🔸 Problem 2: Rotate Array
📌 Problem Statement:
Given an integer array nums, rotate the array to the right by k steps in-place.

📌 Constraints:

1 <= nums.length <= 10⁵

0 <= k <= 10⁵

-2³¹ <= nums[i] <= 2³¹ - 1

📌 Approach:

Use reverse-based rotation:

Reverse entire array

Reverse first k elements

Reverse the remaining elements

Handles large k using k = k % len(nums)
📌 Example:
Input: nums = [1,2,3,4,5,6,7], k = 3
Output: [5,6,7,1,2,3,4]
📌 Time Complexity: O(n)
📌 Space Complexity: O(1)

📌 Topics Covered:
Stack Simulation

Queue Mechanics

Array Manipulation
In-Place Algorithms

Leetcode

