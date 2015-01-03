

Summary of some [LeetCode](https://oj.leetcode.com/problems/) problems marked as easy in difficulty.

Solutions are on my [Github](https://github.com/startupjing/coding_problems)

<!-- more -->

Contents:

- [Lists](#Lists)

- [Arrays](#Arrays)

- [Strings](#Strings)

- [Trees](#Trees)

- [Math and Integers](#Math and Integers)

- [Stack](#Stack)

- [Dynamic Programming](#Dynamic Programming)

- [Sorting and Searching](#Sorting and Searching)


<a name="Lists"/>

### Lists

* Linked List Cycle:

Use fast/slow runner technique. Fast and slow runner will eventually meet if a cycle exists. Otherwise, fast runner will hit null

* Swap Node Pair:

Use two pointers to adjacent nodes and link two nodes to previous swapped list


<a name="Arrays"/>

### Arrays

* Single Number:

If additional space allowed, use a hashset to store(first time) and remove(second time) elements. If space not allowed, use XOR operation since y XOR y = 0;

* Search Insert Position:n

Simple array traversal

* Minimum Rotated Sorted Array:

The first element such that arr[i-1]>arr[i] is the min element.

* Set Matrix Zeroes:

Use first row and column to mark rows and columns to be set to 0, but need to check if need to zero out first row and column first

<a name="Strings"/>

### Strings



<a name="Trees"/>

### Trees

* Binary Tree Inorder Traversal:

Use a stack to store parent nodes. Traverse to the left until reaching a leaf, then pop parent node from stack and switch to parent's right subtree.

* Binary Tree Preorder Traversal:

Use a stack to store roots. Visit root first, then store root of right subtree into stack, switch to visit left subtree until reaching a leaf, then pop right subtree from stack and visit

* Populate Next Right Pointer:

First connect two children of the same parent, then connect neighbor children of neighbor parents, and finally do recursion on left/right subtrees

* Sorted Array to BST:

Build root using middle element, and build left/right child using recursion on left/right subarrays

* Sum Root to Leaf Numbers:

Use DFS to sum from bottom up.


<a name="Math and Integers"/>

### Math and Integers

* Single Number 2:

Sum up bit at each position and modulo 3 to get single number

* Integer to Roman:

First build mapping between integer values and Roman numerals including subtractive notations. Then use modulo operation to convert bases to Roman numerals

<a name="Stack"/>

### Stack



<a name="Dynamic Programming"/>

### Dynamic Programming

* Unique Binary Trees:

Suppose tree[i]=#trees given value i, then tree[i]+=(#left tree)*(#right tree) for each possible root value j=1,2,3..i

* Maximum SubArray:

Dynamic programming -- track max_so_far and upate max_end_here; Divide and conquer -- max(max left subarray, max right subarray, max subarray crossing midpoint)

* Best Time to Buy and Sell Stock:

Track min price to buy stock and track max profit to sell stock

* Best Time to Buy and Sell Stock 2:

Perform a transaction whenver price goes down in adjacent days


<a name="Divide and Conquer"/>

### Divide and Conquer

* Find Peak Element:

Divide-and-Conquer, check if mid element is a peak, otherwise check if mid is smaller than left/right neighbor, then left/right subarray must contain a peak element(due to locally raising)

<a name="Sorting and Searching"/>

### Sorting and Searching

* Sort Colors:

One simple approach is to do a counting sort, and rewrite the array by number of different elements. An improvement is to use two pointers pointer to the positions to insert red and blue elements. While traversing the array, move elements into its belonged region and upate boundary pointers.

* Search 2D Matrix:

First do binary search on rows and do binary search on selected rows.


