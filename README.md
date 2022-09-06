# assingment1

Given 3 arrays stack1[ ], stack2[ ] and stack3[ ] representing stacks and the starting index of these arrays are treated as their top. We need to fnd out the  common maximum sum possible in all the three stacks i.e. the sum of elements of stack1, stack2 and stack3 are equal. Removal of the top is allowed in each array to find the common maximum sum.

We can find all possible sums by first finding the initial sum of the three stacks and popping elements one by one and then storing the sums in an array.We do the same for all three stacks.hence we check if any number is found in all three arrays. If yes, we return the maximum number.Else we will always have an answer as 0 as we can just empty all three stacks and their sum will be the same.

Let us take an example"
Stack1:               Stack2:                  Stack3:
  3                         4                       1
  2                         3                       1
  1                         2                       4
  1                                                 1
  1
  SUM1= 8                    SUM2=9                 SUM3=7
  
  *By observing the values of all the three sums , we can say that sum2 in the greatest of all.Hence, we will pop the top of the stack2 which is "4"
  Stack 2 :
  3
  2
  
  Hence, our sum2 now becomes 3+2=5
  
  We will compare again among sum1,sum2,sum3
  Now, sum 1 is greater than other two.
  hence, top of stack1 will be removed i.e. 3
  
  Hence, stack1 becomes 
  2
  1
  1
  1
  sum1=5
  
Again comparing three sums
Stack3 is greater. again applying the same method
Stack 3:
1
4
1
Sum3:6
this is again greater than other two
Removing the top again

stack3:
4
1

sum3=5

**Therefore, common maximum sum is 5**
Complexity Analysis
Time Complexity: O(n1+n2+n3) where n1, n2, and n3 are the number of elements in arrays stack1, stack2, and stack3 respectively.

*************************************************************************************************
