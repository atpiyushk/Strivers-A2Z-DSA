# Selection Sort

## Code

```java

class Solution {
    // Function to sort the array using selection sort algorithm.
    void selectionSort(int[] arr) {
        int i,j,min,temp;
        for(i=0;i<arr.length-1;i++){
            min=i;
            for(j=i+1;j<arr.length;j++){
                if(arr[j]<arr[min]){
                    min=j;
                }
            }
            temp=arr[i];
            arr[i]=arr[min];
            arr[min]=temp;
        }
    }
}