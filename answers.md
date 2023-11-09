# CMPS 2200 Recitation 06
## Answers

**Name:**___Amara Midouhas______________________
**Name:**_________________________


Place all written answers from `recitation-07.md` here for easier grading.



- **2)** F(n) = F(n-1) + F(n-2) + c
if n =2 then, F(2)= F(2-1) + F(2-2) +c = F(2) = 1+1+c = 2+c
if n = 3, then F(3) = F(3-1) + F(3-2) +c = F(3)= 2 + 1+c = 3+c
The Fibonacci Sequence start with 0 and 1 so this is our base case
and if n = 0, then W(0) = F(0+1)+c-1 = W(0)= F(1) + c-1
and if n =1, then W(1) = F(1+1)+c-1 = W(1) = F(2)+c-1
Therefore, W(n) will be higher then F(n+1) because of the constant amount of work and 1 is because of the intial base case so W(n)=F(n+1)+c-1

- **3)** F(n) = F(n-1) + F(n-2) + c. Since we know the base cases are 0 and 1 and we have two subproblems of size n-1 and n-2.
To compute F(n), we use n-1 and n-1 (like seen above)
Then we add on the constant time which is c 
Then since we want to look at the maximum time spent on either F(n-1) or F(n-2), we subtract -1 to ensure there isnt overlap of time for both F(n-1) and F(n-2)
Therefore, we get S(n)= F(n) + d -1


- **4)** The count is used to keep track of how many times each value is computed when computing the Fibonacci numbers. The count goes up by 1 everytime a number is calculated in the recursive. Therefore, it ensures there wont be redundant operations and hence shows how memoization improves the efficiency of calculating Fibonacci numbers. The pattern shows when you move away from the base (0 and 1) where the Fibonacci numbers are low, the higher the count gets.


- **6)** The maximum number of times it will be called is n+1. The work and span are both O(n) because the work it the sum of calls made for each number from 0 to n and the span is O(n) because in the worst case, it will perform n+1 calls so its O(n).

- **8)** The maximum number of time it will be read is 2. The work is O(n) because it is computing and storing values between 0 and n. The span is O(n) because in the worst case the each of the numbers are computed sequentially.
