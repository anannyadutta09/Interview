# Stack Algo

## 1. Duplicate Brackets
- Pepcoding : https://www.youtube.com/watch?v=aMPXhEdpXFA&list=PL-Jc9J83PIiEyUGT3S8zPdTMYojwZPLUM&index=3 

### Problem 
  - (a+b) *((C+D)) --> Contains Duplicate Bracket 
  - (a+b) *(C+D) --> Does not contains Duplicate Bracket 

### Algo
  - push every element on stack 
  - if we find a cosing bracket `)`; pop all elements untill the next `(`
  - if there is no middle element between `(` and `)` then it must be a duplicate bracket 

## 2. Next Greater Element on Right 
- Pepcoding : https://www.youtube.com/watch?v=rSf9vPtKcmI&list=PL-Jc9J83PIiEyUGT3S8zPdTMYojwZPLUM&index=7

### Explanation
 - or a given array find teh next greater element element on right 
 - compelxity `O(n)`
 -  ![image](https://user-images.githubusercontent.com/68387132/172214628-689eb0ce-df9a-4c46-8084-f3cfecd602a0.png)
### Algo
 - we want to finf the next Greater Element on the Right 
 - if we start with the last element ( `arr[n-1]` ) , there is no `next` element , and clearly there is **no** `next greater element`
 - As per Dynamic Programming rule , on the right hand side we have smaller problem ; we start from the last element of the array
 - Direction :
   - right to left ; end to start   

 - we put the last element of the array and put it in stack 
 - we make the next greater element on right for teh last element = -1
 - from the second last element of teh array till teh first element of teh array , we perform the following 
    -  we continue to pop elelemts from stack which are smaller than the current array element 
    -  the element on top of the stack is the next greater element for teh current array element 
    -  if no elelemnt on stack is present, then there is no greater element on right 
    -  now we put the current element on the stack    

### Code
 - ![image](https://user-images.githubusercontent.com/68387132/172216064-45cf3cab-4d3c-4d0d-b6e8-5615d12df9d4.png)
### Complexity 
 - `O(n)`
- the inner while loop runs fewer time 
- each element is pushed and popped only once 
- compleity is `O(n) + O(n)`
