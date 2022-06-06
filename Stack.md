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
 - compelxity O(n)
 -  ![image](https://user-images.githubusercontent.com/68387132/172214628-689eb0ce-df9a-4c46-8084-f3cfecd602a0.png)


