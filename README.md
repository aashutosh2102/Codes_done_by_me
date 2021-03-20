# Codes_done_by_me
Here, I will provide the solutions of all those question which I will be following on different competitive websites.(HackerRank, Codechef, GFG)

### Hacker Rank

Question 1:
Array-Ds ::An array is a type of data structure that stores elements of the same type in a contiguous block of memory. In an array,A, of size N, each memory location has some unique index,i (where 0<=i<N), that can be referenced as A[i] or Ai .
Reverse an array of integers.

Note: If you've already solved our C++ domain's Arrays Introduction challenge, you may want to skip this.

Example
A = [1,2,3]
Return [3,2,1].

###### Solution:::::::>>>                   USING C                <<<<<<<<<<<<<:::::::

```
   #include<stdio.h>
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
   }
```


Question 2:
2D Array-DS :: Given a 6*6 2D Array,arr: An hourglass in A is a subset of values with indices falling in this pattern in arr's graphical representation:
There are 16 hourglasses in arr. An hourglass sum is the sum of an hourglass' values. Calculate the hourglass sum for every hourglass in arr, then print the maximum hourglass sum. The array will always be 6*6.
Note: If you have already solved the Java domain's Java 2D Array challenge, you may wish to skip this challenge.

Example

arr=

-9 -9 -9  1 1 1 
 0 -9  0  4 3 2
-9 -9 -9  1 2 3
 0  0  8  6 6 0
 0  0  0 -2 0 0
 0  0  1  2 4 0
 
 The 16 hourglass sums are:
 
 -63, -34, -9, 12, 
-10,   0, 28, 23, 
-27, -11, -2, 10, 
  9,  17, 25, 18
  
The highest hourglass sum is 28 from the hourglass beginning at row 1, column 2:
  
0 4 3
  1
8 6 6

###### Solution:::::::>>>                   USING C                <<<<<<<<<<<<<:::::::

```
   #include<stdio.h>
   int main()
   {
     int i,j,n,a[6][6],b[4][4];
     for(i=0;i<6;i++) //Providing the 2D array of 6*6 input
    {
        for(j=0;j<6;j++)
        {
            scanf("%d",&a[i][j]);
        }
    }
    for(i=0;i<6;i++)
    {
        for(j=0;j<6;j++)
        {// addition of values accotding to the format of watch-glass
            b[i][j]=a[i][j]+a[i][j+1]+a[i][j+2]+a[i+1][j+1]+a[i+2][j]+a[i+2][j+1]+a[i+2][j+2];
        }
    }
    int max=b[0][0];// setting a max value
    for(i=0;i<4;i++)
    {
        for(j=0;j<4;j++)
        {
            if(b[i][j]>max)// any of the element is max
            {
                max=b[i][j];
            }    
        }
    }
    printf("%d",max);
  }
```
