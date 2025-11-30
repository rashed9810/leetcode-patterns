# Complete Algorithms Guide for Big Tech Interviews

## Table of Contents

1. [Sorting Algorithms](#1-sorting-algorithms)
2. [Searching Algorithms](#2-searching-algorithms)
3. [Two Pointers](#3-two-pointers)
4. [Sliding Window](#4-sliding-window)
5. [Recursion](#5-recursion)
6. [Backtracking](#6-backtracking)
7. [Dynamic Programming](#7-dynamic-programming)
8. [Greedy Algorithms](#8-greedy-algorithms)
9. [Divide and Conquer](#9-divide-and-conquer)
10. [Graph Algorithms](#10-graph-algorithms)
11. [Binary Search Variations](#11-binary-search-variations)
12. [Bit Manipulation](#12-bit-manipulation)
13. [Math & Number Theory](#13-math--number-theory)
14. [Interval Problems](#14-interval-problems)
15. [Advanced Algorithms](#15-advanced-algorithms)

---

## 1. Sorting Algorithms

### Importance: ⭐⭐⭐⭐⭐ (Critical Foundation)

### Algorithms to Master

#### 1.1 Comparison-Based Sorting

| Algorithm      | Best       | Average    | Worst      | Space    | Stable |
| -------------- | ---------- | ---------- | ---------- | -------- | ------ |
| Bubble Sort    | O(n)       | O(n²)      | O(n²)      | O(1)     | Yes    |
| Selection Sort | O(n²)      | O(n²)      | O(n²)      | O(1)     | No     |
| Insertion Sort | O(n)       | O(n²)      | O(n²)      | O(1)     | Yes    |
| Merge Sort     | O(n log n) | O(n log n) | O(n log n) | O(n)     | Yes    |
| Quick Sort     | O(n log n) | O(n log n) | O(n²)      | O(log n) | No     |
| Heap Sort      | O(n log n) | O(n log n) | O(n log n) | O(1)     | No     |

#### 1.2 Non-Comparison Sorting

| Algorithm     | Time        | Space    | Use Case              |
| ------------- | ----------- | -------- | --------------------- |
| Counting Sort | O(n + k)    | O(k)     | Small integer range   |
| Radix Sort    | O(d(n + k)) | O(n + k) | Fixed-length integers |
| Bucket Sort   | O(n + k)    | O(n)     | Uniformly distributed |

### Must-Know Implementations

- [ ] **Quick Sort** - Partition logic, pivot selection
- [ ] **Merge Sort** - Divide and merge, external sorting
- [ ] **Heap Sort** - Heapify process

### Interview Patterns

- Custom comparators
- Sorting with multiple criteria
- Partial sorting (K-th element)
- Sort stability considerations

### Common Interview Problems

- [ ] Sort Colors (Dutch National Flag)
- [ ] Kth Largest Element
- [ ] Merge Intervals
- [ ] Meeting Rooms
- [ ] Largest Number
- [ ] Sort List (Merge Sort on Linked List)
- [ ] Wiggle Sort
- [ ] Queue Reconstruction by Height

### Free Resources

1. **Video Tutorials**

   - [Sorting Algorithms - Abdul Bari](https://www.youtube.com/playlist?list=PLDN4rrl48XKpZkf03iYFl-O29szjTrs_O)
   - [Sorting Visualized - Fireship](https://www.youtube.com/watch?v=RfXt_qHDEPw)
   - [Quick Sort - mycodeschool](https://www.youtube.com/watch?v=COk73cpQbFQ)
   - [Merge Sort - MIT OCW](https://www.youtube.com/watch?v=JPyuH4qXLZ0)

2. **Reading Materials**

   - [Visualgo - Sorting](https://visualgo.net/en/sorting)
   - [GeeksforGeeks Sorting](https://www.geeksforgeeks.org/sorting-algorithms/)
   - [Sorting Algorithm Animations](https://www.toptal.com/developers/sorting-algorithms)

3. **Practice**
   - [LeetCode Sorting Problems](https://leetcode.com/tag/sorting/)

---

## 2. Searching Algorithms

### Importance: ⭐⭐⭐⭐⭐ (Critical)

### Algorithms to Master

| Algorithm            | Time         | Space | Requirements          |
| -------------------- | ------------ | ----- | --------------------- |
| Linear Search        | O(n)         | O(1)  | None                  |
| Binary Search        | O(log n)     | O(1)  | Sorted array          |
| Ternary Search       | O(log₃n)     | O(1)  | Unimodal function     |
| Exponential Search   | O(log n)     | O(1)  | Sorted, unknown size  |
| Interpolation Search | O(log log n) | O(1)  | Uniformly distributed |

### Binary Search Patterns

1. **Standard Binary Search**
2. **Lower Bound** (First occurrence)
3. **Upper Bound** (Last occurrence)
4. **Search Insert Position**
5. **Search in Rotated Array**
6. **Search on Answer** (Minimize/Maximize)

### Common Interview Problems

- [ ] Binary Search
- [ ] Search in Rotated Sorted Array
- [ ] Find Minimum in Rotated Sorted Array
- [ ] Search a 2D Matrix
- [ ] Find Peak Element
- [ ] Search for a Range (First and Last Position)
- [ ] Koko Eating Bananas
- [ ] Capacity to Ship Packages
- [ ] Split Array Largest Sum
- [ ] Median of Two Sorted Arrays

### Free Resources

1. **Video Tutorials**

   - [Binary Search - NeetCode](https://www.youtube.com/watch?v=s4DPM8ct1pI)
   - [Binary Search Patterns - Errichto](https://www.youtube.com/watch?v=GU7DpgHINWQ)
   - [Binary Search - take U forward](https://www.youtube.com/playlist?list=PLgUwDviBIf0pMFMWuuvDNMAkoQFi-h0ZF)

2. **Reading Materials**

   - [Binary Search 101 - LeetCode](https://leetcode.com/problems/binary-search/solutions/423162/binary-search-101/)
   - [TowardsDataScience Binary Search](https://towardsdatascience.com/understanding-binary-search-a-detailed-analysis-e2edbc95e1e4)

3. **Practice**
   - [LeetCode Binary Search Problems](https://leetcode.com/tag/binary-search/)

---

## 3. Two Pointers

### Importance: ⭐⭐⭐⭐⭐ (Critical)

### Patterns to Master

1. **Opposite Direction Pointers**

   - Start from both ends
   - Used in: Palindrome, Two Sum (sorted), Container problems

2. **Same Direction Pointers (Fast & Slow)**

   - Different speeds
   - Used in: Cycle detection, Middle element, Remove duplicates

3. **Sliding Window (see next section)**

4. **Partition Pointers**
   - Dutch National Flag
   - Quick Select

### Time Complexity

- Typically O(n) or O(n log n) if sorting needed
- Space: Usually O(1)

### Common Interview Problems

- [ ] Two Sum II (Sorted Array)
- [ ] 3Sum
- [ ] Container With Most Water
- [ ] Trapping Rain Water
- [ ] Valid Palindrome
- [ ] Remove Duplicates from Sorted Array
- [ ] Move Zeroes
- [ ] Sort Colors
- [ ] Linked List Cycle
- [ ] Palindrome Linked List
- [ ] Partition Labels
- [ ] Boats to Save People

### Free Resources

1. **Video Tutorials**

   - [Two Pointers - NeetCode](https://www.youtube.com/watch?v=cQ1Oz4ckceM)
   - [Two Pointers Pattern - take U forward](https://www.youtube.com/watch?v=A_v5PUr74Ho)
   - [Two Pointer Technique - Kevin Naughton Jr.](https://www.youtube.com/watch?v=-gjxg6Pln50)

2. **Reading Materials**

   - [LeetCode Two Pointers Guide](https://leetcode.com/articles/two-pointer-technique/)
   - [GeeksforGeeks Two Pointer](https://www.geeksforgeeks.org/two-pointers-technique/)

3. **Practice**
   - [LeetCode Two Pointers Problems](https://leetcode.com/tag/two-pointers/)

---

## 4. Sliding Window

### Importance: ⭐⭐⭐⭐⭐ (Critical)

### Patterns to Master

#### 4.1 Fixed Size Window

```
Window size is given

- Maximum/Minimum in window
- Window sum/average
```

#### 4.2 Variable Size Window

```
Find window satisfying condition

- Shrink when condition violated
- Expand otherwise
```

#### 4.3 With HashMap/Counter

```
Track character/element frequencies

- Anagram matching
- Substring problems
```

### Template Pattern

```python
def sliding_window(arr):
    left = 0
    result = 0
    window_state = {}  # or variable

    for right in range(len(arr)):
        # Expand window - add arr[right]

        while window_invalid():
            # Shrink window - remove arr[left]
            left += 1

        # Update result

    return result
```

### Time Complexity

- O(n) - each element visited at most twice

### Common Interview Problems

- [ ] Maximum Sum Subarray of Size K
- [ ] Longest Substring Without Repeating Characters
- [ ] Minimum Window Substring
- [ ] Longest Repeating Character Replacement
- [ ] Permutation in String
- [ ] Find All Anagrams in a String
- [ ] Sliding Window Maximum
- [ ] Minimum Size Subarray Sum
- [ ] Fruit Into Baskets
- [ ] Subarrays with K Different Integers

### Free Resources

1. **Video Tutorials**

   - [Sliding Window - NeetCode](https://www.youtube.com/watch?v=1pkOgXD63yU)
   - [Sliding Window Technique - Aditya Verma](https://www.youtube.com/playlist?list=PL_z_8CaSLPWeM8BDJmIYDaoQ5zuwyxnfj)
   - [Sliding Window - take U forward](https://www.youtube.com/watch?v=9kdHxplyl5I)

2. **Reading Materials**

   - [Sliding Window Patterns - Medium](https://medium.com/outco/how-to-solve-sliding-window-problems-28d67601a66)
   - [LeetCode Sliding Window Article](https://leetcode.com/discuss/study-guide/657507/Sliding-Window-for-Beginners-Problems-or-Template-or-Sample-Solutions)

3. **Practice**
   - [LeetCode Sliding Window Problems](https://leetcode.com/tag/sliding-window/)

---

## 5. Recursion

### Importance: ⭐⭐⭐⭐⭐ (Foundation for DP & Backtracking)

### Concepts to Master

1. **Base Cases**
2. **Recursive Cases**
3. **Call Stack Understanding**
4. **Tail Recursion**
5. **Recursion Tree Visualization**
6. **Memoization (leads to DP)**

### Common Patterns

1. **Linear Recursion** - Factorial, Sum
2. **Binary Recursion** - Fibonacci, Binary Tree
3. **Multiple Recursion** - Permutations
4. **Mutual Recursion** - Even/Odd check

### Time/Space Analysis

- Time: Count nodes in recursion tree
- Space: Maximum depth of recursion

### Common Interview Problems

- [ ] Fibonacci Number
- [ ] Pow(x, n)
- [ ] Reverse Linked List (Recursive)
- [ ] Merge Two Sorted Lists
- [ ] Maximum Depth of Binary Tree
- [ ] Same Tree
- [ ] Climbing Stairs
- [ ] Generate Parentheses
- [ ] Letter Combinations of a Phone Number
- [ ] K-th Symbol in Grammar

### Free Resources

1. **Video Tutorials**

   - [Recursion - Abdul Bari](https://www.youtube.com/watch?v=kHi1DUhp9kM)
   - [Recursion - freeCodeCamp](https://www.youtube.com/watch?v=IJDJ0kBx2LM)
   - [Recursion Masterclass - take U forward](https://www.youtube.com/playlist?list=PLgUwDviBIf0rGlzIn_7rsaR2FQ5e6ZOL9)

2. **Reading Materials**
   - [Recursion Guide - GeeksforGeeks](https://www.geeksforgeeks.org/recursion/)
   - [Thinking Recursively - Real Python](https://realpython.com/python-thinking-recursively/)

---

## 6. Backtracking

### Importance: ⭐⭐⭐⭐⭐ (Critical)

### Core Concept

```
Explore all possibilities
    If valid solution → add to result
    If dead end → backtrack (undo choice)
```

### Template Pattern

```python
def backtrack(path, choices):
    if is_solution(path):
        result.append(path.copy())
        return

    for choice in choices:
        if is_valid(choice):
            path.append(choice)        # Make choice
            backtrack(path, new_choices)  # Explore
            path.pop()                 # Undo choice (backtrack)
```

### Optimization Techniques

1. **Pruning** - Skip invalid branches early
2. **Ordering** - Try more promising choices first
3. **Constraint Propagation** - Reduce search space

### Common Patterns

1. **Subsets/Combinations**
2. **Permutations**
3. **Partitioning**
4. **Grid Exploration**
5. **Game Playing (N-Queens, Sudoku)**

### Common Interview Problems

- [ ] Subsets (I & II)
- [ ] Permutations (I & II)
- [ ] Combinations
- [ ] Combination Sum (I, II, III, IV)
- [ ] N-Queens
- [ ] Sudoku Solver
- [ ] Palindrome Partitioning
- [ ] Word Search
- [ ] Generate Parentheses
- [ ] Letter Combinations of Phone Number
- [ ] Restore IP Addresses
- [ ] Word Break II

### Free Resources

1. **Video Tutorials**

   - [Backtracking - Abdul Bari](https://www.youtube.com/watch?v=DKCbsiDBN6c)
   - [Backtracking Masterclass - NeetCode](https://www.youtube.com/watch?v=Zq4upTEaQyM)
   - [Backtracking Problems - take U forward](https://www.youtube.com/playlist?list=PLgUwDviBIf0rQ6cnlaHRMuOp4H_D-7hwP)

2. **Reading Materials**

   - [Backtracking Template - LeetCode](https://leetcode.com/problems/subsets/solutions/27281/a-general-approach-to-backtracking-questions-in-java/)
   - [GeeksforGeeks Backtracking](https://www.geeksforgeeks.org/backtracking-algorithms/)

3. **Practice**
   - [LeetCode Backtracking Problems](https://leetcode.com/tag/backtracking/)

---

## 7. Dynamic Programming

### Importance: ⭐⭐⭐⭐⭐ (Most Important for Big Tech)

### Core Concepts

1. **Overlapping Subproblems**
2. **Optimal Substructure**
3. **State Definition**
4. **State Transition (Recurrence)**
5. **Base Cases**

### Approaches

1. **Top-Down (Memoization)**

   - Recursive with caching
   - More intuitive

2. **Bottom-Up (Tabulation)**
   - Iterative
   - Often more efficient

### DP Patterns to Master

#### 7.1 Linear DP

- House Robber
- Climbing Stairs
- Fibonacci
- Maximum Subarray

#### 7.2 Grid DP

- Unique Paths
- Minimum Path Sum
- Dungeon Game
- Cherry Pickup

#### 7.3 String DP

- Longest Common Subsequence
- Edit Distance
- Longest Palindromic Subsequence
- Regular Expression Matching

#### 7.4 Knapsack Pattern

- 0/1 Knapsack
- Unbounded Knapsack
- Subset Sum
- Coin Change

#### 7.5 Interval DP

- Matrix Chain Multiplication
- Burst Balloons
- Minimum Cost to Merge Stones

#### 7.6 Tree DP

- House Robber III
- Binary Tree Maximum Path Sum
- Diameter of Binary Tree

#### 7.7 State Machine DP

- Best Time to Buy and Sell Stock (all variants)
- Paint House
- Paint Fence

### Problem-Solving Framework

```
1. Define state: dp[i] = ?
2. Find recurrence: dp[i] = f(dp[i-1], ...)
3. Identify base cases
4. Determine computation order
5. Optimize space if possible
```

### Common Interview Problems

- [ ] Climbing Stairs
- [ ] Coin Change (I & II)
- [ ] Longest Increasing Subsequence
- [ ] Longest Common Subsequence
- [ ] Edit Distance
- [ ] 0/1 Knapsack
- [ ] House Robber (I, II, III)
- [ ] Unique Paths
- [ ] Word Break
- [ ] Partition Equal Subset Sum
- [ ] Target Sum
- [ ] Maximum Product Subarray
- [ ] Decode Ways
- [ ] Best Time to Buy and Sell Stock (I-IV)
- [ ] Palindrome Partitioning II
- [ ] Burst Balloons
- [ ] Interleaving String
- [ ] Regular Expression Matching
- [ ] Wildcard Matching

### Free Resources

1. **Video Tutorials**

   - [DP Playlist - Aditya Verma (Best for DP)](https://www.youtube.com/playlist?list=PL_z_8CaSLPWekqhdCPmFohncHwz8TY2Go)
   - [DP - take U forward](https://www.youtube.com/playlist?list=PLgUwDviBIf0qUlt5H_kiKYaNSqJ81PMMY)
   - [DP Patterns - NeetCode](https://www.youtube.com/watch?v=mBNrRy2_hVs)
   - [DP - MIT OCW](https://www.youtube.com/watch?v=OQ5jsbhAv_M)

2. **Reading Materials**

   - [DP Patterns - LeetCode](https://leetcode.com/discuss/general-discussion/458695/Dynamic-Programming-Patterns)
   - [AtCoder DP Contest](https://atcoder.jp/contests/dp)
   - [CSES DP Section](https://cses.fi/problemset/)

3. **Practice**
   - [LeetCode DP Problems](https://leetcode.com/tag/dynamic-programming/)
   - [NeetCode 150 DP Section](https://neetcode.io)

---

## 8. Greedy Algorithms

### Importance: ⭐⭐⭐⭐ (High)

### Core Concept

```
Make locally optimal choice at each step
Hope it leads to globally optimal solution
```

### When to Use Greedy

1. **Optimal Substructure** exists
2. **Greedy Choice Property** holds
3. Problem has **matroid structure** (advanced)

### Common Patterns

1. **Interval Scheduling**
2. **Activity Selection**
3. **Huffman Coding**
4. **Minimum Spanning Tree**
5. **Dijkstra's Algorithm**
6. **Fractional Knapsack**

### Proof Techniques

1. **Greedy stays ahead**
2. **Exchange argument**
3. **Structural argument**

### Common Interview Problems

- [ ] Jump Game (I & II)
- [ ] Gas Station
- [ ] Candy
- [ ] Task Scheduler
- [ ] Meeting Rooms II
- [ ] Non-overlapping Intervals
- [ ] Merge Intervals
- [ ] Partition Labels
- [ ] Queue Reconstruction by Height
- [ ] Minimum Number of Arrows
- [ ] Lemonade Change
- [ ] Assign Cookies
- [ ] Reorganize String
- [ ] Boats to Save People

### Free Resources

1. **Video Tutorials**

   - [Greedy Algorithms - Abdul Bari](https://www.youtube.com/watch?v=ARvQcqJ_-NY)
   - [Greedy - NeetCode](https://www.youtube.com/watch?v=bC7o8P_Ste4)
   - [Greedy Problems - take U forward](https://www.youtube.com/playlist?list=PLgUwDviBIf0rF1w2Koyh78zafB0cz7tea)

2. **Reading Materials**

   - [Greedy Algorithms - GeeksforGeeks](https://www.geeksforgeeks.org/greedy-algorithms/)
   - [Greedy on CP-Algorithms](https://cp-algorithms.com/)

3. **Practice**
   - [LeetCode Greedy Problems](https://leetcode.com/tag/greedy/)

---

## 9. Divide and Conquer

### Importance: ⭐⭐⭐⭐ (High)

### Core Pattern

```
1. DIVIDE: Break problem into subproblems
2. CONQUER: Solve subproblems recursively
3. COMBINE: Merge subproblem solutions
```

### Classic Applications

1. **Merge Sort**
2. **Quick Sort**
3. **Binary Search**
4. **Fast Exponentiation**
5. **Closest Pair of Points**
6. **Karatsuba Multiplication**
7. **Strassen's Matrix Multiplication**

### Master Theorem

For recurrence T(n) = aT(n/b) + f(n):

- If f(n) = O(n^(log_b(a) - ε)) → T(n) = Θ(n^log_b(a))
- If f(n) = Θ(n^log_b(a)) → T(n) = Θ(n^log_b(a) \* log n)
- If f(n) = Ω(n^(log_b(a) + ε)) → T(n) = Θ(f(n))

### Common Interview Problems

- [ ] Merge Sort
- [ ] Quick Select (Kth Element)
- [ ] Maximum Subarray (D&C approach)
- [ ] Pow(x, n)
- [ ] Median of Two Sorted Arrays
- [ ] Count of Smaller Numbers After Self
- [ ] Closest Pair of Points
- [ ] Different Ways to Add Parentheses
- [ ] Kth Largest Element in Array
- [ ] Search a 2D Matrix II

### Free Resources

1. **Video Tutorials**

   - [Divide and Conquer - MIT OCW](https://www.youtube.com/watch?v=EzeYI7p9MjU)
   - [D&C - Abdul Bari](https://www.youtube.com/watch?v=2Rr2tW9zvRg)
   - [Master Theorem - Back To Back SWE](https://www.youtube.com/watch?v=OynWkEj0S-s)

2. **Reading Materials**
   - [D&C - GeeksforGeeks](https://www.geeksforgeeks.org/divide-and-conquer/)
   - [CLRS Chapter 4](https://mitpress.mit.edu/books/introduction-algorithms-third-edition)

---

## 10. Graph Algorithms

### Importance: ⭐⭐⭐⭐⭐ (Critical)

### 10.1 Graph Traversal

#### BFS (Breadth-First Search)

```
Time: O(V + E)
Space: O(V)
Use: Shortest path (unweighted), Level order
```

#### DFS (Depth-First Search)

```
Time: O(V + E)
Space: O(V)
Use: Cycle detection, Connectivity, Topological sort
```

### 10.2 Shortest Path Algorithms

| Algorithm      | Graph Type | Time          | Negative Edges |
| -------------- | ---------- | ------------- | -------------- |
| BFS            | Unweighted | O(V+E)        | N/A            |
| Dijkstra       | Weighted   | O((V+E)log V) | No             |
| Bellman-Ford   | Weighted   | O(VE)         | Yes            |
| Floyd-Warshall | All pairs  | O(V³)         | Yes            |
| A\*            | Weighted   | O(E) best     | No             |

### 10.3 Minimum Spanning Tree

| Algorithm | Time           | Best For      |
| --------- | -------------- | ------------- |
| Kruskal   | O(E log E)     | Sparse graphs |
| Prim      | O((V+E) log V) | Dense graphs  |

### 10.4 Topological Sort

```
Use: Dependency resolution, Course scheduling
Algorithms: Kahn's (BFS), DFS-based
Time: O(V + E)
```

### 10.5 Cycle Detection

- **Undirected**: Union-Find or DFS
- **Directed**: DFS with colors, Topological sort

### 10.6 Strongly Connected Components

- Tarjan's Algorithm
- Kosaraju's Algorithm

### Common Interview Problems

- [ ] Number of Islands
- [ ] Clone Graph
- [ ] Course Schedule (I & II)
- [ ] Pacific Atlantic Water Flow
- [ ] Graph Valid Tree
- [ ] Number of Connected Components
- [ ] Alien Dictionary
- [ ] Word Ladder
- [ ] Network Delay Time
- [ ] Cheapest Flights Within K Stops
- [ ] Shortest Path in Binary Matrix
- [ ] Critical Connections in a Network
- [ ] Reconstruct Itinerary
- [ ] Evaluate Division
- [ ] Word Search II

### Free Resources

1. **Video Tutorials**

   - [Graph Theory Full Course - William Fiset](https://www.youtube.com/playlist?list=PLDV1Zeh2NRsDGO4--qE8yH72HFL1Km93P)
   - [Graph Algorithms - Abdul Bari](https://www.youtube.com/playlist?list=PLDN4rrl48XKpZkf03iYFl-O29szjTrs_O)
   - [Graphs - NeetCode](https://www.youtube.com/watch?v=utDu3Q7C8Ws)
   - [Graph Problems - take U forward](https://www.youtube.com/playlist?list=PLgUwDviBIf0oE3gA41TKO2H5bHpPd7fzn)

2. **Reading Materials**

   - [Visualgo - Graph Traversal](https://visualgo.net/en/dfsbfs)
   - [CP-Algorithms Graphs](https://cp-algorithms.com/)
   - [GeeksforGeeks Graph Algorithms](https://www.geeksforgeeks.org/graph-data-structure-and-algorithms/)

3. **Practice**
   - [LeetCode Graph Problems](https://leetcode.com/tag/graph/)

---

## 11. Binary Search Variations

### Importance: ⭐⭐⭐⭐⭐ (Critical)

### Patterns to Master

#### 11.1 Classic Binary Search

```python
def binary_search(arr, target):
    left, right = 0, len(arr) - 1
    while left <= right:
        mid = left + (right - left) // 2
        if arr[mid] == target:
            return mid
        elif arr[mid] < target:
            left = mid + 1
        else:
            right = mid - 1
    return -1
```

#### 11.2 Lower Bound (First Occurrence)

```python
def lower_bound(arr, target):
    left, right = 0, len(arr)
    while left < right:
        mid = left + (right - left) // 2
        if arr[mid] < target:
            left = mid + 1
        else:
            right = mid
    return left
```

#### 11.3 Upper Bound (First Greater)

```python
def upper_bound(arr, target):
    left, right = 0, len(arr)
    while left < right:
        mid = left + (right - left) // 2
        if arr[mid] <= target:
            left = mid + 1
        else:
            right = mid
    return left
```

#### 11.4 Binary Search on Answer

```python
def binary_search_answer(low, high, condition):
    while low < high:
        mid = low + (high - low) // 2
        if condition(mid):
            high = mid  # or low = mid + 1 for maximum
        else:
            low = mid + 1
    return low
```

### Common Interview Problems

- [ ] Binary Search
- [ ] Search Insert Position
- [ ] First and Last Position in Sorted Array
- [ ] Search in Rotated Sorted Array (I & II)
- [ ] Find Minimum in Rotated Sorted Array
- [ ] Find Peak Element
- [ ] Search a 2D Matrix (I & II)
- [ ] Koko Eating Bananas
- [ ] Capacity to Ship Packages
- [ ] Split Array Largest Sum
- [ ] Median of Two Sorted Arrays
- [ ] Find K-th Smallest Pair Distance

### Free Resources

1. **Video Tutorials**
   - [Binary Search - Errichto (Advanced)](https://www.youtube.com/watch?v=GU7DpgHINWQ)
   - [Binary Search on Answer - NeetCode](https://www.youtube.com/watch?v=UXDSeD9mN-k)
   - [Binary Search Playlist - take U forward](https://www.youtube.com/playlist?list=PLgUwDviBIf0pMFMWuuvDNMAkoQFi-h0ZF)

---

## 12. Bit Manipulation

### Importance: ⭐⭐⭐⭐ (High)

### Essential Operations

```
AND (&)   : Check bit, clear bit
OR (|)    : Set bit
XOR (^)   : Toggle bit, find unique
NOT (~)   : Invert bits
Left Shift (<<)  : Multiply by 2
Right Shift (>>) : Divide by 2
```

### Common Techniques

```python
# Check if bit is set
(n >> i) & 1

# Set bit
n | (1 << i)

# Clear bit
n & ~(1 << i)

# Toggle bit
n ^ (1 << i)

# Check if power of 2
n & (n - 1) == 0

# Get lowest set bit
n & (-n)

# Clear lowest set bit
n & (n - 1)

# Count set bits
bin(n).count('1')  # or Brian Kernighan's algorithm
```

### Common Interview Problems

- [ ] Single Number (I, II, III)
- [ ] Number of 1 Bits
- [ ] Counting Bits
- [ ] Reverse Bits
- [ ] Missing Number
- [ ] Power of Two
- [ ] Bitwise AND of Numbers Range
- [ ] Sum of Two Integers (without +/-)
- [ ] Maximum XOR of Two Numbers
- [ ] Find the Duplicate Number

### Free Resources

1. **Video Tutorials**

   - [Bit Manipulation - NeetCode](https://www.youtube.com/watch?v=5Km3utixwZs)
   - [Bit Manipulation - Errichto](https://www.youtube.com/watch?v=xXKL9YBWgCY)
   - [Bit Manipulation - take U forward](https://www.youtube.com/watch?v=5rtVTYAk9KQ)

2. **Reading Materials**

   - [Bit Manipulation - GeeksforGeeks](https://www.geeksforgeeks.org/bits-manipulation-important-tactics/)
   - [Bit Twiddling Hacks](https://graphics.stanford.edu/~seander/bithacks.html)

3. **Practice**
   - [LeetCode Bit Manipulation Problems](https://leetcode.com/tag/bit-manipulation/)

---

## 13. Math & Number Theory

### Importance: ⭐⭐⭐ (Medium-High)

### Essential Concepts

#### 13.1 Basic Math

- Prime numbers and Sieve of Eratosthenes
- GCD and LCM (Euclidean Algorithm)
- Modular arithmetic
- Fast exponentiation

#### 13.2 Number Theory

- Prime factorization
- Modular inverse
- Chinese Remainder Theorem (advanced)

#### 13.3 Combinatorics

- Permutations and Combinations
- Pascal's Triangle
- Catalan Numbers

#### 13.4 Geometry (Basic)

- Distance formulas
- Line intersection
- Convex hull (advanced)

### Common Interview Problems

- [ ] Palindrome Number
- [ ] Reverse Integer
- [ ] Power of Three
- [ ] Count Primes
- [ ] Factorial Trailing Zeroes
- [ ] Sqrt(x)
- [ ] Happy Number
- [ ] Ugly Number (I & II)
- [ ] Integer Break
- [ ] Valid Perfect Square
- [ ] GCD and LCM
- [ ] Robot Return to Origin

### Free Resources

1. **Video Tutorials**

   - [Math for Programmers - freeCodeCamp](https://www.youtube.com/watch?v=2SpuBqvNjHI)
   - [Number Theory - CodeNCode](https://www.youtube.com/playlist?list=PL2q4fbVm1Ik6DCzm9XZJbNwyHtHGclcEh)
   - [Modular Arithmetic - William Fiset](https://www.youtube.com/watch?v=B-ka_7T_qVw)

2. **Reading Materials**

   - [CP-Algorithms Number Theory](https://cp-algorithms.com/algebra/euclid-algorithm.html)
   - [GeeksforGeeks Mathematical Algorithms](https://www.geeksforgeeks.org/mathematical-algorithms/)

3. **Practice**
   - [LeetCode Math Problems](https://leetcode.com/tag/math/)

---

## 14. Interval Problems

### Importance: ⭐⭐⭐⭐ (High)

### Common Patterns

1. **Merge Overlapping Intervals**
2. **Insert Interval**
3. **Interval Scheduling**
4. **Meeting Rooms**
5. **Minimum Platforms**

### Techniques

1. **Sort by start time**
2. **Sort by end time**
3. **Sweep Line Algorithm**
4. **Min Heap for end times**

### Common Interview Problems

- [ ] Merge Intervals
- [ ] Insert Interval
- [ ] Non-overlapping Intervals
- [ ] Meeting Rooms (I & II)
- [ ] Minimum Number of Arrows
- [ ] Employee Free Time
- [ ] Interval List Intersections
- [ ] My Calendar (I, II, III)
- [ ] Remove Covered Intervals
- [ ] Data Stream as Disjoint Intervals

### Free Resources

1. **Video Tutorials**

   - [Interval Problems - NeetCode](https://www.youtube.com/watch?v=44H3cEC2fFM)
   - [Interval Scheduling - Abdul Bari](https://www.youtube.com/watch?v=hVhOeaONg1Y)
   - [Sweep Line - Algorithms Live](https://www.youtube.com/watch?v=RBCJkkZYwwI)

2. **Practice**
   - [LeetCode Interval Problems](https://leetcode.com/tag/intervals/)

---

## 15. Advanced Algorithms

### Importance: ⭐⭐⭐ (For Senior Roles)

### 15.1 String Algorithms

- **KMP Pattern Matching** - O(n + m)
- **Rabin-Karp** - O(n + m) average
- **Z-Algorithm** - O(n + m)
- **Manacher's Algorithm** - Longest palindrome O(n)
- **Suffix Array/Tree** - String matching O(n)

### 15.2 Advanced Graph

- **Tarjan's SCC**
- **Articulation Points & Bridges**
- **Maximum Flow** (Ford-Fulkerson)
- **Bipartite Matching**

### 15.3 Advanced DP

- **DP on Trees**
- **DP with Bitmask**
- **Digit DP**
- **SOS DP (Sum over Subsets)**

### 15.4 Computational Geometry

- **Convex Hull**
- **Line Sweep**
- **Closest Pair of Points**

### Free Resources

1. **Video Tutorials**

   - [Advanced Algorithms - MIT OCW](https://ocw.mit.edu/courses/6-854j-advanced-algorithms-fall-2008/)
   - [String Algorithms - William Fiset](https://www.youtube.com/playlist?list=PLDV1Zeh2NRsDGO4--qE8yH72HFL1Km93P)
   - [Advanced Topics - Errichto](https://www.youtube.com/c/Errichto)

2. **Reading Materials**
   - [CP-Algorithms (All Advanced Topics)](https://cp-algorithms.com/)
   - [CSES Problem Set](https://cses.fi/problemset/)

---

## Summary: Algorithms Priority Matrix

| Algorithm              | Interview Frequency | Difficulty | Priority |
| ---------------------- | ------------------- | ---------- | -------- |
| Binary Search          | ⭐⭐⭐⭐⭐          | Easy       | 1        |
| Two Pointers           | ⭐⭐⭐⭐⭐          | Easy       | 1        |
| Sliding Window         | ⭐⭐⭐⭐⭐          | Medium     | 1        |
| BFS/DFS                | ⭐⭐⭐⭐⭐          | Medium     | 1        |
| Dynamic Programming    | ⭐⭐⭐⭐⭐          | Hard       | 1        |
| Backtracking           | ⭐⭐⭐⭐            | Medium     | 2        |
| Sorting                | ⭐⭐⭐⭐            | Easy       | 2        |
| Greedy                 | ⭐⭐⭐⭐            | Medium     | 2        |
| Recursion              | ⭐⭐⭐⭐            | Easy       | 2        |
| Bit Manipulation       | ⭐⭐⭐              | Medium     | 3        |
| Math                   | ⭐⭐⭐              | Medium     | 3        |
| Divide & Conquer       | ⭐⭐⭐              | Medium     | 3        |
| Topological Sort       | ⭐⭐⭐              | Medium     | 3        |
| Union Find             | ⭐⭐⭐              | Medium     | 3        |
| Dijkstra/Shortest Path | ⭐⭐⭐              | Medium     | 3        |
| Advanced String Algos  | ⭐⭐                | Hard       | 4        |
| Advanced Graph         | ⭐⭐                | Hard       | 4        |

---

## Recommended Study Plan

### Week 1-2: Foundations

- Arrays, Strings, Hash Tables
- Basic Sorting and Searching
- Two Pointers, Sliding Window

### Week 3-4: Linear Structures

- Linked Lists
- Stacks and Queues
- Monotonic Stack/Queue

### Week 5-6: Recursion & Backtracking

- Recursion Mastery
- Backtracking Patterns
- Subset/Permutation/Combination

### Week 7-8: Trees

- Binary Trees
- BST
- Tree Traversals and Properties

### Week 9-10: Dynamic Programming

- 1D DP
- 2D DP
- Common Patterns (Knapsack, LCS, LIS)

### Week 11-12: Graphs

- BFS/DFS
- Shortest Path
- Topological Sort

### Week 13-14: Advanced Topics

- Heaps and Priority Queues
- Tries
- Union Find
- Bit Manipulation

### Week 15-16: Practice & Mock Interviews

- Mixed problems
- Company-specific problems
- Time-based practice

---

## Essential Free Courses

1. **Abdul Bari Algorithms** (YouTube)

   - Best for algorithm theory
   - [https://www.youtube.com/c/AbdulBari](https://www.youtube.com/results?search_query=abdul+bari+algorithm)

2. **MIT OpenCourseWare 6.006** (YouTube)

   - Introduction to Algorithms
   - https://www.youtube.com/playlist?list=PLUl4u3cNGP61Oq3tWYp6V_F-5jb5L2iHb

3. **NeetCode** (YouTube + Website)

   - Best for interview prep
   - https://www.youtube.com/@NeetCode
   - https://neetcode.io

4. **take U forward** (YouTube)

   - Comprehensive DSA
   - https://www.youtube.com/@takeUforward

5. **William Fiset** (YouTube)

   - Graph theory expert
   - https://www.youtube.com/@WilliamFiset-videos

6. **freeCodeCamp** (YouTube)

   - Full courses
   - https://www.youtube.com/@freecodecamp

7. **CS50** (Harvard)
   - CS fundamentals
   - https://cs50.harvard.edu/x

---

## Practice Platforms

| Platform        | Best For            | URL             |
| --------------- | ------------------- | --------------- |
| LeetCode        | Interview Problems  | leetcode.com    |
| NeetCode        | Structured Learning | neetcode.io     |
| HackerRank      | Basics              | hackerrank.com  |
| Codeforces      | Competitive         | codeforces.com  |
| AtCoder         | Quality Problems    | atcoder.jp      |
| CSES            | Classic Problems    | cses.fi         |
| Pramp           | Mock Interviews     | pramp.com       |
| Interviewing.io | Mock Interviews     | interviewing.io |
