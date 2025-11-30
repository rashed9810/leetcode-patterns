# Complete Data Structures Guide for Big Tech Interviews

## Table of Contents

1. [Arrays](#1-arrays)
2. [Strings](#2-strings)
3. [Hash Tables](#3-hash-tables)
4. [Linked Lists](#4-linked-lists)
5. [Stacks](#5-stacks)
6. [Queues](#6-queues)
7. [Trees](#7-trees)
8. [Heaps](#8-heaps)
9. [Graphs](#9-graphs)
10. [Tries](#10-tries)
11. [Union-Find (Disjoint Set)](#11-union-find-disjoint-set)
12. [Advanced Data Structures](#12-advanced-data-structures)

---

## 1. Arrays

### Importance: ⭐⭐⭐⭐⭐ (Critical - Asked in 90%+ interviews)

### Concepts to Master

- **Static vs Dynamic Arrays**
- **Multi-dimensional Arrays (2D, 3D)**
- **Array Manipulation Techniques**
  - Two Pointers
  - Sliding Window
  - Prefix Sum
  - Kadane's Algorithm
- **In-place Operations**
- **Rotation and Reversal**

### Time Complexities

| Operation       | Average | Worst |
| --------------- | ------- | ----- |
| Access          | O(1)    | O(1)  |
| Search          | O(n)    | O(n)  |
| Insert (end)    | O(1)    | O(n)  |
| Insert (middle) | O(n)    | O(n)  |
| Delete          | O(n)    | O(n)  |

### Common Interview Problems

- [ ] Two Sum, Three Sum, Four Sum
- [ ] Container With Most Water
- [ ] Trapping Rain Water
- [ ] Maximum Subarray (Kadane's)
- [ ] Product of Array Except Self
- [ ] Merge Intervals
- [ ] Next Permutation
- [ ] Rotate Array
- [ ] Find Duplicate Number
- [ ] First Missing Positive

### Free Resources

1. **Video Tutorials**

   - [Arrays - CS Dojo](https://www.youtube.com/watch?v=pmN9ExDf3yQ)
   - [Array Data Structure - freeCodeCamp](https://www.youtube.com/watch?v=o2W7FFKJ3PU)
   - [Two Pointers Technique - NeetCode](https://www.youtube.com/watch?v=cQ1Oz4ckceM)
   - [Sliding Window - take U forward](https://www.youtube.com/watch?v=9kdHxplyl5I)

2. **Reading Materials**

   - [GeeksforGeeks Arrays](https://www.geeksforgeeks.org/array-data-structure/)
   - [Programiz Arrays](https://www.programiz.com/dsa/array)

3. **Practice**
   - [LeetCode Array Problems](https://leetcode.com/tag/array/)
   - [HackerRank Arrays](https://www.hackerrank.com/domains/data-structures?filters%5Bsubdomains%5D%5B%5D=arrays)

---

## 2. Strings

### Importance: ⭐⭐⭐⭐⭐ (Critical)

### Concepts to Master

- **String Manipulation**
- **Pattern Matching Algorithms**
  - Naive Pattern Search
  - KMP Algorithm
  - Rabin-Karp Algorithm
  - Z-Algorithm
- **String Hashing**
- **Palindrome Techniques**
- **Anagram Detection**
- **Substring Problems**

### Time Complexities

| Operation              | Complexity |
| ---------------------- | ---------- |
| Access                 | O(1)       |
| Find substring (naive) | O(n\*m)    |
| Find substring (KMP)   | O(n+m)     |
| Concatenation          | O(n)       |
| Comparison             | O(n)       |

### Common Interview Problems

- [ ] Longest Substring Without Repeating Characters
- [ ] Longest Palindromic Substring
- [ ] Valid Anagram
- [ ] Group Anagrams
- [ ] Valid Parentheses
- [ ] Minimum Window Substring
- [ ] Longest Common Prefix
- [ ] String to Integer (atoi)
- [ ] Edit Distance
- [ ] Regular Expression Matching

### Free Resources

1. **Video Tutorials**

   - [String Algorithms - Abdul Bari](https://www.youtube.com/watch?v=V5-7GzOfADQ)
   - [KMP Algorithm - Tushar Roy](https://www.youtube.com/watch?v=GTJr8OvyEVQ)
   - [Rabin-Karp - MIT OCW](https://www.youtube.com/watch?v=BRO7mVIFt08)

2. **Reading Materials**

   - [CP-Algorithms String Processing](https://cp-algorithms.com/string/string-hashing.html)
   - [GeeksforGeeks String Algorithms](https://www.geeksforgeeks.org/string-data-structure/)

3. **Practice**
   - [LeetCode String Problems](https://leetcode.com/tag/string/)

---

## 3. Hash Tables

### Importance: ⭐⭐⭐⭐⭐ (Critical - Used in 70%+ solutions)

### Concepts to Master

- **Hash Functions**
- **Collision Resolution**
  - Chaining
  - Open Addressing (Linear Probing, Quadratic Probing, Double Hashing)
- **Load Factor and Rehashing**
- **HashSet vs HashMap**
- **Designing Custom Hash Functions**

### Time Complexities

| Operation | Average | Worst |
| --------- | ------- | ----- |
| Insert    | O(1)    | O(n)  |
| Delete    | O(1)    | O(n)  |
| Search    | O(1)    | O(n)  |

### Common Interview Problems

- [ ] Two Sum
- [ ] LRU Cache
- [ ] Group Anagrams
- [ ] Subarray Sum Equals K
- [ ] Longest Consecutive Sequence
- [ ] Top K Frequent Elements
- [ ] Design HashMap
- [ ] First Unique Character
- [ ] Isomorphic Strings
- [ ] Copy List with Random Pointer

### Free Resources

1. **Video Tutorials**

   - [Hash Tables - CS50](https://www.youtube.com/watch?v=nvzVHwrrub0)
   - [Hashing - MIT OCW](https://www.youtube.com/watch?v=0M_kIqhwbFo)
   - [Hash Table Implementation - NeetCode](https://www.youtube.com/watch?v=cNWsgbKwwoU)

2. **Reading Materials**

   - [Hash Table - Wikipedia](https://en.wikipedia.org/wiki/Hash_table)
   - [GeeksforGeeks Hashing](https://www.geeksforgeeks.org/hashing-data-structure/)

3. **Practice**
   - [LeetCode Hash Table Problems](https://leetcode.com/tag/hash-table/)

---

## 4. Linked Lists

### Importance: ⭐⭐⭐⭐ (High)

### Concepts to Master

- **Singly Linked List**
- **Doubly Linked List**
- **Circular Linked List**
- **Fast and Slow Pointers (Floyd's Cycle Detection)**
- **Dummy Node Technique**
- **In-place Reversal**

### Time Complexities

| Operation      | Singly      | Doubly   |
| -------------- | ----------- | -------- |
| Access         | O(n)        | O(n)     |
| Insert at head | O(1)        | O(1)     |
| Insert at tail | O(n)/O(1)\* | O(1)     |
| Delete         | O(n)        | O(1)\*\* |
| Search         | O(n)        | O(n)     |

\*O(1) if tail pointer maintained
\*\*O(1) if node reference given

### Common Interview Problems

- [ ] Reverse Linked List
- [ ] Merge Two Sorted Lists
- [ ] Linked List Cycle (I & II)
- [ ] Remove Nth Node From End
- [ ] Reorder List
- [ ] Add Two Numbers
- [ ] Merge K Sorted Lists
- [ ] Palindrome Linked List
- [ ] Intersection of Two Linked Lists
- [ ] LRU Cache

### Free Resources

1. **Video Tutorials**

   - [Linked Lists - CS Dojo](https://www.youtube.com/watch?v=WwfhLC16bis)
   - [Linked List Problems - NeetCode](https://www.youtube.com/watch?v=G0_I-ZF0S38)
   - [Floyd's Cycle Detection - Tushar Roy](https://www.youtube.com/watch?v=zbozWoMgKW0)

2. **Reading Materials**

   - [Visualgo - Linked List](https://visualgo.net/en/list)
   - [GeeksforGeeks Linked List](https://www.geeksforgeeks.org/data-structures/linked-list/)

3. **Practice**
   - [LeetCode Linked List Problems](https://leetcode.com/tag/linked-list/)

---

## 5. Stacks

### Importance: ⭐⭐⭐⭐ (High)

### Concepts to Master

- **LIFO Principle**
- **Implementation (Array vs Linked List)**
- **Monotonic Stack**
- **Stack for Expression Evaluation**
- **Call Stack Understanding**
- **Min/Max Stack**

### Time Complexities

| Operation | Complexity |
| --------- | ---------- |
| Push      | O(1)       |
| Pop       | O(1)       |
| Peek/Top  | O(1)       |
| isEmpty   | O(1)       |

### Common Interview Problems

- [ ] Valid Parentheses
- [ ] Min Stack
- [ ] Daily Temperatures
- [ ] Evaluate Reverse Polish Notation
- [ ] Largest Rectangle in Histogram
- [ ] Basic Calculator (I, II, III)
- [ ] Decode String
- [ ] Trapping Rain Water
- [ ] Next Greater Element
- [ ] Remove K Digits

### Free Resources

1. **Video Tutorials**

   - [Stacks - mycodeschool](https://www.youtube.com/watch?v=F1F2imiOJfk)
   - [Monotonic Stack - NeetCode](https://www.youtube.com/watch?v=zx5Sw9130L0)
   - [Stack Problems - take U forward](https://www.youtube.com/watch?v=P1bAPZg5uaE)

2. **Reading Materials**

   - [GeeksforGeeks Stack](https://www.geeksforgeeks.org/stack-data-structure/)
   - [Programiz Stack](https://www.programiz.com/dsa/stack)

3. **Practice**
   - [LeetCode Stack Problems](https://leetcode.com/tag/stack/)

---

## 6. Queues

### Importance: ⭐⭐⭐⭐ (High)

### Concepts to Master

- **FIFO Principle**
- **Simple Queue**
- **Circular Queue**
- **Double-Ended Queue (Deque)**
- **Priority Queue (see Heaps)**
- **Monotonic Deque**
- **BFS Foundation**

### Time Complexities

| Operation  | Queue | Deque |
| ---------- | ----- | ----- |
| Enqueue    | O(1)  | O(1)  |
| Dequeue    | O(1)  | O(1)  |
| Front/Back | O(1)  | O(1)  |
| isEmpty    | O(1)  | O(1)  |

### Common Interview Problems

- [ ] Implement Queue using Stacks
- [ ] Implement Stack using Queues
- [ ] Sliding Window Maximum
- [ ] Design Circular Queue
- [ ] Number of Recent Calls
- [ ] Rotting Oranges
- [ ] Design Hit Counter
- [ ] Task Scheduler
- [ ] Moving Average from Data Stream
- [ ] Design Snake Game

### Free Resources

1. **Video Tutorials**

   - [Queue - mycodeschool](https://www.youtube.com/watch?v=XuCbpw6Bj1U)
   - [Deque - William Fiset](https://www.youtube.com/watch?v=5VDspKL6qmk)
   - [Monotonic Deque - NeetCode](https://www.youtube.com/watch?v=DfljaUwZsOk)

2. **Reading Materials**

   - [GeeksforGeeks Queue](https://www.geeksforgeeks.org/queue-data-structure/)
   - [Visualgo - Queue](https://visualgo.net/en/list)

3. **Practice**
   - [LeetCode Queue Problems](https://leetcode.com/tag/queue/)

---

## 7. Trees

### Importance: ⭐⭐⭐⭐⭐ (Critical)

### Types to Master

1. **Binary Tree**
2. **Binary Search Tree (BST)**
3. **Balanced BSTs**
   - AVL Tree
   - Red-Black Tree
4. **N-ary Tree**
5. **Segment Tree**
6. **Binary Indexed Tree (Fenwick Tree)**

### Concepts to Master

- **Tree Traversals**
  - Inorder, Preorder, Postorder
  - Level Order (BFS)
  - Morris Traversal (O(1) space)
- **Tree Properties**
  - Height, Depth, Diameter
  - Balanced, Complete, Full, Perfect
- **BST Operations**
  - Insert, Delete, Search
  - Predecessor, Successor
- **Lowest Common Ancestor (LCA)**
- **Tree Construction from Traversals**
- **Serialization/Deserialization**

### Time Complexities (BST)

| Operation | Average  | Worst |
| --------- | -------- | ----- |
| Search    | O(log n) | O(n)  |
| Insert    | O(log n) | O(n)  |
| Delete    | O(log n) | O(n)  |

### Common Interview Problems

- [ ] Maximum Depth of Binary Tree
- [ ] Validate Binary Search Tree
- [ ] Binary Tree Level Order Traversal
- [ ] Lowest Common Ancestor
- [ ] Binary Tree Maximum Path Sum
- [ ] Serialize and Deserialize Binary Tree
- [ ] Construct Binary Tree from Traversals
- [ ] Kth Smallest Element in BST
- [ ] Same Tree / Subtree of Another Tree
- [ ] Diameter of Binary Tree
- [ ] Invert Binary Tree
- [ ] Binary Tree Right Side View
- [ ] Path Sum (I, II, III)
- [ ] Count Good Nodes in Binary Tree
- [ ] Balanced Binary Tree

### Free Resources

1. **Video Tutorials**

   - [Trees - mycodeschool](https://www.youtube.com/playlist?list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P)
   - [Binary Trees - NeetCode](https://www.youtube.com/watch?v=OnSn2XEQ4MY)
   - [BST - Abdul Bari](https://www.youtube.com/watch?v=cySVml6e_Fc)
   - [Segment Trees - Tushar Roy](https://www.youtube.com/watch?v=ZBHKZF5w4YU)
   - [AVL Trees - MIT OCW](https://www.youtube.com/watch?v=FNeL18KsWPc)

2. **Reading Materials**

   - [Visualgo - Binary Search Tree](https://visualgo.net/en/bst)
   - [GeeksforGeeks Trees](https://www.geeksforgeeks.org/binary-tree-data-structure/)
   - [CP-Algorithms Segment Tree](https://cp-algorithms.com/data_structures/segment_tree.html)

3. **Practice**
   - [LeetCode Tree Problems](https://leetcode.com/tag/tree/)
   - [LeetCode Binary Search Tree](https://leetcode.com/tag/binary-search-tree/)

---

## 8. Heaps

### Importance: ⭐⭐⭐⭐⭐ (Critical)

### Concepts to Master

- **Min Heap and Max Heap**
- **Heap Property**
- **Heapify Operations (Sift Up/Down)**
- **Building Heap in O(n)**
- **Priority Queue Interface**
- **Two Heap Pattern**
- **K-way Merge**

### Time Complexities

| Operation       | Complexity |
| --------------- | ---------- |
| Insert          | O(log n)   |
| Extract Min/Max | O(log n)   |
| Get Min/Max     | O(1)       |
| Build Heap      | O(n)       |
| Heapsort        | O(n log n) |

### Common Interview Problems

- [ ] Kth Largest Element in an Array
- [ ] Top K Frequent Elements
- [ ] Find Median from Data Stream
- [ ] Merge K Sorted Lists
- [ ] Task Scheduler
- [ ] Reorganize String
- [ ] K Closest Points to Origin
- [ ] Sliding Window Median
- [ ] Smallest Range Covering Elements from K Lists
- [ ] Meeting Rooms II

### Free Resources

1. **Video Tutorials**

   - [Heaps - Abdul Bari](https://www.youtube.com/watch?v=HqPJF2L5h9U)
   - [Priority Queue - William Fiset](https://www.youtube.com/watch?v=wptevk0bshY)
   - [Two Heaps Pattern - NeetCode](https://www.youtube.com/watch?v=itmhHWaHupI)
   - [Heap Problems - take U forward](https://www.youtube.com/watch?v=_9RP71umU9I)

2. **Reading Materials**

   - [Visualgo - Heap](https://visualgo.net/en/heap)
   - [GeeksforGeeks Heap](https://www.geeksforgeeks.org/heap-data-structure/)

3. **Practice**
   - [LeetCode Heap Problems](https://leetcode.com/tag/heap-priority-queue/)

---

## 9. Graphs

### Importance: ⭐⭐⭐⭐⭐ (Critical)

### Representations to Master

- **Adjacency Matrix**
- **Adjacency List**
- **Edge List**
- **Implicit Graphs (Grids)**

### Concepts to Master

- **Graph Types**
  - Directed vs Undirected
  - Weighted vs Unweighted
  - Cyclic vs Acyclic
  - Connected Components
- **Traversals**
  - BFS (Breadth-First Search)
  - DFS (Depth-First Search)
- **Shortest Path**
  - Dijkstra's Algorithm
  - Bellman-Ford Algorithm
  - Floyd-Warshall Algorithm
- **Minimum Spanning Tree**
  - Prim's Algorithm
  - Kruskal's Algorithm
- **Topological Sort**
- **Cycle Detection**
- **Strongly Connected Components (Tarjan's, Kosaraju's)**
- **Bipartite Graph Check**

### Time Complexities

| Algorithm        | Time          | Space |
| ---------------- | ------------- | ----- |
| BFS              | O(V+E)        | O(V)  |
| DFS              | O(V+E)        | O(V)  |
| Dijkstra         | O((V+E)log V) | O(V)  |
| Bellman-Ford     | O(VE)         | O(V)  |
| Floyd-Warshall   | O(V³)         | O(V²) |
| Topological Sort | O(V+E)        | O(V)  |
| Kruskal          | O(E log E)    | O(V)  |
| Prim             | O((V+E)log V) | O(V)  |

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
- [ ] Redundant Connection
- [ ] Accounts Merge
- [ ] Word Search (I & II)
- [ ] Surrounded Regions
- [ ] Rotting Oranges
- [ ] Shortest Path in Binary Matrix
- [ ] Is Graph Bipartite?

### Free Resources

1. **Video Tutorials**

   - [Graph Theory Full Course - William Fiset](https://www.youtube.com/playlist?list=PLDV1Zeh2NRsDGO4--qE8yH72HFL1Km93P)
   - [Graph Algorithms - Abdul Bari](https://www.youtube.com/playlist?list=PLDN4rrl48XKpZkf03iYFl-O29szjTrs_O)
   - [Graph for Beginners - NeetCode](https://www.youtube.com/watch?v=utDu3Q7C8Ws)
   - [Graphs - MIT OCW](https://www.youtube.com/watch?v=s-CYnVz-uh4)

2. **Reading Materials**

   - [Visualgo - Graph Traversal](https://visualgo.net/en/dfsbfs)
   - [CP-Algorithms Graphs](https://cp-algorithms.com/graph/breadth-first-search.html)
   - [GeeksforGeeks Graphs](https://www.geeksforgeeks.org/graph-data-structure-and-algorithms/)

3. **Practice**
   - [LeetCode Graph Problems](https://leetcode.com/tag/graph/)

---

## 10. Tries

### Importance: ⭐⭐⭐⭐ (High)

### Concepts to Master

- **Trie Structure (Prefix Tree)**
- **Insert, Search, Delete Operations**
- **Prefix Matching**
- **Wildcard Matching**
- **Trie with HashMap vs Array**
- **Memory Optimization**

### Time Complexities

| Operation     | Complexity |
| ------------- | ---------- |
| Insert        | O(m)       |
| Search        | O(m)       |
| Prefix Search | O(m)       |
| Delete        | O(m)       |

\*m = length of the word/key

### Common Interview Problems

- [ ] Implement Trie (Prefix Tree)
- [ ] Design Add and Search Words Data Structure
- [ ] Word Search II
- [ ] Replace Words
- [ ] Longest Word in Dictionary
- [ ] Maximum XOR of Two Numbers
- [ ] Palindrome Pairs
- [ ] Search Suggestions System
- [ ] Stream of Characters

### Free Resources

1. **Video Tutorials**

   - [Trie Data Structure - Tushar Roy](https://www.youtube.com/watch?v=AXjmTQ8LEoI)
   - [Tries - NeetCode](https://www.youtube.com/watch?v=oobqoCJlHA0)
   - [Trie - William Fiset](https://www.youtube.com/watch?v=zIjfhVPRZCg)

2. **Reading Materials**

   - [Visualgo - Trie](https://visualgo.net/en/suffixtrie)
   - [GeeksforGeeks Trie](https://www.geeksforgeeks.org/trie-insert-and-search/)

3. **Practice**
   - [LeetCode Trie Problems](https://leetcode.com/tag/trie/)

---

## 11. Union-Find (Disjoint Set)

### Importance: ⭐⭐⭐⭐ (High)

### Concepts to Master

- **Find Operation with Path Compression**
- **Union Operation with Rank/Size**
- **Connected Components**
- **Cycle Detection in Undirected Graphs**
- **Dynamic Connectivity**

### Time Complexities (with optimizations)

| Operation | Complexity     |
| --------- | -------------- |
| Find      | O(α(n)) ≈ O(1) |
| Union     | O(α(n)) ≈ O(1) |
| Connected | O(α(n)) ≈ O(1) |

\*α(n) = inverse Ackermann function, effectively constant

### Common Interview Problems

- [ ] Number of Connected Components
- [ ] Redundant Connection
- [ ] Accounts Merge
- [ ] Longest Consecutive Sequence
- [ ] Graph Valid Tree
- [ ] Number of Islands II
- [ ] Satisfiability of Equality Equations
- [ ] Most Stones Removed
- [ ] Smallest String With Swaps
- [ ] Number of Operations to Make Network Connected

### Free Resources

1. **Video Tutorials**

   - [Union Find - William Fiset](https://www.youtube.com/watch?v=ibjEGG7ylHk)
   - [Disjoint Set - Abdul Bari](https://www.youtube.com/watch?v=wU6udHRIkcc)
   - [Union Find - NeetCode](https://www.youtube.com/watch?v=8f1XPm4WOUc)

2. **Reading Materials**

   - [CP-Algorithms DSU](https://cp-algorithms.com/data_structures/disjoint_set_union.html)
   - [GeeksforGeeks Union Find](https://www.geeksforgeeks.org/union-find/)

3. **Practice**
   - [LeetCode Union Find Problems](https://leetcode.com/tag/union-find/)

---

## 12. Advanced Data Structures

### Importance: ⭐⭐⭐ (Medium - For senior roles)

### Structures to Know

1. **Segment Tree**

   - Range queries (sum, min, max)
   - Point updates
   - Lazy propagation

2. **Binary Indexed Tree (Fenwick Tree)**

   - Prefix sums
   - Range sum queries
   - Point updates

3. **Skip List**

   - Probabilistic data structure
   - O(log n) operations

4. **LRU/LFU Cache**

   - Doubly linked list + HashMap
   - OrderedDict implementation

5. **Bloom Filter**

   - Probabilistic set membership
   - Space-efficient

6. **Suffix Array / Suffix Tree**
   - String matching
   - Longest repeated substring

### Free Resources

1. **Video Tutorials**

   - [Segment Tree - Tushar Roy](https://www.youtube.com/watch?v=ZBHKZF5w4YU)
   - [Fenwick Tree - William Fiset](https://www.youtube.com/watch?v=RgITNht_f4Q)
   - [LRU Cache - NeetCode](https://www.youtube.com/watch?v=7ABFKPK2hD4)
   - [Advanced DS - MIT OCW](https://www.youtube.com/watch?v=T0yzrZL1py0)

2. **Reading Materials**
   - [CP-Algorithms Advanced DS](https://cp-algorithms.com/data_structures/segment_tree.html)
   - [GeeksforGeeks Advanced DS](https://www.geeksforgeeks.org/advanced-data-structures/)

---

## Summary: Data Structures Priority Matrix

| Data Structure | Interview Frequency | Difficulty | Priority |
| -------------- | ------------------- | ---------- | -------- |
| Arrays         | ⭐⭐⭐⭐⭐          | Easy       | 1        |
| Hash Tables    | ⭐⭐⭐⭐⭐          | Easy       | 1        |
| Strings        | ⭐⭐⭐⭐⭐          | Medium     | 1        |
| Trees          | ⭐⭐⭐⭐⭐          | Medium     | 1        |
| Graphs         | ⭐⭐⭐⭐⭐          | Hard       | 1        |
| Heaps          | ⭐⭐⭐⭐            | Medium     | 2        |
| Stacks         | ⭐⭐⭐⭐            | Easy       | 2        |
| Queues         | ⭐⭐⭐⭐            | Easy       | 2        |
| Linked Lists   | ⭐⭐⭐⭐            | Medium     | 2        |
| Tries          | ⭐⭐⭐              | Medium     | 3        |
| Union-Find     | ⭐⭐⭐              | Medium     | 3        |
| Segment Tree   | ⭐⭐                | Hard       | 4        |
| Fenwick Tree   | ⭐⭐                | Hard       | 4        |

---

## Recommended Study Order

### Phase 1: Fundamentals (Weeks 1-2)

1. Arrays
2. Strings
3. Hash Tables

### Phase 2: Linear Structures (Weeks 3-4)

4. Linked Lists
5. Stacks
6. Queues

### Phase 3: Hierarchical Structures (Weeks 5-7)

7. Binary Trees
8. Binary Search Trees
9. Heaps

### Phase 4: Advanced Structures (Weeks 8-10)

10. Graphs
11. Tries
12. Union-Find

### Phase 5: Expert Level (Weeks 11-12)

13. Segment Trees
14. Advanced Graph Structures
15. System Design Data Structures

---

## Practice Platforms (Free)

1. **LeetCode** - https://leetcode.com

   - Best for interview prep
   - Company-tagged problems

2. **HackerRank** - https://hackerrank.com

   - Great for learning basics
   - Structured tracks

3. **Codeforces** - https://codeforces.com

   - Competitive programming
   - Advanced problems

4. **GeeksforGeeks** - https://practice.geeksforgeeks.org

   - Theory + Practice
   - Company-specific

5. **NeetCode** - https://neetcode.io
   - Curated 150 problems
   - Video explanations
