# Table of Contents

- [I. Data Structures and Libraries](#I-Data-Structures-and-Libraries)
    - [1. Linear DS with Built-in Libraries](#1-Linear-DS-with-Built-in-Libraries)
        - [1.1 Array](#11-Array)
            - [1.1.1 Static (Fixed-size) Array](#111-Static-Fixed-size-Array)
            - [1.1.2 Dynamic (Resizeable) Array](#112-Dynamic-Resizeable-Array)
            - [1.1.3 Array of Booleans](#113-Array-of-Booleans)
            - [1.1.4 Sorting & Searching](#111-Sorting-&-Searching)

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
