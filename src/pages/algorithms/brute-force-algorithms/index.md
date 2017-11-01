---
title: Brute Force Algorithms
---
## Brute Force Algorithms

Brute force algorithms, also known as exhaustive search algorithms are a method of problem solving that consists of systematically enumerating every possible solution candidate and checking if the candidate satisfies the problem statement. 

Brute force algorithms have the following basic structure:
1. Find a first candidate solution for problem P: *first(P)*
1. Find the next candidate solution after the current solution: *next(P, c)*
1. Check whether the candidate solution is a valid solution: *valid(P, c)*
1. Output the solution: *output(P, c)*

The basic flow looks like this:
```
c = first(P)
while (c != end) do
  if(valid(P, c)) then output(P, c)
  c = next(P, c)
end while
```

### Examples of the Brute Force Approach ###
1.*Sorting*: BubbleSort is an example of a brute force algorithm. It compares every element with every other element and runs in O(n^2)

2.*Search*: A linear search through an array is an example of a brute force approach. In this simple case, a brute force search runs in O(n), but in more complex cases such as searching through a two-dimensional matrix or searching for a subarray, it turns into O(n^2) or worse.

### Disadvantage of Brute Force Algorithms ###
The brute force approach may work for simple problems, but many real-world problems have a very large amount of candidate solutions, so the algorithms become impractically slow. For example, array sorting with BubbleSort will work for an array of 100 elements, but will be too slow if the array has 1,000,000 elements or more. Faster algorithms such as Quicksort (O(nlogn)) or dynamic programming and heuristic approaches are required for such problems.

#### More Information:
[Which algorithms are brute force, greedy, and dynamic programming](http://practice.geeksforgeeks.org/problems/which-algorithms-come-under-brute-force-greedy-and-dynamic-programming)


