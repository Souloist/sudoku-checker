# sudoku_checker

A valid sudoku board will only contain distinct entries of the numbers 1 - 9 but any duplicates of 0s. 0s will refer to an entry which is not yet filled. 

## Valid Example
```
>>> valid = [[1,0,0,0,0,7,0,9,0],             
...         [0,3,0,0,2,0,0,0,8],             
...         [0,0,9,6,0,0,5,0,0],             
...         [0,0,5,3,0,0,9,0,0],             
...         [0,1,0,0,8,0,0,0,2],             
...         [6,0,0,0,0,4,0,0,0],             
...         [3,0,0,0,5,0,0,1,0],             
...         [0,4,0,0,0,0,0,0,7],             
...         [0,0,7,0,0,0,3,0,0]]             
>>> from sudoku_checker import check_sudoku_board   
>>> check_sudoku_board(hard)                 
True                                         
```

## Invalid Example
```
>>> invald = [[1,0,0,0,0,7,0,9,0],     
...          [0,3,0,0,2,0,0,0,8],     
...          [0,0,9,6,0,0,5,0,0],     
...          [0,0,5,3,0,0,9,0,0],     
...          [0,1,0,0,8,0,0,0,2],     
...          [6,0,0,0,0,4,0,0,0],     
...          [3,0,0,0,0,0,0,1,0],     
...          [0,4,0,0,0,0,0,0,7],     
...          [0,4,0,0,0,0,0,0,7],     
... ]    
>>> from sudoku_checker import check_sudoku_board   
>>> check_sudoku_board(hard)         
False                                
```

This board is invalid since the bottom-left subgroup has a duplicate 4
```
3 0 0 
0 4 0
0 4 0
```
