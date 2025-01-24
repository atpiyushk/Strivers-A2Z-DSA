# Insertion Sort

## Code

```java

class Solution {
    // Function to sort the array using insertion sort algorithm.
    public void insertionSort(int arr[]) {
        int i, j, temp;
        for(i=0;i<arr.length;i++){
            j=i;
            while(j>0 && arr[j-1]>arr[j]){
                temp=arr[j-1];
                arr[j-1]=arr[j];
                arr[j]=temp;
                j--;
            }
        }
    }
}