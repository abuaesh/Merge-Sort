# Merge-Sort
This project is an implementation of the well known merge sort algorithm, but with the possibility of parallelizing it using Cilk. In this repository, you will find the following files:

**1. mergesort_seq.cilk -** This the sequantial implementation of the algorithm with no parallelization at all. This means that only one processor will run the code.

**2. mergesort_half.cilk -** This version of the program has the sort function parallelized, but not the merge function. Hence, it is half-parallel execution, since there is a function(merge) that is parallelizable, but has not been set to execute in parallel. 

**3. mergesort_full.cilk -** This is the fully parallel implementation of the program, with both the merge and the sort functions set to execute in parallel.

**4. results.htm -** This file shows the statistics collected after running each of the above files on various array sizes(n ranges from 100 elements to 1M elements), and with various number of processors working on the program in parallel(p ranges from 1 core to 4 cores)


