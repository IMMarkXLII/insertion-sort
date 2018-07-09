# insertion-sort

```
  static void insertionSort(int[] arr) {
		for(int i = 0; i<arr.length ; i++) {
			// for each iteraion of i, we bring the element at ith position to its correct position in the sorted order
			// for each i, array to the left of i is sorted and to its right, unsorted
			int j=i;
			int val = arr[i];
			for(; j>0 && arr[j-1] > val; j--) {
				arr[j] = arr[j-1];
			}
			if(j!=i) {
				arr[j] = val;
			}
		}
		
	}
```
