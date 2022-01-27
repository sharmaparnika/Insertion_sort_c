# Insertion Sort C

Insertion sort is a simple sorting algorithm that builds the final sorted array (or list) one item at a time. It is much less efficient on large lists than more advanced algorithms such as quicksort, heapsort, or merge sort.

However, insertion sort provides several advantages:

1. Simple implementation
2. Efficient for (quite) small data sets, much like other quadratic sorting algorithms
3. More efficient in practice than most other simple quadratic (i.e., O(n2)) algorithms such as selection sort or bubble sort
4. Adaptive, i.e., efficient for data sets that are already substantially sorted: the time complexity is O(kn) when each element in the input is no more than k places away from its sorted position
5. Stable; i.e., does not change the relative order of elements with equal keys
6. In-place; i.e., only requires a constant amount O(1) of additional memory space
7. Online; i.e., can sort a list as it receives it.

## Logic

The logic used to sort the elements by using the insertion sort technique is as follows −

    for(i = 1; i <= n - 1; i++){
      for(j = i; j > 0 && a[j - 1] > a[j]; j--){
        t = a[j];
        a[j] = a[j - 1];
        a[j - 1] = t;
         }
     }
     
 
 
## Algorithm

The simple steps of achieving the insertion sort are listed as follows -

**Step 1** - If the element is the first element, assume that it is already sorted. Return 1.

**Step2** - Pick the next element, and store it separately in a key.

**Step3** - Now, compare the key with all elements in the sorted array.

**Step 4** - If the element in the sorted array is smaller than the current element, then move to the next element. Else, shift greater elements in the array towards the right.

**Step 5** - Insert the value.

**Step 6** - Repeat until the array is sorted.


## Insertion Sort Complexity


Now, let's see the time complexity of insertion sort in best case, average case, and in worst case. We will also see the space complexity of insertion sort.

### 1. Time Complexity
Case	Time Complexity
Best Case - O(n)
Average Case - O(n2)
Worst Case - O(n2)


*   **Best Case Complexity** - It occurs when there is no sorting required, i.e. the array is already sorted. The best-case time complexity of insertion sort is O(n).
*   **Average Case Complexity** - It occurs when the array elements are in jumbled order that is not properly ascending and not properly descending. The average case time complexity of insertion sort is O(n2).
*   **Worst Case Complexity** - It occurs when the array elements are required to be sorted in reverse order. That means suppose you have to sort the array elements in ascending order, but its elements are in descending order. The worst-case time complexity of insertion sort is O(n2).


### 2. Space Complexity

**Space Complexity** - O(1)

**Stable** - YES

Please Note:- The space complexity of insertion sort is O(1). It is because, in insertion sort, an extra variable is required for swapping.


## **OUTPUT:-**

![image](https://user-images.githubusercontent.com/73773202/151296465-cb8f4c00-9cb6-4ebd-93c3-94bb8eb0d011.png)

---
