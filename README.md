# Optimal-Binary-Search-Tree
A little more Dynamic Programming. Suppose you have a large number of search terms, and you happen to work at Google. You can arrange the search terms in a binary tree (with the terms at the leaves). The terms have to stay in alphabetical order, but how you arrange the tree will impact how many edges you have to traverse down to find what you're looking for.
As a simple example, suppose you have three terms, A, B, and C. You search for A 10 times, B 3 times, and C 1 time. You could arrange them with A on the left branch, and B and C as a pair on the right branch. In terms of the number of edges you have to traverse to handle all the searches, there are 10 traversals of a single edge to get to A, and then 4 traversals of the edge to get to the B and C pair, and then 3 down the edge to B, and 1 down the edge to C. The total number of edge traversals for this tree is 10 + 4 + 3 + 1, or 18.
An alternate way to build the tree would be to place A and B onto a branch, and then have C on the right hand side of the tree. The total number of traversals this way is 13 to get down to the point where A and B are paired, 10 more to reach A, 3 more to get to B, and then a single edge traveral to get to C. The total this way is 13 + 10 + 3 + 1, or 27. The first tree is better, right?
For this program, the input will consist of the number of search terms (up to 1000), and then the total number of times each term is searched for. Your program should print out the total number of traversals required, for an optimal binary search tree.
Read from standard input, and print out the single number (total traversals) to standard output. Check the textbook for more details on the problem....
Here are a few input files to test with:
•	bst1.txt (correct answer 225)
•	bst2.txt (correct answer 997)
•	bst3.txt (correct answer 789)
•	bst4.txt (correct answer 5968)
