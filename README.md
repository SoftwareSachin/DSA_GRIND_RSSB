# 🎯 DSA Zero to Hero — Exam Edition (Rajasthan Senior Computer Instructor)

> **THE definitive DSA sheet for THIS exam format.**
> Not interview prep. Pure **MCQ-style, theory + output prediction + algorithm tracing + complexity tables**.
> Based on deep analysis of 119B & 118B papers. Every question pattern covered.

---

## 📑 Table of Contents

**PART 1 — FOUNDATIONS & COMPLEXITY (1–10)**
1. What is a Data Structure? Algorithm?
2. Abstract Data Types (ADT)
3. Linear vs Non-Linear Data Structures
4. Static vs Dynamic Data Structures
5. Asymptotic Notations — Big O, Omega, Theta
6. Complexity Comparison Tables (MEMORIZE!)
7. Best/Average/Worst Case Analysis
8. Space Complexity
9. Recurrence Relations
10. Master Theorem

**PART 2 — ARRAYS & STRINGS (11–18)**
11. Arrays — Storage, Access, Address Calculation
12. Lower Bound, Upper Bound Algorithms
13. 2D Array Address Calculation (Row-Major / Column-Major)
14. Sparse Matrix
15. String Operations
16. Pattern Matching Algorithms
17. Common Array Operations Complexity
18. Array vs Linked List Comparison

**PART 3 — STACKS (19–28)**
19. Stack — LIFO Principle
20. Stack Operations (PUSH, POP, PEEK)
21. Stack Implementation (Array vs Linked List)
22. Stack Overflow/Underflow Conditions
23. Maximum Value of Top (Critical Question Type!)
24. Infix to Postfix Conversion
25. Infix to Prefix Conversion
26. Postfix Evaluation
27. Prefix Evaluation
28. Stack Applications

**PART 4 — QUEUES (29–36)**
29. Queue — FIFO Principle
30. Queue Operations (ENQUEUE, DEQUEUE)
31. Linear Queue vs Circular Queue
32. Circular Queue Conditions (Full/Empty)
33. Deque (Double-Ended Queue)
34. Priority Queue
35. Queue Applications (Critical for Networks!)
36. Queue Implementation Complexity

