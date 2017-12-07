# Unique Binary Search Trees 


## Prompt 
Given n, how many structurally unique BST's (binary search trees) that store values 1...n?



### Example 
Given n = 3, there are a total of 5 unique BSTs. 

```
   1           3      2       1             3 
    \         /      / \       \           / 
     3       2      1   3       2         1 
    /       /                    \         \ 
   2       1                      3         2 

```

Given n = 4, there are a total of 10 unique BSTs

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