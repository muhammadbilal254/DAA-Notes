# Topics

```
DESIGN ANALYSIS OF ALGORITHM
Final Paper IMP

1.	Introduction of DAA ✅
2.	Role of algorithm in computer ✅
3.	Analysis of algorithm ✅
4.	Sorting of algorithm ✅
5.	Amortized analysis of algorithms ✅
6.	Algorithm design techniques (only 4) ✅
.	Brute-Force Search
.	Divide and Conquer ✅
.	Greedy Algorithm
.	Dynamic Programming
.	Branch and Bound Algorithm ✅
.	Randomized Algorithm ✅
.	Backtracking Algorithms ✅
7.	Hashing ✅
8.	MST
9.	Graph algorithm ✅

```

# Algorithm:

An algorithm is a step-by-step procedure or set of rules designed to solve a specific problem or perform a particular task. It is a finite sequence of well-defined instructions that, when executed, produces a desired output.
**Example** : Linear Search, Binary Search, Bubble Sort.

## Algorithmic Techniques:

**1. Divide and Conquer:**

- _Definition:_ Divide a problem into smaller sub-problems, solve them independently, and then combine the solutions.
- _Example:_ Merge Sort - Divide an array into two halves, recursively sort each half, and merge the sorted halves.

**2. Backtracking:**

- _Definition:_ Systematically try different possibilities until a solution is found, undoing incorrect choices along the way.
- _Example:_ Sudoku Solver - Fill the grid row by row, backtrack when a wrong number is placed, and try alternative numbers.

**3. Branch and Bound:**

- _Definition:_ Divide the problem space into branches, explore each branch, and use pruning techniques to eliminate unpromising branches.
- _Example:_ Traveling Salesman Problem - Explore possible routes, eliminate those with higher costs early, and find the most efficient route.

**4. Randomized Algorithms:**

- _Definition:_ Use randomness to make algorithmic choices, providing a probabilistic rather than deterministic solution.
- _Example:_ QuickSort - Randomly choose a pivot element for partitioning, reducing the likelihood of worst-case scenarios, leading to efficient sorting.

---

# Hashing

Hashing is a process of mapping data of variable size to a fixed-size value using a hash function, producing a unique identifier, or hash code. This technique is commonly employed for indexing and quick data retrieval.
**Uses**: Fast Data Retrieval, Unique Identification:, Security, Distributed Systems, Optimized Searching.

## popular hash Function

1. Divide Method [ h(k) = k % m ]
2. Folding Method
3. Mid Square Method

## COLLISION

If two keys map on the same hash table index then we have a collision.
Two approaches are used to resolve collisions.

1. Open Hashing
   - Separate Chaining