**PART 5 — LINKED LISTS (37–44)**
37. Singly Linked List
38. Doubly Linked List
39. Circular Linked List
40. Linked List Operations Complexity
41. Linked List vs Array
42. Reversing a Linked List
43. Detecting Cycles (Floyd's Algorithm)
44. Common LL Interview/Exam Questions

**PART 6 — TREES (45–58)** [VERY HIGH PRIORITY]
45. Tree Terminology (Root, Leaf, Height, Depth, Level)
46. Binary Tree Types (Full, Complete, Perfect, Skewed)
47. Binary Tree Traversals — Preorder, Inorder, Postorder
48. Level-Order Traversal (BFS)
49. Building Tree from Traversals (ALWAYS ASKED!)
50. Binary Search Tree (BST)
51. BST Insertion
52. BST Deletion (Critical Pattern!)
53. AVL Trees
54. Red-Black Trees
55. B-Trees & B+ Trees
56. Heap (Max Heap, Min Heap)
57. Heap Insertion & Deletion
58. Heapify Operation

**PART 7 — GRAPHS (59–66)**
59. Graph Terminology
60. Graph Representation (Adjacency Matrix vs List)
61. BFS — Breadth First Search
62. DFS — Depth First Search
63. BFS vs DFS Comparison
64. Shortest Path Algorithms (Dijkstra, Bellman-Ford)
65. Minimum Spanning Tree (Prim's, Kruskal's)
66. Topological Sort

**PART 8 — HASHING (67–72)**
67. Hash Function Properties
68. Collision Handling — Chained Hashing
69. Collision Handling — Open Addressing
70. Chained vs Open Addressing Comparison
71. Load Factor
72. Hash Table Operations Complexity

**PART 9 — SORTING & SEARCHING (73–84)**
73. Linear Search vs Binary Search
74. When Binary Search Cannot Be Applied (TRICKY!)
75. Bubble Sort
76. Selection Sort
77. Insertion Sort
78. Quick Sort
79. Merge Sort
80. Heap Sort
81. Radix Sort, Counting Sort, Bucket Sort
82. Sorting Algorithm Comparison Table (CRITICAL!)
83. Stable vs Unstable Sorting
84. In-Place vs Out-of-Place Sorting

**PART 10 — ADVANCED TOPICS & EXAM PATTERNS (85–100)**
85. Dynamic Programming
86. Greedy Algorithms
87. Divide and Conquer
88. Branch and Bound
89. Backtracking
90. Knapsack Problem Variants (Asked in Paper!)
91. Recursion & Stack Frames
92. Tail Recursion
93. Semaphores P/V Operations (Asked!)
94. Disk Scheduling Algorithms
95. Round Robin Scheduling
96. NP-Complete vs NP-Hard
97. Algorithm Design Paradigms Summary
98. Common Exam Patterns & Tricks
99. 50 Practice MCQs (Exam-Style)
100. Final Cheat Sheet & Quick Reference

---

# 🔥 EXAM PATTERN ANALYSIS

**What this exam asks (NOT interview style):**
- ✅ Predict output of algorithm
- ✅ Trace given algorithm step-by-step
- ✅ "Which traversal gives this output?"
- ✅ "What is maximum value of top?"
- ✅ Complexity comparison (Big O vs Omega vs Theta)
- ✅ "Which is NOT a property of..."
- ✅ Postfix/Prefix conversion
- ✅ Semaphore arithmetic
- ✅ Heap operation results
- ❌ NOT: Write complete code
- ❌ NOT: Solve LeetCode

---

# 1️⃣ FOUNDATIONS & COMPLEXITY

---

## 1. What is a Data Structure? Algorithm?

**Data Structure** = a particular way of organizing data in a computer so it can be used efficiently.

**Algorithm** = step-by-step procedure to solve a problem.

### Properties of a good algorithm
1. **Input** — zero or more inputs
2. **Output** — at least one output
3. **Finiteness** — must terminate
4. **Definiteness** — each step clearly defined
5. **Effectiveness** — each step doable

### Properties of a good data structure
1. Correct representation
2. Efficient operations
3. Memory efficient
4. Reusable

> **Exam tip:** Distinguish ADT (logical) from data structure (implementation).

---

## 2. Abstract Data Types (ADT)

**ADT** = mathematical model that specifies WHAT operations are performed, not HOW.

### Examples
| ADT | Operations | Common Implementations |
|-----|-----------|------------------------|
| **List** | insert, delete, search, traverse | Array, Linked list |
| **Stack** | push, pop, peek, isEmpty | Array, Linked list |
| **Queue** | enqueue, dequeue, front | Array, Linked list |
| **Tree** | insert, delete, traverse | Array, Linked structure |
| **Graph** | addEdge, removeEdge | Matrix, List |
| **Set** | add, remove, contains | Hash table, BST |
| **Map** | put, get, remove | Hash table, BST |

**Key idea:** ADT = interface. DS = implementation.

---

## 3. Linear vs Non-Linear Data Structures

### Linear
**Elements arranged sequentially.** One-by-one connection.
- Array
- Linked List
- Stack
- Queue
- Deque

### Non-Linear
**Elements not arranged sequentially.** Hierarchical or networked.
- Tree
- Graph
- Heap
- Hash Table (debatable — some classify as linear)

### Hierarchical vs Network
- **Hierarchical** — Trees (parent-child)
- **Network** — Graphs (any-to-any)

---

## 4. Static vs Dynamic Data Structures

### Static
- **Fixed size** at compile time
- Memory allocated on stack
- Example: **Array**

### Dynamic
- **Variable size** at runtime
- Memory on heap
- Examples: **Linked List, Trees, Graphs**

| Feature | Static | Dynamic |
|---------|--------|---------|
| Size | Fixed | Variable |
| Memory | Stack | Heap |
| Access | Direct (O(1)) | Sequential (often O(n)) |
| Memory waste | If under-used | Minimal |

---

## 5. Asymptotic Notations — Big O, Omega, Theta

**MOST TESTED IN EXAM!** Memorize this completely.

### Big O (O) — Upper Bound
"At most this fast."
```
f(n) = O(g(n))  if  f(n) ≤ c·g(n)  for n ≥ n₀
```
Worst case.

### Omega (Ω) — Lower Bound
"At least this fast."
```
f(n) = Ω(g(n))  if  f(n) ≥ c·g(n)  for n ≥ n₀
```
Best case.

### Theta (Θ) — Tight Bound
"Exactly this fast."
```
f(n) = Θ(g(n))  if  c₁·g(n) ≤ f(n) ≤ c₂·g(n)
```
Average case (both upper + lower).

### Little o (o) — Strictly Upper
"Strictly slower than."
Strict inequality: f(n) < c·g(n).

### Little omega (ω) — Strictly Lower
"Strictly faster than."

### CRITICAL EXAM EXAMPLE
**Q (from paper):** For f(n) = log(n) and g(n) = √n:
- f(n) ∈ Ω(g(n))? — **NO** (log n grows slower than √n)
- g(n) ∈ Ω(f(n))? — **YES** (√n grows faster than log n)

**Answer:** f(n) ∉ Ω(g(n)), and g(n) ∈ Ω(f(n))

### 🔥 Paper Q99 — Full Worked Solution

**Q:** For defining the best time complexity, let f(n) = log(n) and g(n) = √n.
Which of the following is true?
- (A) f(n) ∈ Ω(g(n)), but g(n) ∉ Ω(f(n))
- (B) f(n) ∉ Ω(g(n)), but g(n) ∈ Ω(f(n))  
- (C) f(n) ∉ Ω(g(n)), and g(n) ∉ Ω(f(n))
- (D) f(n) ∈ Ω(g(n)), and g(n) ∈ Ω(f(n))

**Analysis:**

**Step 1:** Compare growth rates:
- For large n, √n grows MUCH FASTER than log(n)
- Example: n = 100 → log(100) ≈ 7, √100 = 10
- Example: n = 10000 → log(10000) ≈ 13, √10000 = 100
- Example: n = 10^6 → log(10^6) ≈ 20, √(10^6) = 1000

**Step 2:** Apply Big Omega definition:
- f(n) ∈ Ω(g(n)) means f grows AT LEAST AS FAST as g
- log n grows SLOWER than √n → so log(n) ∉ Ω(√n) ✓
- √n grows FASTER than log n → so √n ∈ Ω(log n) ✓

**Step 3:** Match answer:
- f(n) ∉ Ω(g(n)) ✓
- g(n) ∈ Ω(f(n)) ✓
- **Answer: (B)** ✓

### Big O vs Big Omega vs Big Theta — Memory Trick

```
f(n) = O(g(n))     ← f grows AT MOST as fast as g (upper bound)
f(n) = Ω(g(n))     ← f grows AT LEAST as fast as g (lower bound)
f(n) = Θ(g(n))     ← f grows EXACTLY as fast as g (tight bound)
```

**Quick check for two functions f and g:**
- If f grows slower → f = O(g) only
- If f grows faster → f = Ω(g) only
- If they grow at same rate → f = Θ(g)

### Growth Rate Comparison (MEMORIZE!)
```
O(1) < O(log log n) < O(log n) < O(√n) < O(n) <
O(n log n) < O(n²) < O(n³) < O(n^k) < O(2ⁿ) < O(n!) < O(nⁿ)
```

---

## 6. Complexity Comparison Tables — MEMORIZE!

### Common Function Growth

| n | log n | √n | n | n log n | n² | 2ⁿ |
|---|-------|-----|---|---------|-----|-----|
| 10 | 3 | 3 | 10 | 33 | 100 | 1024 |
| 100 | 7 | 10 | 100 | 664 | 10K | 10³⁰ |
| 1000 | 10 | 32 | 1000 | 10K | 1M | 10³⁰¹ |
| 10000 | 13 | 100 | 10000 | 130K | 100M | huge |

### Algorithm Complexity Quick Reference

| Operation | Best | Avg | Worst |
|-----------|------|-----|-------|
| **Linear Search** | O(1) | O(n) | O(n) |
| **Binary Search** | O(1) | O(log n) | O(log n) |
| **Bubble Sort** | O(n) | O(n²) | O(n²) |
| **Selection Sort** | O(n²) | O(n²) | O(n²) |
| **Insertion Sort** | O(n) | O(n²) | O(n²) |
| **Merge Sort** | O(n log n) | O(n log n) | O(n log n) |
| **Quick Sort** | O(n log n) | O(n log n) | O(n²) |
| **Heap Sort** | O(n log n) | O(n log n) | O(n log n) |
| **Radix Sort** | O(d(n+k)) | O(d(n+k)) | O(d(n+k)) |
| **Counting Sort** | O(n+k) | O(n+k) | O(n+k) |

### Data Structure Operation Complexity

| Data Structure | Access | Search | Insert | Delete |
|----------------|--------|--------|--------|--------|
| **Array** | O(1) | O(n) | O(n) | O(n) |
| **Sorted Array** | O(1) | O(log n) | O(n) | O(n) |
| **Linked List** | O(n) | O(n) | O(1)* | O(1)* |
| **Stack** | O(n) | O(n) | O(1) | O(1) |
| **Queue** | O(n) | O(n) | O(1) | O(1) |
| **Hash Table** | N/A | O(1) avg | O(1) avg | O(1) avg |
| **BST (avg)** | O(log n) | O(log n) | O(log n) | O(log n) |
| **BST (worst)** | O(n) | O(n) | O(n) | O(n) |
| **AVL/Red-Black** | O(log n) | O(log n) | O(log n) | O(log n) |
| **B-Tree** | O(log n) | O(log n) | O(log n) | O(log n) |
| **Binary Heap** | O(1) (root) | O(n) | O(log n) | O(log n) |

*if position known

### Graph Algorithm Complexity

| Algorithm | Complexity |
|-----------|-----------|
| **BFS / DFS** | O(V + E) |
| **Dijkstra (with heap)** | O((V+E) log V) |
| **Bellman-Ford** | O(VE) |
| **Floyd-Warshall** | O(V³) |
| **Prim's (with heap)** | O(E log V) |
| **Kruskal's** | O(E log E) |
| **Topological Sort** | O(V + E) |

---

## 7. Best/Average/Worst Case Analysis

### Example: Linear Search
- **Best case:** Element at first position → O(1)
- **Average case:** Element in middle → O(n/2) = O(n)
- **Worst case:** Element at end or absent → O(n)

### Example: Quick Sort
- **Best case:** Always balanced partitions → O(n log n)
- **Average case:** Random partitions → O(n log n)
- **Worst case:** Already sorted (bad pivot) → O(n²)

### Example: Insertion Sort
- **Best case:** Already sorted → O(n)
- **Worst case:** Reverse sorted → O(n²)

> **Exam trick:** When question says "in the best case," think about ideal input.

---

## 8. Space Complexity

**Memory used by algorithm.**

```
Space = Input space + Auxiliary space
```

- **Auxiliary space** = extra space used (excluding input)
- Often what we care about

### Common Space Complexities

| Algorithm | Space |
|-----------|-------|
| Iterative algorithms (loops) | O(1) usually |
| Recursive algorithms | O(depth of recursion) |
| Merge Sort | O(n) |
| Quick Sort | O(log n) average |
| BFS | O(V) |
| DFS | O(V) (recursion stack) |
| Dynamic programming | O(table size) |

---

## 9. Recurrence Relations

**Mathematical equations expressing recursive algorithm's complexity.**

### Common forms

**Merge Sort:**
```
T(n) = 2T(n/2) + O(n)
     = O(n log n)
```

**Binary Search:**
```
T(n) = T(n/2) + O(1)
     = O(log n)
```

**Linear Recursion:**
```
T(n) = T(n-1) + O(1)
     = O(n)
```

**Fibonacci (naive):**
```
T(n) = T(n-1) + T(n-2) + O(1)
     = O(2ⁿ)
```

---

## 10. Master Theorem

For recurrence: **T(n) = aT(n/b) + f(n)**, where a ≥ 1, b > 1

### Three cases

**Case 1:** If f(n) = O(n^(log_b(a) - ε))
→ T(n) = Θ(n^log_b(a))

**Case 2:** If f(n) = Θ(n^log_b(a))
→ T(n) = Θ(n^log_b(a) · log n)

**Case 3:** If f(n) = Ω(n^(log_b(a) + ε)) AND a·f(n/b) ≤ c·f(n)
→ T(n) = Θ(f(n))

### Examples

**T(n) = 2T(n/2) + n** (Merge Sort)
- a=2, b=2, f(n)=n
- log_b(a) = log_2(2) = 1
- f(n) = n = n^1 → Case 2
- **T(n) = O(n log n)** ✓

**T(n) = T(n/2) + 1** (Binary Search)
- a=1, b=2, f(n)=1
- log_b(a) = 0
- f(n) = 1 = n^0 → Case 2
- **T(n) = O(log n)** ✓

**T(n) = 4T(n/2) + n** 
- a=4, b=2, f(n)=n
- log_b(a) = 2
- f(n) = n = n^1, and 1 < 2 → Case 1
- **T(n) = O(n²)** ✓

---

# 2️⃣ ARRAYS & STRINGS

---

## 11. Arrays — Storage, Access, Address Calculation

**Array** = collection of same-type elements stored in contiguous memory.

### Properties
- Random access — O(1) via index
- Fixed size (static) in most languages
- Stored contiguously
- Cache-friendly

### Address Calculation (1D Array)

```
Address of A[i] = Base_Address + i × element_size
```

**Example:** Array A starting at 1000, each element 4 bytes
- A[0] at 1000
- A[1] at 1004
- A[5] at 1020

### With Lower Bound (LB)
If array indexed from LB:
```
Address of A[i] = Base_Address + (i - LB) × element_size
```

**Example:** A[5..10], base 2000, 4 bytes each
- A[5] at 2000
- A[7] at 2000 + (7-5)×4 = 2008

> **EXAM PATTERN:** They give base address + element size + asked index, you calculate.

---

## 12. Lower Bound, Upper Bound Algorithms

**From Paper Q63:** "LB and UB are lower and upper bound."

### Lower Bound (LB)
**Smallest index** of an array. Usually 0 (C-style) or 1 (Pascal/some math).

### Upper Bound (UB)
**Largest index** of array.

### Length of array
```
Length = UB - LB + 1
```

### Linear Search algorithm (LB to UB)
```
1. Repeat for K = LB to UB:
2.   if A[K] = ITEM:
3.     return K
4. Exit (return -1 if not found)
```

### Binary Search algorithm
```
1. Set BEG = LB, END = UB
2. While BEG ≤ END:
3.   MID = (BEG + END) / 2
4.   if A[MID] = ITEM: return MID
5.   if ITEM < A[MID]: END = MID - 1
6.   else: BEG = MID + 1
7. Exit (-1 if not found)
```

> **Exam asks:** Algorithm step traces, identifying searches/iterations.

---

## 13. 2D Array Address Calculation

### Row-Major Order (C, C++, Java)
**Rows stored consecutively.**

```
A[i][j] address = Base + ((i - LB_row) × cols + (j - LB_col)) × size
```

**Where cols = number of columns**

### Column-Major Order (FORTRAN, MATLAB)
**Columns stored consecutively.**

```
A[i][j] address = Base + ((j - LB_col) × rows + (i - LB_row)) × size
```

### Example
A[5][4] starting at 1000, each 4 bytes, row-major:
- A[2][3] at 1000 + (2×4 + 3) × 4 = 1000 + 44 = 1044

> **EXAM PATTERN:** Often asked! Memorize formulas.

---

## 14. Sparse Matrix

**Matrix with most elements = 0.**

### Storage approaches
1. **Triplet representation** — (row, col, value) for non-zero only
2. **Linked list representation**

### Why?
- Save memory
- Faster operations on non-zero only

### Example
```
   0 0 3 0
   0 5 0 0
   0 0 0 7

Triplet:
   row col val
   0   2   3
   1   1   5
   2   3   7
```

---

## 15. String Operations

### Common operations
- **Length** — strlen()
- **Concatenation** — strcat()
- **Compare** — strcmp()
- **Copy** — strcpy()
- **Substring** — strstr()
- **Reverse**
- **Pattern Match**

### Complexity
| Operation | Time |
|-----------|------|
| Length | O(n) |
| Concatenation | O(n+m) |
| Comparison | O(min(n,m)) |
| Search substring | O(n*m) naive |

---

## 16. Pattern Matching Algorithms

### Naive Pattern Matching
O(n*m) — check every position

### KMP (Knuth-Morris-Pratt)
O(n+m) — uses failure function (LPS array)

### Rabin-Karp
O(n+m) average, uses hashing

### Boyer-Moore
O(n/m) best case — fastest in practice

---

## 17. Common Array Operations Complexity

| Operation | Complexity |
|-----------|-----------|
| Access A[i] | O(1) |
| Search (unsorted) | O(n) |
| Search (sorted) | O(log n) |
| Insert at end | O(1) |
| Insert at beginning | O(n) (shift all) |
| Insert at middle | O(n) |
| Delete at end | O(1) |
| Delete at beginning | O(n) |
| Delete at middle | O(n) |
| Update A[i] | O(1) |
| Traverse | O(n) |
| Reverse | O(n) |

---

## 18. Array vs Linked List Comparison

| Feature | Array | Linked List |
|---------|-------|-------------|
| **Memory** | Contiguous | Non-contiguous |
| **Size** | Fixed (usually) | Dynamic |
| **Access** | O(1) random | O(n) sequential |
| **Insert at start** | O(n) | O(1) |
| **Insert at end** | O(1) amortized | O(n) or O(1)* |
| **Delete** | O(n) | O(1)* |
| **Memory overhead** | None | Pointer per node |
| **Cache locality** | Excellent | Poor |

*if node reference is given

---

# 3️⃣ STACKS

---

## 19. Stack — LIFO Principle

**Stack** = Last-In-First-Out (LIFO) data structure.

```
      ┌─────┐
      │  3  │ ← TOP (most recently added)
      ├─────┤
      │  2  │
      ├─────┤
      │  1  │ ← Bottom (first added)
      └─────┘
```

**Real-world examples:**
- Plate stack
- Undo in editors
- Browser back button
- Function call stack
- Recursion

---

## 20. Stack Operations

### Push (Insert)
**Add element to top.**

### Pop (Remove)
**Remove element from top.**

### Peek / Top (View)
**See top element without removing.**

### isEmpty
**Check if empty.**

### isFull
**Check if full (for array-based).**

### Complexity
All operations: **O(1)**

### Pseudocode (Array-based)

```
PUSH(item):
   if TOP == SIZE-1: OVERFLOW
   else:
      TOP = TOP + 1
      stack[TOP] = item

POP():
   if TOP == -1: UNDERFLOW
   else:
      item = stack[TOP]
      TOP = TOP - 1
      return item

PEEK():
   if TOP == -1: empty
   else: return stack[TOP]
```

---

## 21. Stack Implementation (Array vs Linked List)

### Array-Based Stack
**Pros:** Simple, cache-friendly, less overhead.
**Cons:** Fixed size.

```cpp
int stack[SIZE];
int top = -1;
```

### Linked List Stack
**Pros:** Dynamic size.
**Cons:** Memory overhead per node.

```cpp
class Node { int data; Node* next; };
Node* top = nullptr;
```

---

## 22. Stack Overflow/Underflow Conditions

### Stack Overflow
**Pushing when stack is full.**
```
if top == SIZE - 1: overflow
```

### Stack Underflow
**Popping when stack is empty.**
```
if top == -1: underflow
```

> **EXAM PATTERN Q36:** "What is max value of top that does not cause overflow?"
> If SIZE = 11, max top = **10** (indices 0-10)
> If stack uses 0-indexed array of size N, top can be 0 to N-1, so max = N-1

---

## 23. Maximum Value of Top — CRITICAL!

**Paper Q36:** 
```cpp
#define SIZE 11
struct STACK {
   int arr[SIZE];
   int top = -1;
}
```
**What would be the maximum value of top that does not cause overflow?**

### Answer
- Array has indices 0 to 10 (SIZE - 1)
- top starts at -1 (empty)
- After pushing 11 elements, top = 10
- **Maximum value of top = SIZE - 1 = 10**

**General Formula:**
```
Max top (without overflow) = SIZE - 1
```

> If question says "top = 0 means one element", count carefully!

---

## 24. Infix to Postfix Conversion

**Infix:** `A + B`
**Postfix:** `A B +`
**Prefix:** `+ A B`

### Algorithm
1. Scan infix expression left to right
2. If operand → output
3. If `(` → push to stack
4. If `)` → pop until `(`
5. If operator → pop all operators of higher/equal precedence, then push
6. End: pop all remaining operators

### Precedence
```
^   (highest)
* / %
+ -    (lowest)
```

### Example: `(A+B)*(C*D-E)*F/G`

Step-by-step:
```
Input: ( A + B ) * ( C * D - E ) * F / G

Output: A B + C D * E - * F * G /
```

### Paper Q52 actual example
**Postfix of `(A+B)*(C*D-E)*F/G`:**
- A B + C D * E - * F * G /

### Quick rule
- **Operands** keep order
- **Operators** rearranged by precedence

---

## 25. Infix to Prefix Conversion

### Algorithm
1. Reverse infix expression
2. Convert to postfix (treating reversed brackets)
3. Reverse the postfix → prefix

### Example: `A + B * C`
1. Reverse: `C * B + A`
2. Postfix: `C B * A +`
3. Reverse: `+ A * B C` ← **Prefix**

### Paper Q35/53 example: `(a+(b/c)*(d^e)-f)`
**Prefix:** `-+a*/bc^def`

### Faster method (Direct conversion)
Apply operator before its operands:
- `A+B` → `+AB`
- `A*B+C` → `+*ABC`
- `(A+B)*C` → `*+ABC`

---

## 26. Postfix Evaluation

**Use a stack.**

### Algorithm
1. Scan postfix left to right
2. If operand → push to stack
3. If operator → pop top two, apply operator, push result
4. End → top of stack is result

### Example: Evaluate `2 3 + 4 *`
```
Read 2 → push → stack: [2]
Read 3 → push → stack: [2, 3]
Read + → pop 3, pop 2, push 2+3=5 → stack: [5]
Read 4 → push → stack: [5, 4]
Read * → pop 4, pop 5, push 5*4=20 → stack: [20]
Result: 20
```

---

## 27. Prefix Evaluation

**Use a stack. Scan RIGHT TO LEFT.**

### Algorithm
1. Scan prefix right to left
2. If operand → push
3. If operator → pop two, apply (FIRST popped is FIRST operand)
4. Push result

### Example: Evaluate `+ * 2 3 4`
```
Read 4 → push → [4]
Read 3 → push → [4, 3]
Read 2 → push → [4, 3, 2]
Read * → pop 2, pop 3, push 2*3=6 → [4, 6]
Read + → pop 6, pop 4, push 6+4=10 → [10]
Result: 10
```

---

## 28. Stack Applications

1. **Function call management** (call stack)
2. **Recursion** (uses stack)
3. **Expression evaluation** (postfix/prefix)
4. **Expression conversion** (infix to postfix)
5. **Syntax parsing**
6. **Browser history** (back button)
7. **Undo/Redo** in editors
8. **Backtracking** algorithms
9. **String reversal**
10. **Balanced parentheses checking**
11. **Memory management**
12. **Compiler design** (operator stack)
13. **Tree traversals** (iterative)
14. **Graph DFS** (iterative)

---

# 4️⃣ QUEUES

---

## 29. Queue — FIFO Principle

**Queue** = First-In-First-Out (FIFO).

```
   FRONT                            REAR
     ↓                                ↓
   ┌───┬───┬───┬───┬───┐
   │ 1 │ 2 │ 3 │ 4 │ 5 │
   └───┴───┴───┴───┴───┘
   Remove from front      Add at rear
```

**Real-world examples:**
- Line at a counter
- Print queue
- Process scheduling
- BFS
- Customer service tickets

---

## 30. Queue Operations

### Enqueue (Insert at rear)
```
ENQUEUE(item):
   if rear == SIZE-1: OVERFLOW
   if front == -1: front = 0
   rear = rear + 1
   queue[rear] = item
```

### Dequeue (Remove from front)
```
DEQUEUE():
   if front == -1: UNDERFLOW
   item = queue[front]
   if front == rear: front = rear = -1
   else: front = front + 1
   return item
```

### Front / Peek
**View front without removing.**

### Complexity
All operations: **O(1)**

---

## 31. Linear Queue vs Circular Queue

### Linear Queue Problem
After dequeue, front advances but space at start is wasted.

```
Initial: [_, _, _, _, _]
Enqueue A,B,C: [A, B, C, _, _]    front=0, rear=2
Dequeue: [_, B, C, _, _]           front=1, rear=2
Even though space at start exists, can't enqueue if rear=SIZE-1!
```

### Circular Queue Solution
**Treat array as circular.** Rear wraps around.

```
   ┌───┬───┬───┬───┬───┐
   │   │   │   │   │   │
   └───┴───┴───┴───┴───┘
        ↑              ↑
       front         rear (wraps to 0)
```

### Operations (Circular Queue)
```
ENQUEUE:
   rear = (rear + 1) % SIZE

DEQUEUE:
   front = (front + 1) % SIZE
```

---

## 32. Circular Queue Conditions

### Empty
```
front == -1
```
Or: `front == rear` (with one variation)

### Full
```
(rear + 1) % SIZE == front
```

Or another common condition:
```
count == SIZE
```

### Size of Circular Queue
```
size = (rear - front + SIZE) % SIZE + 1
```

---

## 33. Deque (Double-Ended Queue)

**Insertion and deletion possible at BOTH ends.**

### Operations
- insertFront, insertRear
- deleteFront, deleteRear
- getFront, getRear

### Types
- **Input-Restricted Deque** — insert only at one end, delete at both
- **Output-Restricted Deque** — delete only at one end, insert at both

### Uses
- Browser history (forward + back)
- Sliding window problems

---

## 34. Priority Queue

**Each element has priority. Highest priority dequeued first.**

### Implementation
- **Array** — O(n) dequeue, O(1) enqueue
- **Sorted Array** — O(n) enqueue, O(1) dequeue
- **Heap** — O(log n) both! (Best!)

### Uses
- Dijkstra's algorithm
- Huffman coding
- Job scheduling (priority-based)
- A* search

---

## 35. Queue Applications

**CRITICAL — Paper Q90 asked queue applications!**

1. **Resource sharing among multiple consumers** ✓
2. **Asynchronous data transfer between processes** ✓
3. **Load balancing** ✓
4. **CPU scheduling** (Round Robin, FCFS)
5. **Disk scheduling**
6. **Print queue management**
7. **Network packet buffering**
8. **BFS in graphs**
9. **Cache implementation**
10. **Call center wait queues**

---

## 36. Queue Implementation Complexity

| Operation | Array | Linked List | Circular | Priority Queue (Heap) |
|-----------|-------|-------------|----------|----------------------|
| Enqueue | O(1) | O(1) | O(1) | O(log n) |
| Dequeue | O(n)* | O(1) | O(1) | O(log n) |
| Front | O(1) | O(1) | O(1) | O(1) |
| isEmpty | O(1) | O(1) | O(1) | O(1) |

*Linear queue dequeue requires shifting in some implementations

---

# 5️⃣ LINKED LISTS

---

## 37. Singly Linked List

**Each node has data + pointer to next.**

```
HEAD → [10|→] → [20|→] → [30|→] → NULL
```

### Node structure
```cpp
struct Node {
   int data;
   Node* next;
};
```

### Operations
- **Insert at beginning** — O(1)
- **Insert at end** — O(n) (need to traverse)
- **Insert at middle (given position)** — O(n)
- **Delete from beginning** — O(1)
- **Delete from end** — O(n)
- **Search** — O(n)
- **Traversal** — O(n)

---

## 38. Doubly Linked List

**Each node has data + next + prev pointers.**

```
NULL ← [10|↔] ↔ [20|↔] ↔ [30|↔] → NULL
```

### Pros
- Bidirectional traversal
- Easy deletion (given node)

### Cons
- Extra memory for prev pointer

---

## 39. Circular Linked List

**Last node points back to first.**

```
[10|→] → [20|→] → [30|→]
   ↑                  │
   └──────────────────┘
```

### Uses
- Round Robin scheduling
- Multiplayer games (turn order)
- Music playlist (loop)

---

## 40. Linked List Operations Complexity

| Operation | Singly | Doubly | Circular |
|-----------|--------|--------|----------|
| Access nth | O(n) | O(n) | O(n) |
| Search | O(n) | O(n) | O(n) |
| Insert at beginning | O(1) | O(1) | O(n)* |
| Insert at end | O(n) | O(n) | O(1)** |
| Delete from beginning | O(1) | O(1) | O(n)* |
| Delete given node | O(n) | O(1) | O(n) |

*Need traversal to update last pointer
**If we maintain tail pointer

---

## 41. Linked List vs Array (Critical!)

| Feature | Array | Linked List |
|---------|-------|-------------|
| Memory | Contiguous | Scattered |
| Size | Static (mostly) | Dynamic |
| Access | O(1) | O(n) |
| Insert/Delete (middle) | O(n) | O(1)* |
| Memory per element | Just data | Data + pointer(s) |
| Cache performance | Excellent | Poor |

---

## 42. Reversing a Linked List

### Iterative approach
```
prev = NULL
curr = head
while curr != NULL:
   next = curr.next
   curr.next = prev
   prev = curr
   curr = next
head = prev
```

**Time:** O(n), **Space:** O(1)

### Recursive approach
```
reverse(head):
   if head == NULL or head.next == NULL: return head
   rest = reverse(head.next)
   head.next.next = head
   head.next = NULL
   return rest
```

**Time:** O(n), **Space:** O(n) (recursion stack)

---

## 43. Detecting Cycles — Floyd's Algorithm

**Tortoise and Hare:**
- Slow pointer moves 1 step
- Fast pointer moves 2 steps
- If they meet → cycle exists
- If fast reaches NULL → no cycle

```
slow = head
fast = head
while fast != NULL and fast.next != NULL:
   slow = slow.next
   fast = fast.next.next
   if slow == fast: return true (cycle!)
return false
```

**Time:** O(n), **Space:** O(1)

---

## 44. Common LL Exam Questions

1. **Reverse linked list**
2. **Find middle node** (slow/fast pointer)
3. **Detect cycle**
4. **Find nth node from end** (two pointers)
5. **Merge two sorted lists**
6. **Remove duplicates**
7. **Check if palindrome**
8. **Add two numbers represented as lists**
9. **Intersection of two lists**
10. **Convert array to linked list and vice versa**

---

# 6️⃣ TREES — [VERY HIGH EXAM PRIORITY!]

---

## 45. Tree Terminology

```
                    A          ← Root (Level 0)
                   / \
                  B   C        ← Children of A (Level 1)
                 / \   \
                D   E   F      ← (Level 2)
               /
              G                ← (Level 3)
```

### Key terms
- **Root** — topmost node (A)
- **Parent** — node with children (A is parent of B, C)
- **Child** — node with parent (B, C are children of A)
- **Sibling** — same parent (D, E are siblings)
- **Leaf / External** — no children (G, E, F)
- **Internal node** — has at least one child (A, B, C, D)
- **Ancestor** — any node on path to root
- **Descendant** — any node in subtree
- **Edge** — connection between parent-child

### Important measurements
- **Depth of node** — # edges from root to node
- **Height of node** — # edges from node to deepest descendant
- **Height of tree** — height of root
- **Level** — depth + 1 (sometimes depth itself, depends on convention!)
- **Degree of node** — number of children
- **Degree of tree** — max degree among all nodes

### Numbers to remember
- **n nodes** → **n - 1 edges** in tree
- **Max nodes at level k** = 2^k (in binary tree, root at level 0)
- **Max nodes in binary tree of height h** = 2^(h+1) - 1

---

## 46. Binary Tree Types

### 1. Full Binary Tree
**Every node has 0 or 2 children.**
```
       A
      / \
     B   C
    / \
   D   E
```

### 2. Complete Binary Tree
**All levels filled except possibly last, last filled left-to-right.**
```
       A
      / \
     B   C
    / \  /
   D  E F
```

### 3. Perfect Binary Tree
**All internal nodes have 2 children, all leaves at same level.**
```
       A
      / \
     B   C
    / \ / \
   D  E F G
```

### 4. Skewed Binary Tree
**All nodes have only left (or only right) child.**
```
Left-skewed:    Right-skewed:
   A                A
  /                  \
 B                    B
/                      \
C                       C
```

### 5. Balanced Binary Tree
**Height difference between left and right subtrees ≤ 1 for every node.**

---

## 47. Binary Tree Traversals — CRITICAL!

```
                    A
                   / \
                  B   C
                 / \   \
                D   E   F
```

### Preorder (Root → Left → Right)
**Output: A B D E C F**

```
preorder(node):
   if node:
      visit(node)
      preorder(node.left)
      preorder(node.right)
```

### Inorder (Left → Root → Right)
**Output: D B E A C F**

```
inorder(node):
   if node:
      inorder(node.left)
      visit(node)
      inorder(node.right)
```

### Postorder (Left → Right → Root)
**Output: D E B F C A**

```
postorder(node):
   if node:
      postorder(node.left)
      postorder(node.right)
      visit(node)
```

### MEMORIZATION TRICK
- **Pre**order → root goes FIRST
- **In**order → root goes MIDDLE
- **Post**order → root goes LAST

### Special property
**Inorder of BST → sorted order**

---

## 48. Level-Order Traversal (BFS)

**Use a Queue.**

```
levelOrder(root):
   if root == NULL: return
   queue.enqueue(root)
   while queue not empty:
      node = queue.dequeue()
      visit(node)
      if node.left: queue.enqueue(node.left)
      if node.right: queue.enqueue(node.right)
```

For tree above: **A B C D E F**

---

## 49. Building Tree from Traversals — EXAM FAVORITE!

**Paper Q13:** "Post order traversal of binary tree T, given preorder ABCDEF and inorder BADCFE"

### Key rules
- **Inorder REQUIRED** (gives left/right split)
- Need ONE of: Preorder OR Postorder OR Level-order

### Algorithm (Preorder + Inorder → Postorder)

Given:
- **Preorder:** A B C D E F
- **Inorder:** B A D C F E

**Step 1:** First in preorder = root → **A**

**Step 2:** Find A in inorder: B [A] D C F E
- Left of A in inorder: **B** (left subtree)
- Right of A in inorder: **D C F E** (right subtree)

**Step 3:** From preorder, after A, next |left subtree| elements are left subtree:
- Left subtree (1 element): B → preorder of left = **B**
- Right subtree (4 elements): C D E F → preorder of right = **C D E F**

**Step 4:** Recurse on right subtree:
- Preorder: C D E F
- Inorder: D C F E
- Root = C → split: left=D, right=F E
- Right subtree: preorder D E F → wait, |left| = 1, so... 

Let me redo more carefully:

**Right subtree:** Preorder C D E F, Inorder D C F E
- Root = C (first in preorder)
- Inorder split: D | C | F E → left=D, right=FE
- |left subtree| = 1, so next 1 element after C in preorder = D
- Remaining = E F → preorder of right = E F

**Right-right subtree:** Preorder E F, Inorder F E
- Root = E
- Inorder split: F | E | (empty)
- Left = F, right = empty

**Final tree:**
```
        A
       / \
      B   C
         / \
        D   E
           /
          F
```

**Postorder = Left → Right → Root:**
- B (left of A)
- D (left of C)
- F (left of E)
- E (then root)
- C (then root of right subtree)
- A (root)

**Postorder: B D F E C A**

### Quick MEMORIZATION
- First in **preorder** = root
- Last in **postorder** = root
- Use **inorder** to split left/right subtrees

### 🔥 More Tree-Building Examples (Different Combinations!)

#### Combination 1: Postorder + Inorder → Find Preorder

**Given:**
- Postorder: D E B F C A
- Inorder: D B E A F C

**Step 1:** Last in postorder = root → **A**

**Step 2:** Inorder split around A: `D B E | A | F C`
- Left subtree inorder: D B E (3 nodes)
- Right subtree inorder: F C (2 nodes)

**Step 3:** Split postorder accordingly:
- Left subtree postorder (3 nodes): D E B
- Right subtree postorder (2 nodes): F C
- Root: A

**Step 4:** Recurse on left (postorder D E B, inorder D B E):
- Root = B (last in postorder)
- Split: D | B | E → left=D, right=E

**Step 5:** Recurse on right (postorder F C, inorder F C):
- Root = C (last)
- Split: F | C | (empty) → left=F, right=empty

**Tree:**
```
        A
       / \
      B   C
     / \  /
    D  E F
```

**Preorder = Root, Left, Right:** A B D E C F

#### Combination 2: Level-order + Inorder → Find Preorder/Postorder

**Given:**
- Level-order: A B C D E F
- Inorder: D B E A F C

**Step 1:** First in level-order = root → **A**

**Step 2:** Inorder split: `D B E | A | F C`
- Left subtree: D B E
- Right subtree: F C

**Step 3:** Find left subtree's level-order from main level-order
- From {B C D E F}, those in left subtree {D B E}: in level-order = B D E
- Right subtree level-order: C F

**Step 4:** Recurse on left (level B D E, inorder D B E):
- Root = B
- Split: D | B | E

**Step 5:** Recurse on right (level C F, inorder F C):
- Root = C
- Split: F | C |

**Same tree as before. Both work!**

### 🔑 Universal Rules

| Given | Find Root From |
|-------|---------------|
| Preorder + Inorder | First of preorder |
| Postorder + Inorder | Last of postorder |
| Level-order + Inorder | First of level-order |

**Inorder is ALWAYS required** to split into left/right subtrees.

**Cannot uniquely build** with just:
- Preorder + Postorder (ambiguous for non-full trees)
- Preorder + Level-order
- Postorder + Level-order

### Trick for Exam
When asked "which traversal CANNOT uniquely determine the tree?":
- **Without inorder**, you usually can't determine uniquely
- **With inorder** + one of (pre/post/level), you CAN

---

## 50. Binary Search Tree (BST)

**BST Property:** For every node:
- Left subtree contains values < node
- Right subtree contains values > node
- No duplicates (typically)

### Example
```
        50
       /  \
      30    70
     / \   / \
    20 40 60 80
```

### Properties
- **Inorder = sorted ascending**
- Search: O(log n) avg, O(n) worst
- Insert: O(log n) avg
- Delete: O(log n) avg

---

## 51. BST Insertion

### Algorithm
```
insert(root, key):
   if root == NULL: return new Node(key)
   if key < root.data: root.left = insert(root.left, key)
   else if key > root.data: root.right = insert(root.right, key)
   return root
```

### Example: Insert 45 in above BST
- 45 < 50 → left
- 45 > 30 → right
- 45 > 40 → right
- 40 has no right → insert here

Result:
```
        50
       /  \
      30    70
     / \   / \
    20 40 60 80
         \
         45
```

---

## 52. BST Deletion — CRITICAL!

**Paper Q34:** "If root will be deleted, the new root can be..."

### Three cases

**Case 1: Leaf node** — Just remove it.

**Case 2: One child** — Replace with that child.

**Case 3: Two children** — Replace with either:
- **Inorder successor** (smallest in right subtree)
- **Inorder predecessor** (largest in left subtree)

### Example: Delete root 50 from above BST

**Method 1: Inorder Successor (smallest in right subtree)**
- Right subtree: 70, 60, 80
- Smallest = 60
- Replace 50 with 60
- Delete 60 from old position
```
        60
       /  \
      30    70
     / \     \
    20 40    80
```

**Method 2: Inorder Predecessor (largest in left subtree)**
- Left subtree: 30, 20, 40
- Largest = 40
- Replace 50 with 40
- Delete 40 from old position
```
        40
       /  \
      30    70
     /    / \
    20   60  80
```

> **EXAM TIP:** When asked "new root can be...", both successor AND predecessor are valid answers (depends on which method used).

---

## 53. AVL Trees

**Self-balancing BST.** Named after Adelson-Velsky and Landis.

### Property
**Balance Factor = height(left) - height(right) ∈ {-1, 0, 1}**

### Rotations to restore balance
- **Left rotation**
- **Right rotation**
- **Left-Right rotation**
- **Right-Left rotation**

### Complexity
All operations: **O(log n) guaranteed**

---

## 54. Red-Black Trees

**Self-balancing BST with colored nodes (red/black).**

### Properties
1. Every node is red or black
2. Root is black
3. Every leaf (NIL) is black
4. If a node is red, both children are black
5. Every path from root to NIL has same number of black nodes

### Complexity
All operations: **O(log n)**

### Used in
- C++ `std::map`, `std::set`
- Java `TreeMap`, `TreeSet`
- Linux kernel scheduler

---

## 55. B-Trees & B+ Trees

### B-Tree
**Generalized BST where each node can have multiple children.** Used for disk-based storage (databases).

### Properties
- Each node has multiple keys
- All leaves at same level
- Self-balancing
- Order m: each node has up to m children

### B+ Tree
**Variation where:**
- All actual data stored in leaves
- Internal nodes only have keys
- Leaves linked for sequential access

### Uses
- Database indexes (MySQL InnoDB, PostgreSQL)
- File systems (NTFS, ext4)

---

## 56. Heap (Max Heap, Min Heap)

**Complete Binary Tree with Heap Property.**

### Max Heap
**Parent ≥ children.** Root is maximum.

```
       100
      /   \
     70    80
    / \   /
   30 50 60
```

### Min Heap
**Parent ≤ children.** Root is minimum.

### Array Representation
**Easy with arrays!**
- Parent of i: `(i-1) / 2`
- Left child of i: `2i + 1`
- Right child of i: `2i + 2`

```
Array: [100, 70, 80, 30, 50, 60]
Index:   0   1   2   3   4   5
```

### Used in
- Priority Queue
- Heap Sort
- Dijkstra's, Prim's algorithms
- Median finding

---

## 57. Heap Insertion & Deletion — CRITICAL!

**Paper Q80:** "Add new node 15 to leftmost leaf in right subtree, what value at leaf?"

### Insertion (Max Heap)
1. Add new element at end (next available position, left-to-right)
2. **Bubble up** — swap with parent while parent < new

### Example: Insert 90 in max heap above
```
Before: [100, 70, 80, 30, 50, 60]
Add 90: [100, 70, 80, 30, 50, 60, 90]

Position 6, parent = (6-1)/2 = 2 → arr[2] = 80
90 > 80? Yes → swap
[100, 70, 90, 30, 50, 60, 80]

Parent of 90 (at index 2): (2-1)/2 = 0 → arr[0] = 100
90 > 100? No → stop
```

### Deletion (Max Heap) — Removes Root
1. Replace root with last element
2. Reduce heap size by 1
3. **Heapify down** — swap with larger child while it's smaller

### Example: Delete root from heap above
```
Before: [100, 70, 80, 30, 50, 60]
Replace root with 60: [60, 70, 80, 30, 50]

Heapify down:
60 vs 70, 80 → larger is 80 → swap with 80
[80, 70, 60, 30, 50]

60 at index 2 has no children → done
```

### Complexity
- Insert: O(log n)
- Delete max/min: O(log n)
- Get max/min: O(1)
- Build heap: O(n)

---

## 58. Heapify Operation

**Maintain heap property at a given node.**

### Heapify Down (sift down)
For Max Heap:
```
heapify(arr, n, i):
   largest = i
   left = 2i + 1
   right = 2i + 2
   if left < n and arr[left] > arr[largest]: largest = left
   if right < n and arr[right] > arr[largest]: largest = right
   if largest != i:
      swap arr[i] and arr[largest]
      heapify(arr, n, largest)
```

### Build Heap
```
for i from n/2-1 down to 0:
   heapify(arr, n, i)
```
**O(n)** — surprisingly linear!

---

# 7️⃣ GRAPHS

---

## 59. Graph Terminology

**Graph G = (V, E)** where V = vertices, E = edges.

### Types
- **Directed (Digraph)** — edges have direction (A→B)
- **Undirected** — edges have no direction (A—B)
- **Weighted** — edges have weights
- **Unweighted** — edges have no weight
- **Cyclic** — has at least one cycle
- **Acyclic** — no cycles (DAG = directed acyclic graph)
- **Connected** — path between every pair (undirected)
- **Strongly Connected** — path both ways (directed)
- **Sparse** — few edges
- **Dense** — many edges
- **Simple** — no self-loops or parallel edges
- **Multi-graph** — allows parallel edges

### Key Numbers
- **Max edges in undirected simple graph** = n(n-1)/2
- **Max edges in directed simple graph** = n(n-1)
- **Connected graph minimum edges** = n - 1 (tree)

---

## 60. Graph Representation

### Adjacency Matrix
**2D array, matrix[i][j] = 1 if edge i-j**

```
For graph: A-B, A-C, B-C
   A B C
A  0 1 1
B  1 0 1
C  1 1 0
```

**Space:** O(V²)
**Add edge:** O(1)
**Check edge:** O(1)
**Traversal:** O(V²)

### Adjacency List
**Array of lists, each vertex's neighbors.**

```
A: [B, C]
B: [A, C]
C: [A, B]
```

**Space:** O(V + E)
**Add edge:** O(1)
**Check edge:** O(degree)
**Traversal:** O(V + E)

### Which to use?
- **Sparse graphs** → Adjacency List
- **Dense graphs** → Adjacency Matrix
- **Frequent edge queries** → Matrix

---

## 61. BFS — Breadth First Search

**Explore level-by-level.** Uses Queue.

### Algorithm
```
BFS(start):
   visited[start] = true
   queue.enqueue(start)
   while queue not empty:
      node = queue.dequeue()
      visit(node)
      for each neighbor of node:
         if not visited[neighbor]:
            visited[neighbor] = true
            queue.enqueue(neighbor)
```

### Properties
- **Shortest path** in unweighted graph
- Explores level by level
- Time: O(V + E)
- Space: O(V)

### Uses
- Shortest path (unweighted)
- Level-order traversal
- Connected components
- Web crawling
- Network broadcasting

### 🔥 CRITICAL BFS THEOREM (Paper Q27 — Asked Directly!)

**BFS Distance Property:**
> If `u` is visited BEFORE `v` during BFS traversal starting from `r`, then:
> **d(r, u) ≤ d(r, v)**

**Why?** BFS visits nodes in increasing order of distance from source.
- Level 0: source (distance 0)
- Level 1: direct neighbors (distance 1)
- Level 2: neighbors of neighbors (distance 2)
- ...

**Key points:**
- BFS guarantees nodes at distance `k` are visited BEFORE any node at distance `k+1`
- For two nodes at SAME distance, either could be visited first (depends on adjacency order)
- This is why BFS finds SHORTEST PATH in unweighted graphs

### Paper Q27 Example
**Q:** Undirected unweighted graph G. BFS started from r. If u visited before v, which is correct?
- (A) d(r,u) < d(r,v) — WRONG (could be equal)
- (B) d(r,u) > d(r,v) — WRONG (impossible)
- (C) **d(r,u) ≤ d(r,v) — CORRECT!** ✓
- (D) None of the above

**Answer: C** — BFS visits nodes in non-decreasing order of distance.

### Related BFS Properties
1. **Shortest path:** BFS finds shortest unweighted paths
2. **Level by level:** All nodes at level `k` visited before level `k+1`
3. **First visit = shortest distance:** Once a node is visited, its distance is finalized
4. **BFS tree property:** Edges in BFS tree are either tree edges (parent-child) or cross edges (same level / one level apart)

---

## 62. DFS — Depth First Search

**Go deep before backtracking.** Uses Stack (or Recursion).

### Algorithm (Recursive)
```
DFS(node):
   visited[node] = true
   visit(node)
   for each neighbor of node:
      if not visited[neighbor]:
         DFS(neighbor)
```

### Algorithm (Iterative with Stack)
```
DFS(start):
   stack.push(start)
   while stack not empty:
      node = stack.pop()
      if not visited[node]:
         visited[node] = true
         visit(node)
         for each neighbor:
            if not visited[neighbor]:
               stack.push(neighbor)
```

### Properties
- Time: O(V + E)
- Space: O(V) (visited + recursion/stack)

### Uses
- Topological sort
- Cycle detection
- Connected components
- Path finding
- Solving puzzles (mazes)

---

## 63. BFS vs DFS Comparison

| Feature | BFS | DFS |
|---------|-----|-----|
| Data structure | Queue | Stack (or recursion) |
| Memory | More | Less (for narrow trees) |
| Shortest path | Yes (unweighted) | No (in general) |
| Complete | Yes | Yes |
| Optimal | Yes (unweighted) | No |
| Tree-like exploration | Level by level | Depth-first |

---

## 64. Shortest Path Algorithms

### Dijkstra's Algorithm
**Single source shortest path. NO negative weights.**

- Greedy approach
- Uses priority queue
- Time: O((V+E) log V) with min-heap
- Space: O(V)

### Bellman-Ford Algorithm
**Single source, ALLOWS negative weights.**

- Dynamic programming
- Detects negative cycles
- Time: O(VE)
- Slower but more flexible than Dijkstra

### Floyd-Warshall
**All pairs shortest path.**

- Dynamic programming
- Time: O(V³)
- Allows negative edges (no negative cycles)

### A* Algorithm
**Like Dijkstra + heuristic.** Used in games, GPS.

---

## 65. Minimum Spanning Tree

**Subset of edges connecting all vertices with minimum total weight.**

### Prim's Algorithm
**Grow tree from one vertex.**
- Greedy
- Time: O(E log V) with heap

### Kruskal's Algorithm
**Sort edges, pick smallest that doesn't create cycle.**
- Greedy
- Uses Union-Find (Disjoint Set)
- Time: O(E log E)

### Properties
- Tree has **n-1 edges** (n = vertices)
- Tree has **no cycles**
- MST not always unique (if equal weights)

---

## 66. Topological Sort

**Linear ordering of vertices in DAG such that for every edge u→v, u comes before v.**

### Algorithms
1. **Kahn's algorithm** — uses BFS + in-degree
2. **DFS-based** — DFS, push to stack on finish, reverse

### Uses
- Course prerequisites
- Build systems (make, gradle)
- Task scheduling
- Compilation order

---

## 66B. Disjoint Set Union (DSU) / Union-Find

**Data structure to track elements in disjoint sets.** Used in Kruskal's MST.

### Operations
- **MakeSet(x)** — create a new set with just x
- **Find(x)** — find which set x belongs to (root of x's tree)
- **Union(x, y)** — merge sets containing x and y

### Implementation
```cpp
int parent[N];
int rank[N];

void makeSet(int x) {
   parent[x] = x;
   rank[x] = 0;
}

int find(int x) {
   if (parent[x] != x)
      parent[x] = find(parent[x]);  // path compression
   return parent[x];
}

void unionSets(int x, int y) {
   int px = find(x), py = find(y);
   if (px == py) return;
   // Union by rank
   if (rank[px] < rank[py]) swap(px, py);
   parent[py] = px;
   if (rank[px] == rank[py]) rank[px]++;
}
```

### Optimizations
1. **Path Compression** — flatten tree during find
2. **Union by Rank/Size** — attach smaller tree under larger

### Complexity
- With both optimizations: **O(α(n))** (inverse Ackermann, practically constant)
- Without: O(n) worst case

### Applications
- **Kruskal's MST** (detect cycles when adding edges)
- **Connected components** in graphs
- **Network connectivity**
- **Equivalence classes**

---

# 8️⃣ HASHING

---

## 67. Hash Function Properties

**Hash function:** maps key → fixed-size value (hash).

### Good hash function
1. **Uniform distribution** — keys spread evenly
2. **Deterministic** — same key → same hash
3. **Fast** — O(1)
4. **Avalanche effect** — small change → big difference
5. **Minimize collisions**

### Common hash functions
- Division method: `h(k) = k mod m`
- Multiplication method: `h(k) = floor(m × (k×A mod 1))`
- Cryptographic: SHA, MD5

---

## 68. Collision Handling — Chained Hashing

**Each bucket holds a linked list of items.**

```
   Index    Items
   ─────    ─────
     0  →   [12] → [22] → [32]
     1  →   [5]
     2  →   NULL
     3  →   [13] → [23]
```

### Advantages (Paper Q66)
- **Simple** to implement
- **No clustering**
- **Easy deletion**
- Table never gets "full"
- Performance degrades gracefully

### Disadvantages
- Extra memory for pointers
- Worst case: O(n) if all collide

---

## 69. Collision Handling — Open Addressing

**All elements stored in table itself.** On collision, probe for next empty slot.

### Probing methods

**1. Linear Probing**
```
h(k, i) = (h(k) + i) mod m
```
Issue: **Primary clustering** (consecutive occupied slots).

**2. Quadratic Probing**
```
h(k, i) = (h(k) + c₁i + c₂i²) mod m
```
Reduces primary clustering. Has **secondary clustering**.

**3. Double Hashing**
```
h(k, i) = (h₁(k) + i × h₂(k)) mod m
```
Best — minimizes clustering.

---

## 70. Chained vs Open Addressing

| Feature | Chained | Open Addressing |
|---------|---------|-----------------|
| Memory | Extra (pointers) | No extra |
| Table size | Can exceed | Must be ≥ items |
| Deletion | Easy | Hard (tombstones) |
| Clustering | None | Yes |
| Cache performance | Poor | Better |
| Resize needed | Rarely | When load factor high |

---

## 71. Load Factor

```
Load Factor α = n / m
where n = number of items, m = table size
```

### Effects
- **α small** (< 0.5): fast operations
- **α close to 1** (open addressing): many collisions
- Rule of thumb: rehash when α > 0.7

---

## 72. Hash Table Operations Complexity

| Operation | Average | Worst |
|-----------|---------|-------|
| Insert | O(1) | O(n) |
| Search | O(1) | O(n) |
| Delete | O(1) | O(n) |

**Worst case** happens when all keys hash to same bucket.

---

# 9️⃣ SORTING & SEARCHING

---

## 73. Linear Search vs Binary Search

### Linear Search
- Works on **any array** (sorted or not)
- Sequentially checks each element
- Time: O(n)
- Simple, no preprocessing

### Binary Search
- **Requires SORTED array!**
- Compare with middle, halve search space
- Time: O(log n)
- Faster but needs sorting first

### Algorithm comparison
```
Linear: A[0], A[1], A[2], ... A[n-1]
Binary: A[mid], then half left or right
```

> **Paper Q62 statement:** "Binary search is faster than linear search" — **TRUE only for sorted arrays!**

---

## 74. When Binary Search Cannot Be Applied — TRICKY!

**Paper Q62 (II):** "Binary search may not be applied on all the input lists on which linear search can be applied."

This is **TRUE!**

### Binary search requires:
1. **Sorted data** ✓
2. **Random access** (e.g., array, not linked list)
3. **Comparable elements**

### Cannot use binary search on:
- Unsorted arrays
- Linked lists (no O(1) random access)
- Data structures without index

---

## 75. Bubble Sort

**Repeatedly swap adjacent elements if wrong order.**

```
for i from 0 to n-1:
   for j from 0 to n-i-2:
      if arr[j] > arr[j+1]:
         swap

Time: O(n²)
Space: O(1)
Stable: Yes
In-place: Yes
```

### Best case (already sorted): O(n) with optimization (early exit if no swaps)

---

## 76. Selection Sort

**Find minimum, swap with first. Repeat for rest.**

```
for i from 0 to n-1:
   min_idx = i
   for j from i+1 to n-1:
      if arr[j] < arr[min_idx]: min_idx = j
   swap arr[i] and arr[min_idx]

Time: O(n²) always
Space: O(1)
Stable: No
In-place: Yes
```

---

## 77. Insertion Sort

**Build sorted portion one element at a time.**

```
for i from 1 to n-1:
   key = arr[i]
   j = i - 1
   while j >= 0 and arr[j] > key:
      arr[j+1] = arr[j]
      j = j - 1
   arr[j+1] = key

Time: O(n²) avg/worst, O(n) best
Space: O(1)
Stable: Yes
In-place: Yes
```

### Best for small arrays, nearly sorted arrays.

---

## 78. Quick Sort

**Pick pivot, partition, recurse.**

```
quicksort(arr, low, high):
   if low < high:
      pi = partition(arr, low, high)
      quicksort(arr, low, pi - 1)
      quicksort(arr, pi + 1, high)

partition(arr, low, high):
   pivot = arr[high]
   i = low - 1
   for j from low to high - 1:
      if arr[j] < pivot:
         i++
         swap arr[i] and arr[j]
   swap arr[i+1] and arr[high]
   return i + 1
```

### Complexity
- **Best:** O(n log n)
- **Avg:** O(n log n)
- **Worst:** O(n²) — when already sorted with bad pivot choice
- **Space:** O(log n) avg (recursion)

### Not stable, in-place.

---

## 79. Merge Sort

**Divide and conquer.**

```
mergeSort(arr):
   if len(arr) <= 1: return arr
   mid = len(arr) / 2
   left = mergeSort(arr[0..mid])
   right = mergeSort(arr[mid..])
   return merge(left, right)
```

### Complexity
- **All cases:** O(n log n)
- **Space:** O(n) — extra array needed
- **Stable:** Yes
- **Not in-place**

---

## 80. Heap Sort

**Build max heap, repeatedly extract max.**

```
heapSort(arr):
   buildMaxHeap(arr)
   for i from n-1 down to 1:
      swap arr[0] and arr[i]
      heapify(arr, i, 0)
```

### Complexity
- **All cases:** O(n log n)
- **Space:** O(1) — in-place!
- **Stable:** No

---

## 81. Radix Sort, Counting Sort, Bucket Sort

### Counting Sort
**For small range integers.**
- Count occurrences, build output
- Time: O(n + k) where k = range
- Space: O(n + k)
- Stable

### Radix Sort
**Sort by digits.**
- Uses Counting Sort as subroutine
- Time: O(d × (n + b)) where d = digits, b = base
- Stable

### Bucket Sort
**Distribute to buckets, sort each.**
- Time: O(n + k) average
- Worst: O(n²) if uneven distribution

---

## 82. Sorting Algorithm Comparison — MEMORIZE!

| Algorithm | Best | Avg | Worst | Space | Stable | In-place | Comparison |
|-----------|------|-----|-------|-------|--------|----------|------------|
| **Bubble** | O(n) | O(n²) | O(n²) | O(1) | Yes | Yes | Yes |
| **Selection** | O(n²) | O(n²) | O(n²) | O(1) | No | Yes | Yes |
| **Insertion** | O(n) | O(n²) | O(n²) | O(1) | Yes | Yes | Yes |
| **Merge** | O(n log n) | O(n log n) | O(n log n) | O(n) | Yes | No | Yes |
| **Quick** | O(n log n) | O(n log n) | O(n²) | O(log n) | No | Yes | Yes |
| **Heap** | O(n log n) | O(n log n) | O(n log n) | O(1) | No | Yes | Yes |
| **Counting** | O(n+k) | O(n+k) | O(n+k) | O(n+k) | Yes | No | No |
| **Radix** | O(d(n+k)) | O(d(n+k)) | O(d(n+k)) | O(n+k) | Yes | No | No |
| **Bucket** | O(n+k) | O(n+k) | O(n²) | O(n+k) | Yes | No | No |

### Special properties
- **Fastest avg:** Quick Sort, Merge Sort, Heap Sort
- **Fastest non-comparison:** Counting, Radix, Bucket (O(n))
- **Best for nearly sorted:** Insertion Sort
- **In-place comparison sort best:** Heap Sort
- **Stable + Fast:** Merge Sort

---

## 83. Stable vs Unstable Sorting

### Stable
**Preserves relative order of equal elements.**

Example: 
```
Input:  [(A, 3), (B, 1), (C, 3), (D, 2)]
Sorted by number:
Stable: [(B, 1), (D, 2), (A, 3), (C, 3)]  ← A before C (preserved)
Unstable: [(B, 1), (D, 2), (C, 3), (A, 3)] ← may swap A, C
```

### Stable sorts
- Bubble, Insertion, Merge, Counting, Radix, Bucket

### Unstable sorts
- Selection, Quick, Heap

---

## 84. In-Place vs Out-of-Place

### In-place
**O(1) extra space** (besides input).
- Bubble, Selection, Insertion, Heap, Quick (recursion stack is O(log n))

### Out-of-place
**Uses extra memory proportional to n.**
- Merge Sort, Counting, Radix, Bucket

---

# 🔟 ADVANCED TOPICS & EXAM PATTERNS

---

## 85. Dynamic Programming

**Solving problems by breaking into overlapping subproblems.**

### Two approaches
1. **Top-down (Memoization)** — recursion + cache
2. **Bottom-up (Tabulation)** — iterative, build table

### Properties needed
- **Optimal substructure** — optimal solution from optimal subproblems
- **Overlapping subproblems** — same subproblems solved multiple times

### Classic examples
- Fibonacci
- 0/1 Knapsack
- Longest Common Subsequence (LCS)
- Edit Distance
- Matrix Chain Multiplication
- Coin Change

---

## 86. Greedy Algorithms

**Make locally optimal choice at each step.**

### When works
- Optimal substructure
- Greedy choice property

### Classic examples
- Activity Selection
- Huffman Coding
- Dijkstra's
- Prim's, Kruskal's
- Fractional Knapsack

### Greedy vs DP
- **Greedy:** Make choice now, never reconsider
- **DP:** Explore all options, pick best

---

## 87. Divide and Conquer

1. **Divide** problem into subproblems
2. **Conquer** by solving recursively
3. **Combine** solutions

### Examples
- Merge Sort
- Quick Sort
- Binary Search
- Strassen's Matrix Multiplication
- Closest Pair of Points
- Karatsuba Multiplication

---

## 88. Branch and Bound

**Like backtracking but with bounding function to prune branches.**

### Used for optimization problems
- **0/1 Knapsack** (Paper Q67!)
- **Traveling Salesman Problem (TSP)**
- **Job Scheduling**

### Three branching strategies
- **FIFO** (BFS-like)
- **LIFO** (DFS-like)
- **Least cost (LC)** — best-first

---

## 89. Backtracking

**Try, fail, undo, try again.**

### Examples
- N-Queens
- Sudoku
- Maze solving
- Subset generation
- Permutations
- Graph coloring
- Hamiltonian Path

### Algorithm template
```
backtrack(state):
   if isGoal(state): return solution
   for each choice:
      make choice
      result = backtrack(state)
      if result: return result
      undo choice  ← KEY!
   return failure
```

---

## 90. Knapsack Problem Variants — Paper Q67!

### 0/1 Knapsack
- Each item: take it OR leave it
- **Cannot take fractions**
- Use: **Dynamic Programming** or **Branch and Bound**
- DP: O(n × W) where W = capacity

### Fractional Knapsack
- **Can take fraction** of item
- Use: **Greedy** (sort by value/weight ratio)
- Time: O(n log n)

### Unbounded Knapsack
- Unlimited supply of each item
- Use: DP

### Multiple Knapsack
- Multiple knapsacks
- NP-Hard

---

## 91. Recursion & Stack Frames

**Recursion uses the function call stack.**

### Each call creates a stack frame containing:
- Local variables
- Function parameters
- Return address
- Saved registers

### Types of recursion
- **Direct** — function calls itself
- **Indirect** — A calls B calls A
- **Tail recursion** — recursive call is last operation
- **Head recursion** — recursive call is first operation
- **Linear** — one recursive call per invocation
- **Tree** — multiple recursive calls (e.g., Fibonacci)

### 🔥 DETAILED RECURSION TYPES (Often Asked!)

#### 1. Direct Recursion
Function calls itself directly.
```cpp
int factorial(int n) {
   if (n == 0) return 1;
   return n * factorial(n-1);  // calls itself
}
```

#### 2. Indirect Recursion
Function A calls B, B calls A (mutual recursion).
```cpp
void A() { B(); }
void B() { A(); }
```

#### 3. Tail Recursion
Recursive call is the **LAST** operation.
```cpp
// Tail recursive
int factorial(int n, int acc = 1) {
   if (n == 0) return acc;
   return factorial(n-1, n * acc);  // last operation
}
```
**Benefit:** Compiler can optimize to loop (no stack overflow).

#### 4. Head Recursion
Recursive call is the **FIRST** operation.
```cpp
void print(int n) {
   if (n == 0) return;
   print(n - 1);     // FIRST operation
   cout << n;        // Then print
}
// Output: 1 2 3 ... n (reverse order printing)
```

#### 5. Linear Recursion
Only ONE recursive call per invocation.
```cpp
int sum(int n) {
   if (n == 0) return 0;
   return n + sum(n-1);  // one recursive call
}
```

#### 6. Tree Recursion
MULTIPLE recursive calls per invocation.
```cpp
int fib(int n) {
   if (n <= 1) return n;
   return fib(n-1) + fib(n-2);  // TWO recursive calls → tree
}
```
**Time:** O(2^n) due to branching!

### Recursion Comparison

| Type | Recursive Calls | Stack Usage | Example |
|------|----------------|-------------|---------|
| Tail | Last operation | Can optimize to O(1) | `factorial(n, acc)` |
| Head | First operation | O(n) | Reverse print |
| Linear | 1 per call | O(n) | `sum(n)` |
| Tree | 2+ per call | Exponential | Fibonacci |
| Direct | Self-call | Depends | Most recursion |
| Indirect | Via another fn | Depends | Mutual |

---

## 92. Tail Recursion

**Recursive call is the LAST statement.**

```
// Tail recursive
factorial(n, acc=1):
   if n == 0: return acc
   return factorial(n-1, n*acc)   ← LAST statement

// Not tail recursive
factorial(n):
   if n == 0: return 1
   return n * factorial(n-1)   ← multiplication after call
```

### Benefit
**Compiler can optimize to loop** (avoid stack overflow).

---

## 93. Semaphores P/V Operations — Paper Q87!

**Semaphore** = integer variable for process synchronization.

### Operations
- **P (wait/down)** — decrement; if < 0, block
- **V (signal/up)** — increment; if waiting, unblock one

### Types
- **Binary semaphore** — 0 or 1 (like mutex)
- **Counting semaphore** — any non-negative integer

### Paper Q87 Example
**Counting semaphore initialized to 8. Then 12 P + 7 V operations done.**

```
Initial: 8
After 12 P: 8 - 12 = -4
After 7 V: -4 + 7 = 3

Final value: 3
```

But wait — when value goes negative, processes are blocked!

When P performed:
- Decrement counter
- If counter < 0: block calling process (number of blocked = |counter|)

When V performed:
- Increment counter
- If counter ≤ 0: wake up one blocked process

So after 12 P operations starting from 8:
- After 8 P: counter = 0, no blocks
- 9th P: counter = -1, 1 process blocked
- 10th P: counter = -2, 2 processes blocked
- 11th P: counter = -3, 3 processes blocked
- 12th P: counter = -4, 4 processes blocked

Then 7 V operations:
- 1st V: counter = -3, unblock 1 (3 still blocked)
- 2nd V: counter = -2, unblock 1 (2 still blocked)
- 3rd V: counter = -1, unblock 1 (1 still blocked)
- 4th V: counter = 0, unblock 1 (0 blocked)
- 5th V: counter = 1
- 6th V: counter = 2
- 7th V: counter = 3

**Final semaphore value = 3**

---

## 94. Disk Scheduling Algorithms

**Decide order of servicing disk I/O requests.**

### Algorithms
1. **FCFS (First Come First Serve)** — fairest, not efficient
2. **SSTF (Shortest Seek Time First)** — closest first
3. **SCAN (Elevator)** — move head in one direction, then reverse
4. **C-SCAN (Circular SCAN)** — move one direction, jump back
5. **LOOK** — like SCAN but only go to last request
6. **C-LOOK** — circular version of LOOK

---

## 95. Round Robin Scheduling

**Each process gets a fixed time quantum.**

### Process
1. Queue of ready processes
2. Each gets time slice (e.g., 10ms)
3. If not finished, goes back to end of queue

### Properties
- Fair
- Good for time-sharing
- Performance depends on quantum size

### Used in
- OS process scheduling
- Network packet scheduling
- Robin-Round circular linked list

---

## 96. NP-Complete vs NP-Hard

### Complexity classes
- **P** — solvable in polynomial time
- **NP** — verifiable in polynomial time
- **NP-Complete** — in NP AND every NP problem reducible to it
- **NP-Hard** — every NP problem reducible to it (may not be in NP)

### Famous NP-Complete problems
- Traveling Salesman
- 0/1 Knapsack
- Boolean Satisfiability (SAT)
- Graph coloring
- Subset sum
- Hamiltonian cycle

### Open question
**P = NP?** — One of greatest unsolved problems!

---

## 97. Algorithm Design Paradigms Summary

| Paradigm | Strategy | Examples |
|----------|---------|----------|
| **Brute Force** | Try all | Linear search, naive matching |
| **Divide & Conquer** | Split + combine | Merge sort, binary search |
| **Greedy** | Local optimal | Dijkstra, Huffman, MST |
| **Dynamic Programming** | Memo subproblems | Knapsack, LCS, Fibonacci |
| **Backtracking** | Try & undo | N-Queens, Sudoku |
| **Branch & Bound** | Prune branches | TSP, 0/1 Knapsack |
| **Randomization** | Use randomness | Quick sort, randomized algorithms |
| **Approximation** | Near-optimal | Vertex cover, TSP heuristic |

---

## 98. Common Exam Patterns & Tricks

### Pattern 1: Traversal Output
**Given tree, find preorder/inorder/postorder.**
- Pre = Root, Left, Right
- In = Left, Root, Right
- Post = Left, Right, Root

### Pattern 2: Build Tree from Traversals
- First in pre = root
- Last in post = root
- Use inorder to split

### Pattern 3: Stack Max Top
- For array size N, max top = N - 1
- If question says "top initialized to -1", count carefully

### Pattern 4: Heap Insertion
- Add at end (next position L-R)
- Bubble up while parent violates property

### Pattern 5: BST Deletion
- Leaf → just remove
- One child → replace with child
- Two children → replace with successor or predecessor

### Pattern 6: Postfix Evaluation
- Operand → push
- Operator → pop 2, apply, push

### Pattern 7: Time Complexity Comparison
- Memorize growth order
- For f(n) ∈ Ω(g(n)): f grows AT LEAST as fast as g

### Pattern 8: Semaphore Arithmetic
- P decrements, V increments
- Track blocked processes when negative

### Pattern 9: Sorting Properties
- Stable: Bubble, Insertion, Merge, Counting, Radix
- Unstable: Selection, Quick, Heap
- In-place: All except Merge, Counting, Radix

### Pattern 10: Algorithm Choice
- Sparse graph + shortest path → Dijkstra (heap)
- Negative weights → Bellman-Ford
- All pairs → Floyd-Warshall
- 0/1 Knapsack → DP or Branch & Bound
- Fractional Knapsack → Greedy

---

## 99. 50 Practice MCQs — Exam Style

### Section A: Data Structures Basics

**Q1.** A stack follows which principle?
(A) FIFO  (B) LIFO  (C) Random  (D) Priority
**Ans: B**

**Q2.** Queue follows which principle?
(A) FIFO  (B) LIFO  (C) Sequential  (D) Hierarchical
**Ans: A**

**Q3.** Which is a non-linear data structure?
(A) Array  (B) Linked List  (C) Stack  (D) Tree
**Ans: D**

**Q4.** Maximum value of top in stack of size 11 (top starts at -1)?
(A) 9  (B) 10  (C) 11  (D) 12
**Ans: B**

**Q5.** Which operation adds element to stack?
(A) ADD  (B) INSERT  (C) PUSH  (D) ENQUEUE
**Ans: C**

### Section B: Trees

**Q6.** Given preorder ABDECFG, root of tree is?
(A) A  (B) B  (C) G  (D) C
**Ans: A**

**Q7.** Inorder traversal of BST gives elements in?
(A) Random order  (B) Ascending  (C) Descending  (D) Level by level
**Ans: B**

**Q8.** In max heap, root is?
(A) Minimum  (B) Maximum  (C) Middle  (D) Any
**Ans: B**

**Q9.** A complete binary tree with n nodes has height?
(A) n  (B) n-1  (C) log n  (D) floor(log₂n)
**Ans: D**

**Q10.** Number of leaves in a perfect binary tree of height h?
(A) h  (B) 2^h  (C) 2^(h+1)  (D) 2h+1
**Ans: B**

### Section C: Sorting

**Q11.** Best time complexity of bubble sort?
(A) O(1)  (B) O(n)  (C) O(n²)  (D) O(n log n)
**Ans: B** (when already sorted with optimization)

**Q12.** Worst case of quicksort?
(A) O(n log n)  (B) O(n²)  (C) O(n)  (D) O(log n)
**Ans: B**

**Q13.** Which sorting is stable?
(A) Quick  (B) Heap  (C) Merge  (D) Selection
**Ans: C**

**Q14.** Which sorting is in-place?
(A) Merge  (B) Counting  (C) Quick  (D) Radix
**Ans: C**

**Q15.** Counting sort complexity?
(A) O(n²)  (B) O(n log n)  (C) O(n+k)  (D) O(n)
**Ans: C**

### Section D: Searching

**Q16.** Binary search requires?
(A) Unsorted array  (B) Sorted array  (C) Linked list  (D) Tree
**Ans: B**

**Q17.** Time complexity of binary search?
(A) O(n)  (B) O(log n)  (C) O(n log n)  (D) O(1)
**Ans: B**

**Q18.** Linear search worst case?
(A) O(1)  (B) O(log n)  (C) O(n)  (D) O(n²)
**Ans: C**

**Q19.** Can binary search be applied to linked list efficiently?
(A) Yes  (B) No  (C) Sometimes  (D) Always
**Ans: B**

**Q20.** Hash table average search time?
(A) O(1)  (B) O(log n)  (C) O(n)  (D) O(n²)
**Ans: A**

### Section E: Graphs

**Q21.** BFS uses which data structure?
(A) Stack  (B) Queue  (C) Heap  (D) Array
**Ans: B**

**Q22.** DFS uses which data structure?
(A) Stack  (B) Queue  (C) Heap  (D) None
**Ans: A**

**Q23.** Dijkstra's algorithm fails when graph has?
(A) Cycles  (B) Negative weights  (C) Disconnected components  (D) Self loops
**Ans: B**

**Q24.** Time complexity of BFS?
(A) O(V)  (B) O(E)  (C) O(V+E)  (D) O(V²)
**Ans: C**

**Q25.** Minimum edges in connected graph with n nodes?
(A) n  (B) n-1  (C) n+1  (D) 2n
**Ans: B**

### Section F: Hashing

**Q26.** Which collision resolution does NOT cause clustering?
(A) Linear probing  (B) Quadratic probing  (C) Double hashing  (D) None
**Ans: C**

**Q27.** Chained hashing advantage?
(A) Less memory  (B) No clustering  (C) Faster search  (D) No collisions
**Ans: B**

**Q28.** Load factor for hash table?
(A) m/n  (B) n/m  (C) n+m  (D) n-m
**Ans: B** (n=items, m=table size)

**Q29.** Best case for hashing operation?
(A) O(1)  (B) O(log n)  (C) O(n)  (D) O(n²)
**Ans: A**

**Q30.** Open addressing alternative to chaining suffers from?
(A) Memory waste  (B) Clustering  (C) Slow insertion  (D) Limited keys
**Ans: B**

### Section G: Stacks & Postfix

**Q31.** Infix `A+B*C` postfix is?
(A) AB+C*  (B) ABC*+  (C) A+BC*  (D) +A*BC
**Ans: B**

**Q32.** Prefix of `A+B*C`?
(A) +AB*C  (B) +A*BC  (C) *A+BC  (D) ABC+*
**Ans: B**

**Q33.** Evaluate postfix `5 6 + 3 *`?
(A) 18  (B) 23  (C) 33  (D) 15
**Ans: C** (5+6=11, 11*3=33)

**Q34.** What's pushed first when converting infix `(A+B)` to postfix?
(A) (  (B) A  (C) +  (D) B
**Ans: A** ( goes to stack first

**Q35.** Stack overflow occurs when?
(A) top == -1  (B) top == SIZE-1  (C) top == 0  (D) Pushing to full stack
**Ans: D** (or B for array implementation)

### Section H: Complexity

**Q36.** Which grows fastest?
(A) log n  (B) √n  (C) n  (D) n²
**Ans: D**

**Q37.** Which grows slowest?
(A) log n  (B) log log n  (C) √n  (D) 2ⁿ
**Ans: B**

**Q38.** O(1) is called?
(A) Linear  (B) Constant  (C) Logarithmic  (D) Quadratic
**Ans: B**

**Q39.** For f(n) = log n, g(n) = √n. Which is true?
(A) f ∈ Ω(g)  (B) g ∈ Ω(f)  (C) Both  (D) Neither
**Ans: B**

**Q40.** Time complexity of T(n) = 2T(n/2) + n?
(A) O(n)  (B) O(n²)  (C) O(n log n)  (D) O(log n)
**Ans: C** (Merge Sort recurrence)

### Section I: Trees Advanced

**Q41.** AVL tree height balance factor range?
(A) -2 to 2  (B) -1 to 1  (C) 0 to 1  (D) -∞ to ∞
**Ans: B**

**Q42.** B-tree primarily used for?
(A) RAM operations  (B) Disk storage  (C) Cache  (D) Registers
**Ans: B**

**Q43.** In array representation of heap, left child of index i is?
(A) i-1  (B) i+1  (C) 2i+1  (D) 2i+2
**Ans: C**

**Q44.** Heap insertion complexity?
(A) O(1)  (B) O(log n)  (C) O(n)  (D) O(n log n)
**Ans: B**

**Q45.** Inorder of BST with values 50, 30, 70, 20, 40 inserted in this order?
(A) 50 30 70 20 40  (B) 20 30 40 50 70  (C) 70 50 40 30 20  (D) 20 40 30 70 50
**Ans: B** (BST inorder = sorted)

### Section J: Misc

**Q46.** Counting semaphore initialized to 5. After 8 P and 6 V operations, value is?
(A) -3  (B) 3  (C) 5  (D) 11
**Ans: B** (5-8+6 = 3)

**Q47.** Which is NOT a divide-and-conquer algorithm?
(A) Merge sort  (B) Quick sort  (C) Binary search  (D) Bubble sort
**Ans: D**

**Q48.** Knapsack 0/1 best solved by?
(A) Greedy  (B) Divide & Conquer  (C) DP or B&B  (D) Linear search
**Ans: C**

**Q49.** Fractional knapsack best solved by?
(A) Greedy  (B) DP  (C) Backtracking  (D) Divide & Conquer
**Ans: A**

**Q50.** Which problem is NOT NP-Complete?
(A) Sorting  (B) TSP  (C) SAT  (D) 0/1 Knapsack
**Ans: A** (sorting is in P)

---

### 🔥 BONUS: 25 EXAM-PATTERN MCQs (Directly from Paper Style)

**Q51.** In a binary tree with preorder ABDECF and inorder DBEACF, the postorder is:
(A) DEBFCA  (B) DEBCFA  (C) BDEFCA  (D) DEFBCA
**Ans:** Apply rules. Root=A, inorder split: DBE|A|CF. Left preorder=BDE, Right=CF.
Left tree: Root=B, inorder split: D|B|E → postorder=DEB.
Right tree: Root=C, inorder split: (empty)|C|F → postorder=FC.
Final postorder = DEB + FC + A = **DEBFCA**. **Answer: A**

**Q52.** What is max value of top in a stack of size 20 where top is initialized to -1?
(A) 18  (B) 19  (C) 20  (D) 21
**Ans: B** (indices 0-19, max top = 19)

**Q53.** Postfix of A*(B+C)/D is:
(A) ABC+*D/  (B) AB*C+D/  (C) ABC*+/D  (D) ABCD+*/
**Ans: A** (multiply A and (B+C), then divide by D)

**Q54.** Counting semaphore initialized to 10. After 15 P operations and 8 V operations, value is:
(A) 3  (B) -3  (C) 17  (D) 33
**Ans: A** (10 - 15 + 8 = 3)

**Q55.** Building a max heap from [3, 1, 6, 5, 2, 4] gives root:
(A) 1  (B) 3  (C) 6  (D) 4
**Ans: C** (max is at root in max heap)

**Q56.** BFS started from node A. Nodes visited in order: A, B, C, D, E. Distance:
(A) d(A,B) < d(A,C)  (B) d(A,B) = d(A,C)  (C) d(A,B) ≤ d(A,C)  (D) Cannot determine
**Ans: C** (BFS visits in non-decreasing distance order)

**Q57.** Deleting root from BST {50, 30, 70, 20, 40, 60, 80}, new root can be:
(A) 30 or 70  (B) 40 or 60  (C) 20 or 80  (D) Any of 30, 40, 60, 70
**Ans: B** (inorder predecessor=40 OR successor=60)

**Q58.** Time complexity of building heap from n elements:
(A) O(n)  (B) O(n log n)  (C) O(log n)  (D) O(n²)
**Ans: A** (heapify-down from n/2 to 0 is O(n))

**Q59.** Which is TRUE about chained hashing vs open addressing?
(A) Open is faster  (B) Chained needs less memory  (C) Chained handles collisions gracefully  (D) Open never has clustering
**Ans: C** (chained has no clustering, deletion is easy)

**Q60.** Best time complexity for searching in a sorted array of n elements:
(A) O(1)  (B) O(log n)  (C) O(n)  (D) O(n log n)
**Ans: A** (when element is at the middle position checked first)

**Q61.** Number of edges in a complete graph with n vertices (undirected):
(A) n  (B) n-1  (C) n(n-1)/2  (D) n²
**Ans: C**

**Q62.** Which sorting algorithm has best space complexity?
(A) Merge Sort  (B) Quick Sort  (C) Heap Sort  (D) Counting Sort
**Ans: C** (O(1) in-place)

**Q63.** Recursive function `f(n) = f(n-1) + f(n-2)` has time complexity:
(A) O(n)  (B) O(n²)  (C) O(2ⁿ)  (D) O(log n)
**Ans: C** (Fibonacci, exponential)

**Q64.** In a complete binary tree with 100 nodes, height is:
(A) 6  (B) 7  (C) 50  (D) 99
**Ans: A** (⌊log₂(100)⌋ = 6, height starts at 0)

**Q65.** Postfix evaluation of `3 4 + 2 *` gives:
(A) 10  (B) 14  (C) 7  (D) 11
**Ans: B** (3+4=7, 7*2=14)

**Q66.** Tail recursion vs head recursion difference:
(A) Tail uses more memory  (B) Head can be optimized to loop  (C) Tail can be optimized to loop  (D) Same
**Ans: C**

**Q67.** Knapsack problem (0/1) can be optimally solved using:
(A) Greedy  (B) Dynamic Programming  (C) Linear search  (D) Bubble sort
**Ans: B** (DP gives optimal; greedy fails for 0/1)

**Q68.** Disjoint Set Union with path compression and union by rank has complexity:
(A) O(1)  (B) O(α(n))  (C) O(log n)  (D) O(n)
**Ans: B** (inverse Ackermann, near-constant)

**Q69.** A graph with n nodes and exactly n-1 edges, connected, is a:
(A) Cyclic graph  (B) Tree  (C) Complete graph  (D) Disconnected
**Ans: B**

**Q70.** In double hashing, h(k, i) =:
(A) h1(k) + i  (B) h1(k) + i²  (C) h1(k) + i × h2(k)  (D) h1(k) × i
**Ans: C**

**Q71.** Quick sort worst case occurs when:
(A) Array is random  (B) Array is sorted ascending  (C) Array has all equal elements  (D) All of these can cause it
**Ans: D** (depends on pivot strategy)

**Q72.** Which traversal gives BST elements in descending order?
(A) Preorder  (B) Inorder  (C) Postorder  (D) Reverse inorder (Right→Root→Left)
**Ans: D**

**Q73.** Critical section problem in OS is solved using:
(A) Stacks  (B) Queues  (C) Semaphores  (D) Trees
**Ans: C**

**Q74.** A binary tree with n leaves has at least how many total nodes?
(A) n  (B) 2n  (C) 2n-1  (D) n+1
**Ans: C** (full binary tree minimum)

**Q75.** Which is NOT a stable sort?
(A) Bubble  (B) Merge  (C) Heap  (D) Insertion
**Ans: C**

---

## 100. Final Cheat Sheet & Quick Reference

### MUST-MEMORIZE TABLES

#### Sorting at a Glance
```
Algorithm    Best       Avg        Worst      Space      Stable
Bubble       O(n)       O(n²)      O(n²)      O(1)       Yes
Selection    O(n²)      O(n²)      O(n²)      O(1)       No
Insertion    O(n)       O(n²)      O(n²)      O(1)       Yes
Merge        O(nlogn)   O(nlogn)   O(nlogn)   O(n)       Yes
Quick        O(nlogn)   O(nlogn)   O(n²)      O(logn)    No
Heap         O(nlogn)   O(nlogn)   O(nlogn)   O(1)       No
Counting     O(n+k)     O(n+k)     O(n+k)     O(n+k)     Yes
Radix        O(d(n+k))  O(d(n+k))  O(d(n+k))  O(n+k)     Yes
```

#### Data Structure Complexities
```
DS           Access    Search    Insert    Delete
Array        O(1)      O(n)      O(n)      O(n)
Sorted Arr   O(1)      O(logn)   O(n)      O(n)
Stack        O(n)      O(n)      O(1)      O(1)
Queue        O(n)      O(n)      O(1)      O(1)
LL           O(n)      O(n)      O(1)*     O(1)*
BST avg      O(logn)   O(logn)   O(logn)   O(logn)
Hash         -         O(1)      O(1)      O(1)
AVL          O(logn)   O(logn)   O(logn)   O(logn)
Heap         -         O(n)      O(logn)   O(logn)
```

#### Tree Traversals
```
Preorder:  Root, Left, Right
Inorder:   Left, Root, Right    (BST → sorted)
Postorder: Left, Right, Root
Level:     BFS, uses queue
```

#### Heap Properties
```
Max heap: parent ≥ children, root = max
Min heap: parent ≤ children, root = min
Array: parent(i) = (i-1)/2, left(i) = 2i+1, right(i) = 2i+2
```

#### Graph Algorithms
```
BFS:           O(V+E), shortest path unweighted
DFS:           O(V+E)
Dijkstra:      O((V+E)logV), no negative weights
Bellman-Ford:  O(VE), allows negative
Floyd-Warshall: O(V³), all pairs
Prim's:        O(ElogV)
Kruskal's:     O(ElogE)
```

#### Asymptotic Order (MEMORIZE!)
```
O(1) < O(loglogn) < O(logn) < O(√n) < O(n) <
O(nlogn) < O(n²) < O(n³) < O(2ⁿ) < O(n!) < O(nⁿ)
```

### Quick Conversion Rules

**Infix to Postfix:**
- Operand → output
- Operator → stack (pop higher priority first)
- ( → push
- ) → pop until (

**Infix to Prefix:**
- Reverse infix
- Convert to postfix (with brackets reversed)
- Reverse result

**Postfix Evaluation:**
- Operand → push
- Operator → pop 2, apply, push

**Prefix Evaluation:** 
- Scan right to left
- Same rules

### Common Tricks

1. **Stack overflow** = pushing to full → top == SIZE-1
2. **Stack underflow** = popping empty → top == -1
3. **Queue empty** = front == -1
4. **Queue full (linear)** = rear == SIZE-1
5. **Circular queue full** = (rear+1)%SIZE == front
6. **BST inorder** = sorted ascending
7. **Heap is a complete tree** but NOT a BST
8. **Binary tree** ≠ **Binary search tree**
9. **MST has** n-1 edges for n vertices
10. **Tree** has exactly n-1 edges for n vertices

---

# 🎯 EXAM SUCCESS FRAMEWORK

### Time Strategy (15-20 DSA questions in exam)
- 90 seconds per question max
- Skip if unsure (negative marking!)
- Mark and return

### Question Type Approach

**Type 1: Output Prediction**
- Carefully trace step by step
- Use pencil/paper
- Don't rush

**Type 2: Complexity Questions**
- Apply standard formulas
- Memorize sorting table
- Know growth order

**Type 3: Algorithm Properties**
- Remember stable/unstable lists
- In-place properties
- Best/worst cases

**Type 4: Conversion (Infix/Prefix/Postfix)**
- Practice 5-10 examples
- Use stack mental model

**Type 5: Tree Building from Traversals**
- Find root first
- Split using inorder
- Recurse

**Type 6: Heap Operations**
- Track array indices
- Apply bubble up/down

### Last 24 Hours Before Exam
1. Review this complete sheet
2. Memorize all comparison tables
3. Practice 5 traversal problems
4. Solve 3 postfix conversions
5. Review semaphore P/V

### Last 1 Hour Before Exam
1. Glance at quick reference (Section 100)
2. Mentally rehearse:
   - Sorting properties
   - Tree traversals
   - Stack/Queue rules
   - BFS/DFS basics

---

# 💪 FINAL MINDSET

> **Master these:**
> 1. **Asymptotic notation** — Big O, Omega, Theta
> 2. **Sorting comparison table** — all properties
> 3. **Tree traversals** — pre, in, post (with examples)
> 4. **Tree building from traversals**
> 5. **Stack operations + overflow conditions**
> 6. **Postfix/Prefix conversion + evaluation**
> 7. **BST insertion/deletion rules**
> 8. **Heap insertion/deletion**
> 9. **Hashing — chained vs open addressing**
> 10. **BFS/DFS + when to use which**
> 11. **Graph algorithms (Dijkstra, BFS, DFS) complexities**
> 12. **Semaphore arithmetic**
> 13. **Time complexity of common algorithms**
> 14. **Recurrence relations and Master theorem**
> 15. **Algorithm paradigms** (DP, Greedy, D&C, B&B)
>
> **This single sheet covers EVERY DSA question pattern in your exam.**
> **Practice the 50 MCQs. Memorize the tables. Trust the patterns.**
> **You WILL ace the DSA section.** 🎯🚀

---

# ✅ FINAL VERIFICATION: PAPER COVERAGE CHECKLIST

> **EVERY DSA-related question from Paper 119B (June 2022) and Paper 118B (June 2022) verified covered in this sheet.**

## Paper 119B (June 13, 2022) — DSA Questions Coverage

| Question | Topic | Section in Sheet |
|----------|-------|------------------|
| Q27 | BFS distance property | Section 61 (BFS Theorem) ✅ |
| Q35 | Equation prefix notation | Section 25 ✅ |
| Q36 | Stack max value of top | Section 23 ✅ |
| Q38 | Queue principle (FIFO) | Section 29 ✅ |
| Q52 | Postfix conversion | Section 24 ✅ |
| Q63 | LB/UB algorithm | Section 12 ✅ |
| Q66 | Chained hashing | Section 68 ✅ |
| Q67 | Knapsack problem | Section 90 ✅ |
| Q80 | Heap insertion | Section 57 ✅ |
| Q87 | Counting semaphore P/V | Section 93 ✅ |
| Q90 | Queue applications | Section 35 ✅ |
| Q97 | Stack push operation | Section 20 ✅ |
| Q98 | Scheduling matching | Section 94 ✅ |
| Q99 | log n vs √n complexity | Section 5 (detailed!) ✅ |

## Paper 118B (June 18, 2022) — DSA Questions Coverage

| Question | Topic | Section in Sheet |
|----------|-------|------------------|
| Q13 | Tree post-order from pre+in | Section 49 (with 3 examples!) ✅ |
| Q22 | Prefix expression | Section 25 ✅ |
| Q34 | BST root deletion | Section 52 ✅ |
| Q35 | Prefix notation | Section 25 ✅ |
| Q44 | Sorting algorithms | Section 75-84 ✅ |
| Q62 | Binary vs linear search | Section 73-74 ✅ |
| Q63 | LB/UB algorithm | Section 12 ✅ |
| Q66 | Chained hashing advantages | Section 68 ✅ |
| Q67 | Knapsack | Section 90 ✅ |
| Q80 | Max heap leaf values | Section 57 ✅ |
| Q87 | Semaphore arithmetic | Section 93 ✅ |
| Q97 | Stack insertion (PUSH) | Section 20 ✅ |
| Q98 | Scheduling match | Section 94 ✅ |
| Q99 | log n vs √n | Section 5 ✅ |

## 🔥 CRITICAL TOPICS — All Verified Present

✅ **Asymptotic notations** (Big O, Ω, Θ) with worked Paper Q99 example
✅ **Complexity comparison tables** — All sorting algorithms
✅ **Tree traversals** — All 4 types (Pre/In/Post/Level)
✅ **Tree building from traversals** — 2+ worked examples (Pre+In, Post+In)
✅ **BST insertion + deletion** — Both successor and predecessor methods
✅ **Heap operations** — Insertion, deletion, heapify with array indices
✅ **Stack operations** — PUSH/POP/PEEK with overflow/underflow conditions
✅ **Max value of top** — Formula and explanation (Paper Q36)
✅ **Infix↔Postfix↔Prefix** — Conversion + evaluation
✅ **Queue applications** — All 10 applications (Paper Q90)
✅ **BFS distance theorem** — Paper Q27 exact answer
✅ **Hash collision** — Chained vs Open addressing comparison
✅ **Binary search prerequisites** — When NOT to use
✅ **Semaphore P/V arithmetic** — Step-by-step blocking explanation
✅ **Knapsack variants** — 0/1 (DP/B&B), Fractional (Greedy)
✅ **Recursion types** — 6 types with examples
✅ **DSU/Union-Find** — Bonus addition for completeness
✅ **75 Practice MCQs** — Including 25 BONUS exam-style questions

## 🎯 Topics Also Covered

- **Tree height/depth formulas** ✅ Section 45
- **Number of edges in tree** ✅ Section 45 (n-1 edges)
- **Complete vs Full vs Perfect tree** ✅ Section 46
- **Time complexity of common algorithms** ✅ Section 6 (table)
- **Recurrence relations** ✅ Section 9, 10
- **Master Theorem** ✅ Section 10 with worked examples
- **Algorithm paradigms** ✅ Section 97
- **NP-Complete vs P** ✅ Section 96
- **Algorithm trace examples** ✅ Multiple examples
- **Stable vs Unstable sorting** ✅ Section 83
- **In-place sorting** ✅ Section 84
- **Pattern matching** ✅ Section 16 (KMP, Rabin-Karp)
- **2D Array address calculation** ✅ Section 13 (row-major/col-major)

## 💪 HONEST ASSESSMENT

**With this single sheet, you will:**
- ✅ Recognize every DSA pattern in the paper
- ✅ Apply correct formulas (heap indices, address calculation, etc.)
- ✅ Trace algorithms step-by-step
- ✅ Compare complexities accurately
- ✅ Solve postfix/prefix conversions confidently
- ✅ Build trees from given traversals
- ✅ Handle semaphore arithmetic
- ✅ Identify scheduling algorithm properties
- ✅ Apply BFS/DFS theorems
- ✅ Choose right algorithm for given problem

**What this sheet WILL NOT do:**
- ❌ Cover specific Rajasthan-only topics outside CS (separate analysis sheet)
- ❌ Replace 5-10 past paper practices
- ❌ Make you faster without timing practice

**Recommendation:**
1. Read entire sheet ONCE thoroughly (4-6 hours)
2. Memorize all comparison tables in Section 100
3. Solve all 75 practice MCQs
4. Re-do the actual paper questions and check against sheet
5. Time yourself on past papers

**Bro, you ARE prepared. Trust the preparation. Execute on exam day.** 🚀💪
