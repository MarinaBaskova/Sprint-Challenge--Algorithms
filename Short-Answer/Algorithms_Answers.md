Add your answers to the Algorithms exercises here.
Exercise I
a) In the example a, we have a while loop. If you count how many times loop run , it runs the n number of times. The loop will run as long as a is less then n to the power of 3. So the loop will run untill it meet (n^3). Inside of a loop a will be incremented by n^2. So n^3 / n ^2 = (n), and we can say that the cycle will run n times. The time complexity is O(n). And space complexity should be O(1), since we only allocating memory to a varable a.

b) In the example b, we have 4 for loops, all nested within one athother. From the first look we could say we could have O(n^4) with those nested loops, but this answer will be incorrect. Here is why, if we look close at the last loop: for l in range(k + 1, 10 + k). This loop will run always constant time no matter what k is, and this loop will be O(1). So time complexity in the example b, will be O(n^3). The space complexity should be O(1), as we allocating memory to a handfull of integer variables.

c) In the example c, we have function that has n input and has a recursive call inside of it. Each recursive call the n input decrements n by 1, untill it reaches the 0, which is the base case. So the time complexity will be O(n), and since the function has a recursive call it allocates memory for function, so the space complexity is O(n).

Exercise II

If we imagine that our buiding with n floors, like a sorted array. And we need to find the last safe floor f, where if we go one floor up the egg we drop will break. We need to create searching algorithim so we make the least amount of passes with broken eggs. In this case we can use a binary-search algorithm to solve the task. We can start by dividing n by 2, and dropping an egg from there. If the egg break, we can then leave out the values larger than n/2, and divide by 2 again to drop another egg. If egg breaks, we again leave out values greater than n/2/2,and keep the until egg doesnt break. So the time complexity will be O(logn) and O(n) for space complexity(when done with iterations).
