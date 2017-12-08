# Unique Binary Search Trees 


## Prompt 
Given n, how many structurally unique BSTs (binary search trees) that store values 1...n?



### Example 
Given n = 3, there are a total of 5 unique BSTs.   

Input: 3   
Output: 5 

```
   1           3      2       1             3 
    \         /      / \       \           / 
     3       2      1   3       2         1 
    /       /                    \         \ 
   2       1                      3         2 

```


Given n = 4, there are a total of 10 unique BSTs.  
  
Input: 4   
Output: 10 

```
 1               1             1       
  \               \             \ 
   2               3             4 
    \             / \           / 
     3           2   4         3 
      \                       / 
       4                     2 
       
      
    2          2  
   / \       /   \ 
  1   3     1     4 
       \         /   
       4        3
       
       
     3          3       
   /  \       /  \       
  2    4     1    4 
 /           \          
1             2
               
       4       4        4         
      /       /       / 
     3       2       1 
    /       /         \
   2       1           2 
  /         \           \ 
 1           3           3 
    
 ```


### Resources
[Leetcode Discussion](https://leetcode.com/problems/unique-binary-search-trees/discuss/)  
[Dynamic Programming Concepts](http://programming.guide/dynamic-programming-vs-memoization-vs-tabulation.html)   
[Catalan numbers](http://www.geeksforgeeks.org/program-nth-catalan-number/)

### Hints 
If we iterated through every possible node in the Binary Search Tree and assigned each one to be a root, how would we
know the number of structurally different binary search trees of the left and the right subtrees? 

Let's say we have an array where each index represents the number of unique nodes, and the value 
associated with each index represents the number of structurally different binary search trees
generated with each index. If we want to find out the number of structurally different BSTs 
generated with two unique nodes, how can we use the previous cases of generating BSTs 
with 1 unique node and 0 unique nodes to reach our solution? 