DSA Notes

1. Basic Math Notes

Palindrome

A number is considered a palindrome if it reads the same backward as forward. However, there are some important boundary conditions to check:

Boundary Conditions:

If x < 0, return false (negative numbers cannot be palindromes).

If x % 10 == 0 && x != 0, return false (numbers ending in zero, except zero itself, cannot be palindromes).

Example:

Input: x = 100

Reverse digits: 001. Since the original number ends with a zero, it cannot be a palindrome.

Approach:

Before proceeding to the loop, ensure the above conditions are satisfied.

If conditions hold, proceed to check for palindrome using a loop or by reversing the number.

GCD (Greatest Common Divisor)

The GCD of two numbers is the largest number that divides both without leaving a remainder. While there are several methods to find the GCD, the Euclidean Algorithm is the most efficient.

Euclidean Algorithm:

Formula: GCD(a, b) = GCD(a % b, b) (if a > b)

Repeat until one of the numbers becomes zero.

Example:

Input: a = 48, b = 18

Steps:

48 % 18 = 12

18 % 12 = 6

12 % 6 = 0

Output: GCD is 6.

Why Optimal?

This approach reduces the size of the numbers drastically in each step, achieving a time complexity of O(log(min(a, b))).

Armstrong Number

An Armstrong number is a number that is equal to the sum of its own digits raised to the power of the number of digits.

Definition:

A number n is Armstrong if:

Example:

Input: n = 153

Calculation:



Output: 153 is an Armstrong number.

Steps to Calculate:

Extract each digit using %:

int temp = n % 10;
n = n / 10;
num += Math.pow(temp, 3);

Repeat until all digits are processed.

Complexity:

Time Complexity: O(log(n)) (proportional to the number of digits).

Summary

Palindrome: Ensure the number is valid before checking.

GCD: Use the Euclidean Algorithm for optimal results.

Armstrong Number: Check by summing powers of digits.

These basic math concepts are essential in solving a wide range of coding problems efficiently. Mastering these techniques will give you a solid foundation for DSA.

