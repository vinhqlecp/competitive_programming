# Table of Contents

- [I. Data Structures and Libraries](#I-Data-Structures-and-Libraries)
    - [1. Linear DS with Built-in Libraries](#1-Linear-DS-with-Built-in-Libraries)
        - [1.1 Array](#11-Array)
            - [1.1.1 Static (Fixed-size) Array](#111-Static-Fixed-size-Array)
            - [1.1.2 Dynamic (Resizeable) Array](#112-Dynamic-Resizeable-Array)
            - [1.1.3 Array of Booleans](#113-Array-of-Booleans)
            - [1.1.4 Sorting & Searching](#114-sorting--searching)

# I. Data Structures and Libraries
## 1. Linear DS with Built-in Libraries
### 1.1 Array
#### 1.1.1 Static (Fixed-size) Array
* This is the most commonly used data structure in programming contests. <br>
* Whenever there is a collection of homogenous sequential data to be stored and later accessed using their indices, the static array is the most natural data structure to use. <br>
* As the maximum input size is usually mentioned in the problem statement, the array size can be declared to be the maximum input size, with a small extra buffer (sentinel) for safety to avoid the unnecessary 'off by one' RTE. <br>
* Typically, 1D and 2D arrays are used in programming contests <br>
#### 1.1.2 Dynamic (Resizeable) Array
* This data structure is similar to the static array, except that it is designed to handle runtime resizing natively <br>
* It is better to use a vector in place of an array if the size of the sequence of items is unknown at compile-time. <br>
* Typical C++ STL vector operations used in competitive programming include push back(), at(), the [] operator, assign(), clear(), erase(), and iterators for traversing the contents of vectors. <br>

There are two operations commonly performed on arrays: **_Sorting_** and **_Searching_**. We will research about them later. <br>
#### 1.1.3 Array of Booleans
* If our array needs only to contain Boolean values (1/true and 0/false), we can use an alternative data structure other than a plain array—a C++ STL bitset (Java BitSet). <br>
* However if our array of Booleans is small (not more than 62 Booleans), it is beneficial to use bitmask data structure. <br>

#### 1.1.4 Sorting & Searching
It is appropriate to discuss two operations commonly performed on arrays: Sorting and Searching. <br>
There are many **_sorting_** algorithms <br>
* **_O(n^2) comparison-based sorting algorithms_**: Bubble/Selection/Insertion Sort... These algorithms are (awfully) slow and usually avoided in programming contests, though understanding them might help you solve a few specific problems, e.g., Insertion Sort actually runs in O(n) when the input array is almost sorted.
* **_O(nlogn) comparison-based sorting algorithms_**: Merge/Quick5/Heap Sort... These algorithms are the default choice in programming contests as an O(n log n) complexity is optimal for comparison-based sorting. Therefore, these sorting algorithms run in the ‘best possible’ time in most cases. we can simply use sort, stable sort, or partial sort in C++ STL algorithm for basic sorting tasks. We only need to specify the required comparison function (which can be a lambda expression) and these effecient sorting library routines will handle the rest. Following example source code give us how to use C++ STL sorting (suppose that we have a vector<int> A):

<pre><code>
// technique 1, create a custom comparison function
bool cmp(const int a, const int b) {
    return a > b;
}

// Using sort with compare function
sort(A.begin(), A.end(), cmp);
</code></pre>

<pre><code>
// technique 2, use an anonymous function (lambda expression)
sort(A.begin(), A.end(), [](const int a, const int b){ return a > b; }));
</code></pre>
    
<pre><code>
// technique 3, use reverse iterator
sort(A.rbegin(), A.rend()); // [1 2 3 4 5] -> [5 4 3 2 1]
</code></pre>

* **_O(n) Special purpose sorting algorithms_**: Counting/Radix/Bucket Sort,... Although rarely used, these special purpose algorithms are good to know as they can reduce the required sorting time if the data has certain special characteristics
    
There are generally three common methods to **_search_** for an item in an array: <br>

* **_O(n) Linear Search_**: Consider every item from index 0 to index n-1 (try to avoid this).
* **_O(log n) Binary Search_**: Use lower bound, upper bound, or binary search in C++ STL algorithm. If the input array is unsorted, it is necessary to sort the array at least once (using one of the O(n log n) sorting algorithms above) before executing one/many Binary Search(es).

## 2. Non-Linear DS with Built-in Libraries
## 3. DS with Our Own Libraries

# II. Problem Solving Paradigms
## 1. Complete Search
## 2. Divide and Conquer
## 3. Greedy
## 4. Dynamic Programming

# III. Graph
## 1. Graph Traversal
## 2. Minimum Spanning Tree (MST)
## 3. Single-Source Shortest Paths (SSSP)
## 4. All-Pairs Shortest Paths (APSP)
## 5. Special Graphs

# IV. Mathematics
## 1. Ad Hoc Mathematical Problems
## 2. Number Theory
## 3. Combinatorics
## 4. Probability Theory
## 5. Cycle-Finding
## 6. Matrix Power

# V. String Processing

# VI. (Computational) Geometry

# VII. More Advanced Topics

# VIII. Rare Topics
