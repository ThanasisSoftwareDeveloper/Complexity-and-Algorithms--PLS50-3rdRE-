Topic 2: Classification algorithms
------------------------------------------------
(otherwise: sorting algorithms)
For each of the following algorithms, demonstrate sorting the elements of the following table of 10 different numbers, step by step. The positions in the table are numbered from 1 to 10.
8 3 9 1 0 4 2 7 6 5

Consider as a step the cases where a swap of the elements of two positions of the table is performed. The two elements that swap positions will be indicated by a coloured highlight.
The algorithms are described in Appendix A at the end of the Assignment.
In particular, the algorithms whose operation you are asked to demonstrate, with individual instructions for each of them, are as follows:
α) Classification by input
In this algorithm you will report the value of variable j each time two items are permuted (you do not need to report the value of variable i). As a hint you are given the first permutation:
j=2
3 8 9 1 0 4 2 7 6 5

b) Sort by selection
In this algorithm, you will report the value of variable i each time two items are permuted (you do not need to report the value of variable j). As a hint, you are given the first permutation:
i=1
0 3 9 1 8 4 2 7 6 5 

(c) Bubble classification
In this algorithm you will report the value of variable i each time two elements are permuted (you do not need to report the value of variable j). As a hint you are given the first permutation:
i=1
3 8 9 1 0 4 2 7 6 5 
d) Quick sorting
In this algorithm you will report the values of the variables left, right and pivot for each recursive call to quicksort (including the initial one), followed by all the permutations of the table values that were made (you do not need to report the values of i and j for each permutation, and the last permutation is understood to result from the line in the 1.c.i command unless j has been made equal to left). As a hint you are given the first permutation:
left=1, right=10, pivot=8
8 3 5 1 0 4 2 7 6 9 

(e) Classification by merge
This algorithm assumes the existence of an auxiliary table B of (at least) the same size as the table A to be sorted. The auxiliary table is used to merge the sub-tables of the original table before each merged sub-table is copied into the corresponding positions of the original table.
Show all calls to MergeSort and Merge, in the order in which they occur and with their definitions, and the incremental creation of table B for each call to Merge (the cell B[temp] that takes a value in row 2.a.i or row 2.a.ii or row 3.a.i or row 3.a.ii should be shown colored). As a hint, you are given the first calls to the algorithm, up to the first execution of the if structure in line 2.a of the Merge pseudocode:
MergeSort(1,10)
MergeSort(1,5)
MergeSort(1,3)
MergeSort(1,2)
MergeSort(1,1)
MergeSort(2,2)
Merge(1,1,2)
3 ....

Topic 3: Design of a search algorithm: finding the middle element of a table
----------------------------------------------------------------------------------
Propose an algorithm that finds the median number in an unsorted matrix A with n different integer numbers (positive and negative), where n is an odd number (so the median number is unique), without being allowed to change the position of the numbers in A (e.g., you are not allowed to sort A) and without accessing additional memory beyond what you need for the local variables of the algorithm (e.g, you cannot commit memory equal to the size of your table to perform a sort, but you can use as much memory as you want, the size of which must be fixed and independent of the size of table A). Try to optimize it as much as possible. 
What are the complexities O and Ω of your algorithm?
