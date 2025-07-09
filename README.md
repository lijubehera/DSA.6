🔁 𝗗𝗮𝘆 𝟲 𝗼𝗳 hashtag#𝗗𝗦𝗔 𝗟𝗲𝗮𝗿𝗻𝗶𝗻𝗴 | 

✅ Problem Solved: Remove Duplicates from Sorted Array II

 🔗 LeetCode Profile – https://lnkd.in/dRAYke5d

Today, I leveled up from yesterday’s problem by tackling a medium variation where each unique element is allowed at most twice — not once!

🧩 Problem Overview:
 Given a sorted array, modify it in-place such that each unique element appears at most twice. Return the new length after duplication removal, ensuring the relative order is maintained.

Example:
 Input: [1,1,1,2,2,3]
 Output: Length = 5, Modified = [1,1,2,2,3,_]
🧠 Approach I Used:
 Still used the two-pointer technique but with a slight twist:
The first two elements are always allowed.
Starting from index 2, for every current element, check if it's not equal to the element two places before (nums[i] != nums[start - 1]).
If it passes the condition, place it at the new position and move the start pointer forward.
🔽 Code Snippet:
if n <= 2: return n

start = 1
for i in range(2, n):
 if nums[i] != nums[start - 1]:
 start += 1
 nums[start] = nums[i]
✅ Time Complexity: O(n)
 ✅ Space Complexity: O(1)

🎯 What I Learned Today:
 🔸 How adding a small condition can make a big difference in logic
 🔸 The power of 2-pointer method in array problems
 🔸 Read constraints carefully — even one word like "at most twice" changes the solution
 🔸 Why understanding previous problems helps solve the next one faster

Let’s keep grinding! 💪
