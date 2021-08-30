## DSA 450 Questions
- Reverse the array
```
string reverseWord(string str){
    int i,n=str.length();
    for(i=n-1;i>=0;i--)
    {
        cout<<str[i];
    }
}
```

- Find the "Kth" max and min element of an array 
```
int kthSmallest(int arr[], int l, int r, int k) {
    sort(arr, arr + r+1); 
    return arr[k-1];
}
```

- Sort an array of 0s, 1s and 2s (Cpp and Python)
- - Cpp
```
class Solution
{
    public:
    void sort012(int a[], int n)
    {
        return sort(a,a+n);
    }
    
};
```
- - Python
```
class Solution:
    def sort012(self,arr,n):
        return arr.sort()
```

- Find the Union and Intersection of the two sorted arrays.
```
class Solution:
    def doUnion(self,a,n,b,m):
        a=set(a)
        b=set(b)
        c=a.union(b)
        c=list(c)
        return len(c)
```

- Write a program to cyclically rotate an array by one.
```
def rotate( arr, n):
    temp = arr[n-1]
    i = n-1
    while i>=1:
        arr[i] = arr[i-1]
        i-=1
    arr[0] = temp
    return arr
```

- find Largest sum contiguous Subarray [V. IMP]
```
class Solution:
    def maxSubArraySum(self,a,size):
        cursum,maxsum=0,max(a)
        for i in range(size):
            cursum=cursum+a[i]
            if(cursum<0):
                cursum=0;
                continue;
            if(maxsum<cursum):
                maxsum=cursum
        return maxsum
```