2. Close hashing (Open Addressing)
   - Linear Probing [H <sub>i</sub> (x) = H(x)% m + i]
   - Quadratic Probing [H <sub>i</sub> (x) = H(x)% m + i^2]
   - Double hashing [H' = h + i*h],[[h(k) = k % m ], [h = m - (k % m)]]

---

# Graph Algoritms

A graph is a data structure that consists of a set of vertices (nodes) connected by edges (lines). It is used to represent relationships and connections between different objects or entities.Vertices can represent any kind of object or entity, while edges represent the relationships between those objects.

## Dept First Search [Stack Process]

Depth First Search (DFS) is an algorithm used to traverse or search a graph. It explores as far as possible along each branch before backtracking.

**Rules:**

1. Visit a vertex (node).
2. Explore all the unvisited neighbors of the current vertex.
3. Mark the current vertex as visited.
4. Backtrack if there are no more unvisited neighbors.

## Breadth First Search [Queue Process]

Breadth First Search (BFS) is an algorithm used to traverse or search a graph. It explores all the vertices of a graph in breadth-first order, i.e., visiting all the neighbors before visiting the children.

**Rules**

1. Enqueue the starting vertex.
2. Dequeue a vertex from the queue and visit it.
3. Enqueue all its unvisited neighbors.
4. Repeat steps 2 and 3 until the queue is empty.

---

# Role of algorithm in computer

1. **Problem Solving:** Algorithms provide systematic approaches for computers to solve diverse problems efficiently.

2. **Task Automation:** They enable computers to automate tasks by specifying a sequence of steps to be executed.

3. **Data Processing:** Algorithms govern the manipulation and processing of data, facilitating information management.

4. **Decision Making:** Computers use algorithms to make logical decisions based on input conditions or criteria.

5. **Efficiency:** Algorithms optimize computational processes, ensuring tasks are performed with minimal resources.

6. **Versatility:** Algorithms are applicable across various domains, from data analysis to artificial intelligence.

7. **Foundation of Software:** Algorithms form the core logic behind software applications, driving their functionality.

8. **Computational Complexity:** They address efficiency and scalability concerns, determining how quickly problems can be solved.

## Analysis of Algorithms

Analysis of algorithms involves evaluating the performance and efficiency of algorithms concerning factors such as time complexity, space complexity, and scalability. It helps in understanding how an algorithm behaves as input sizes increase.

1. **Time Complexity Analysis:**

   - _Definition:_ Evaluates the amount of time an algorithm takes to complete as a function of the input size.
   - _Example:_ Bubble sort has a time complexity of O(n^2) in the worst case, indicating a quadratic relationship with the input size.

2. **Space Complexity Analysis:**

   - _Definition:_ Measures the amount of memory an algorithm uses as a function of the input size.
   - _Example:_ Merge sort has a space complexity of O(n), indicating linear space usage for the input size.

3. **Best, Worst, and Average Case Analysis:**

   - _Definition:_ Examines the algorithm's performance in different scenarios - best (ideal conditions), worst (unfavorable conditions), and average cases.
   - _Example:_ QuickSort has an average-case time complexity of O(n log n) but a worst-case of O(n^2) when not well-pivoted.

4. **Amortized Analysis:**

   - _Definition:_ Analyzes the average performance of an algorithm over a sequence of operations, providing a more realistic view.
   - _Example:_ Dynamic array resizing in a list involves occasional expensive operations, but amortized analysis shows that, on average, each insertion is O(1).

5. **Empirical Analysis:**

   - _Definition:_ Involves running experiments and measuring the actual performance of an algorithm on real-world inputs.
   - _Example:_ Testing sorting algorithms on various datasets to observe their behavior in practice.

6. **Comparative Analysis:**

   - _Definition:_ Compares multiple algorithms to determine their relative performance and advantages in specific contexts.
   - _Example:_ Comparing different sorting algorithms like Bubble Sort, Merge Sort, and QuickSort to choose the most efficient for a particular use case.

7. **Algorithmic Paradigms:**
   - _Definition:_ Refers to overarching strategies or approaches used to solve problems, guiding the design and analysis of algorithms.
   - _Example:_ Divide and Conquer (e.g., Merge Sort), Greedy Algorithms (e.g., Dijkstra's algorithm), and Dynamic Programming (e.g., Fibonacci sequence) are algorithmic paradigms.

## Nature of Input and Output:\*\*

1. **Nature of Input:**

   - _Definition:_ Describes the characteristics and format of the data provided to an algorithm or system.
   - _Example:_ For a sorting algorithm, the nature of input might involve the type of data (numeric, alphabetical), its initial order, and any specific patterns.

2. **Nature of Output:**
   - _Definition:_ Specifies the expected form and content of the result produced by an algorithm or system.
   - _Example:_ In a searching algorithm, the nature of output could be the index or location of the target element in the input data.

**Size of Input:**

1. **Size of Input:**
   - _Definition:_ Refers to the quantity or scale of the data provided as input to an algorithm or system.
   - _Example:_ For a graph traversal algorithm, the size of input might be the number of nodes and edges in the graph.

## Asymptotic notations:

(such as Big O, Omega, and Theta) are used to describe the upper and lower bounds of an algorithm's time or space complexity as the input size grows to infinity.

```
Big O : worst case upper bound

Omega: best case Lower bound

Theta: both

little o : upper bound not tight

little omega: lower bound not tight
```

## Sorting of Algorithm

1. **Bubble Sort** [ TimeComplexity: O(n^2) in the worst and average cases ]
   Bubble Sort is a simple sorting algorithm that repeatedly steps through the list, compares adjacent elements, and swaps them if they are in the wrong order. The pass through the list is repeated until no swaps are needed, indicating that the list is sorted.

- **Algorithm Steps:**
  1. Compare adjacent elements in the list.
  2. Swap them if they are in the wrong order.
  3. Repeat these steps until no more swaps are needed.
  4. The list is now sorted.
- **Example:**
  - Input: [4, 2, 7, 1, 9]
  - Pass 1: [2, 4, 1, 7, 9]
  - Pass 2: [2, 1, 4, 7, 9]
  - Pass 3: [1, 2, 4, 7, 9]
  - The sorted list: [1, 2, 4, 7, 9]

Bubble Sort has a time complexity of O(n^2) in the worst case, making it less efficient for large datasets compared to more advanced sorting algorithms.

2. **Selection Sort** [Time Complexity: O(n^2) in all cases ]

Selection Sort is a simple sorting algorithm that divides the input list into two parts: a sorted and an unsorted region. It repeatedly selects the smallest (or largest, depending on the order) element from the unsorted region and swaps it with the first element of the unsorted region.

- **Algorithm Steps:**

  1. Divide the list into sorted and unsorted regions.
  2. Find the minimum element in the unsorted region.
  3. Swap the minimum element with the first element of the unsorted region.
  4. Expand the sorted region and repeat steps 2-3 until the entire list is sorted.

- **Example:**
  - Input: [4, 2, 7, 1, 9]
  - Pass 1: [1, 2, 7, 4, 9]
  - Pass 2: [1, 2, 7, 4, 9]
  - Pass 3: [1, 2, 4, 7, 9]
  - The sorted list: [1, 2, 4, 7, 9]

Selection Sort has a time complexity of O(n^2) in the worst case and is not the most efficient for large datasets but is simple to understand and implement.

3. **Insertion Sort** [Time Complexity : O(n^2) in the worst case but can be O(n) in the best case]
   **Insertion Sort:**
   Insertion Sort is a simple sorting algorithm that builds the final sorted list one element at a time. It takes each element from the unsorted part of the list and inserts it into its correct position in the sorted region.

- **Algorithm Steps:**

  1. Divide the list into sorted and unsorted regions.
  2. Take an element from the unsorted region.
  3. Insert the element into its correct position in the sorted region.
  4. Repeat steps 2-3 until the entire list is sorted.

- **Example:**
  - Input: [4, 2, 7, 1, 9]
  - Pass 1: [2, 4, 7, 1, 9]
  - Pass 2: [2, 4, 7, 1, 9]
  - Pass 3: [1, 2, 4, 7, 9]
  - The sorted list: [1, 2, 4, 7, 9]

Insertion Sort is efficient for small datasets and nearly sorted lists, with a time complexity of O(n^2) in the worst case. It has a simple implementation and is often used for educational purposes.

4. **Merge Sort** [ Time Complexity: O(n log n) in all cases. ]
5. **Quick Sort** [Time Complexity: O(n^2) in the worst case, but average case is O(n log n). ]
6. **Heap Sort** [ Time Complexity: O(n log n) in all cases. ]
7. **Radix Sort** [ Time Complexity: O(nk) for n elements with k being the number of digits or characters. ]

---

**Amortized Algorithms:**
Amortized analysis is a method for analyzing the average time complexity of a sequence of operations, even if individual operations might have different time complexities. It provides a more accurate understanding of the overall performance.

**Techniques:**

1. **Aggregate Analysis:**

   - _Definition:_ Evaluate the total cost of a sequence of operations and then determine the average cost per operation.
   - _Example:_ Dynamic array resizing - occasional expensive resizing is amortized over a sequence of insertions.

2. **Accounting Method:**

   - _Definition:_ Assign "credits" to inexpensive operations and use them to pay for more costly operations.
   - _Example:_ Implementing a data structure where each operation has an associated credit, and operations with lower actual cost contribute excess credits to those with higher costs.

3. **Potential Method:**
   - _Definition:_ Associate a potential function with the data structure that represents the accumulated "potential" energy.
   - _Example:_ In binary counters, flipping a bit may have a cost of 2, but the potential function decreases by 1, resulting in amortized constant time.

**Example:**
Consider a dynamic array doubling its size when it reaches full capacity. Although occasional resizing is expensive (O(n)), when averaged over a sequence of insertions, the amortized cost per insertion remains O(1). This is because the infrequent resizing operation is offset by a series of cheaper insertions into the larger array.

Amortized analysis helps provide a more accurate and meaningful understanding of the overall efficiency of algorithms over time.

---

# Important Points

1. **Asymtotic Notations**

```
Big O : worst case upper bound
Omega: best case Lower bound
Theta: both
little o : upper bound not tight
little omega: lower bound not tight
```

2. **Time Complexity for Different Sorting Algorithms**

```
Bubble Sort, Selection Sort, Insertion Sort:
Time Complexity: O(n^2)

Merge Sort, Heap Sort:
Time Complexity: O(n log n)

QuickSort:
Time Complexity: O(n^2) in the worst case, O(n log n) on average.

Counting Sort:
Time Complexity: O(n + k), where k is the range of input.

Radix Sort:
Time Complexity: O(nk), where k is the number of digits in the input numbers.
```

3. **Analysis of Algorithms**

```
1. **Time Complexity Analysis:** Checks how fast an algorithm gets slower as the amount of work it has to do increases.

2. **Space Complexity Analysis:** Looks at how much computer memory an algorithm needs as the amount of work it does increases.

3. **Best, Worst, and Average Case Analysis:** Explores how well an algorithm performs in the best, worst, and usual situations it might face.

4. **Amortized Analysis:** Figures out the average time an algorithm takes over a series of actions, giving a more realistic picture of its overall speed.

5. **Empirical Analysis:** Runs real-world tests to see how well an algorithm performs with actual data.

6. **Comparative Analysis:** Puts different algorithms side by side to see which one works better for a specific job.

7. **Algorithmic Paradigms:** Refers to the big strategies or ways of thinking that guide how we design and understand algorithms to solve problems.
```

4. **Hashing**

```
## popular hash Function

1. Divide Method [ h(k) = k % m ]
2. Folding Method
3. Mid Square Method

## COLLISION

If two keys map on the same hash table index then we have a collision.
Two approaches are used to resolve collisions.

1. Open Hashing
   - Separate Chaining
2. Close hashing (Open Addressing)
   - Linear Probing [H <sub>i</sub> (x) = H(x)% m + i]
   - Quadratic Probing [H <sub>i</sub> (x) = H(x)% m + i^2]
   - Double hashing [H' = h + i*h],[[h(k) = k % m ], [h = m - (k % m)]]
```
