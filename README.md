# Moglix_Assignment

I used a stack to keep track of the indices of opening brackets. I started by pushing -1 into the stack so that the length of a valid substring can be calculated easily. While traversing the string, I pushed the index of every '('. For every ')', I popped the top element. If the stack became empty, I pushed the current index because it acts as the starting point for the next possible valid substring. Otherwise, I calculated the current valid length using i - stack.top(). Whenever I found a longer valid substring, I stored its length and ending index. Finally, I printed the substring using substr().

**Time Complexity:** `O(n)` - As I traverse the string only once from left to right.
**Space Complexity:** `O(n)` - As the stack stores the indices of all the opening brackets.
