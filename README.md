# question-no-2894
Solution to the question no 2894 on leet code 

2894. Divisible and Non-divisible Sums Difference
You are given positive integers n and m.

Define two integers as follows:

num1: The sum of all integers in the range [1, n] (both inclusive) that are not divisible by m.
num2: The sum of all integers in the range [1, n] (both inclusive) that are divisible by m.
Return the integer num1 - num2.

(n * (n + 1)) / 2 → Sum of all numbers from 1 to n.

k = n / m → Number of multiples of m up to n.

k * (k + 1) * m / 2 → Sum of all numbers from 1 to n that are divisible by m (using arithmetic series formula).

But instead of dividing by 2 at the end, it multiplies k * (k + 1) * m directly, which gives double the correct sum of multiples of m.
So, this implementation is incorrect unless there's a specific interpretation of the problem.
