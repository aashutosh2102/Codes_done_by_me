# Codes_done_by_me
Here, I will provide the solutions of all those question which I will be following on different competitive websites.(HackerRank, Codechef, GFG)

Hacker Rank

Question 1:
Array-Ds ::An array is a type of data structure that stores elements of the same type in a contiguous block of memory. In an array,A, of size N, each memory location has some unique index,i (where 0<=i<N), that can be referenced as A[i] or Ai .
Reverse an array of integers.

Note: If you've already solved our C++ domain's Arrays Introduction challenge, you may want to skip this.

Example
A = [1,2,3]
Return [3,2,1].

###### Solution:::::::>>>                   USING C                <<<<<<<<<<<<<:::::::

"#include<stdio.h>
int main()
{
    int i,n,a[1000];
    scanf("%d",&n);
    for(i=n-1;i>=0;i--) // Taking the array in reverse order
    {
        scanf("%d",&a[i]);
    }
    for(i=0;i<n;i++) // printing it in the same order as taken in scanf
    {
        printf("%d ",a[i]);   //here, in "%d " space is provided as according to the question
    }                      
    return 0;
}"
