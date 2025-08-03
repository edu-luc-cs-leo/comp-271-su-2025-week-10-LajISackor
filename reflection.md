# Reflection

For the Week 09 assignment, I implemented recursive solutions for several classic problems: finding the maximum in a subarray, reversing an array in-place, counting occurrences of a target value, and performing a binary search. After reviewing Leo's solution, I found that while my logic was mostly aligned in intent, there were areas where my implementation could be improved in both style and structure.

One area I did well in was following the recursive paradigm without relying on any loops, which was a major requirement. I also structured the base cases appropriately and ensured that the recursive calls simplified the problem each time. However, when comparing my `findMax` method to Leo’s, I noticed that he included two different styles: one that gradually trimmed the array from the outside in, and another that used a divide-and-conquer approach like merge sort. This showed me there’s more than one correct recursive approach, and that being deliberate about which one to choose can affect clarity and performance.

In the `binarySearch` method, Leo added defensive checks for bounds and used clear comments to explain how the recursion narrows down the search space. I had implemented a similar structure, but his use of `left + (right - left) / 2` instead of `(left + right)/2` is a subtle improvement that prevents overflow, a detail I hadn’t considered.

From this comparison, I learned the value of thoughtful recursion design and the importance of writing clean, readable code that anticipates edge cases. Going forward, I’ll make sure to plan both the recursion structure and base cases more carefully and aim to add better documentation throughout the code.
