#### Sorting Algorithms

* sorting is the most time consuming thing for a computer to do
   * avoiding sorting is a good thing
   * if possible keep data in sorted order rather than sorting later

> Ordering Items

> Sample Data for Sort
- For all sorts we will use an integer array containing 
   - 10, 7, 11, 4, 8, 3, 9 , 6, 1, 2

  
![Data for sorting algs](https://github.com/RamziCarter/DataStructures1/blob/eef516fff8292c9efb24a77d6bceb79e7b532dad/Sample%20Data.png)

---

Selection Sort
```
10, 7 , 11, 4, 8, 3, 9, 6, 1, 2

1, 7 , 11, 4, 8, 3, 9, 6, 10, 2

1, 2 , 11, 4, 8, 3, 9, 6, 10, 7

1, 2 , 3, 4, 8, 11, 9, 6, 10, 7

1, 2 , 3, 4, 6, 11, 9, 8, 10, 7

1, 2 , 3, 4, 6, 7, 9, 8, 10, 11

1, 2 , 3, 4, 6, 7, 8, 9, 10, 11

Selection sort is O(n^2) for best, worst and general cases. 

```

Insertion Sort
- break array into two pieces (left and right)
```
- 10 | 7 , 11, 4, 8, 3, 9, 6, 1, 2

- 7 10 | , 11, 4, 8, 3, 9, 6, 1, 2

- 7 10 11 | 4, 8, 3, 9, 6, 1, 2

- 4 7 10 11 | 8, 3, 9, 6, 1, 2

- 4 7 8 10 11| 3, 9, 6, 1, 2

- 3 4 7 8 10 11| 9, 6, 1, 2

- 3 4 7 8 9 10 11| 6, 1, 2

- 3 4 6 7 8 9 10 11| 1, 2

- 1 3 4 6 7 8 9 10 11| 2

- 1 2 3 4 6 7 8 9 10 11|

```

Shell Sort
- break the array into subarrays
- O(n^1.5) in the worst case and average case
  - O(n) in the best case 
```
10, 7, 11, 4, 8, 3, 9 , 6, 1, 2

```

Bubble Sort
```
10, 7, 11, 4, 8, 3, 9, 6, 1, 2
7, 10, 11, 4, 8, 3, 9, 6, 1, 2
7, 10, 4, 11, 8, 3, 9, 6, 1, 2
7, 10, 4, 8, 11, 3, 9, 6, 1, 2
7, 10, 4, 8, 3, 11, 9, 6, 1, 2
7, 10, 4, 8, 3, 9, 11, 6, 1, 2
7, 10, 4, 8, 3, 9, 6, 11, 1, 2
7, 10, 4, 8, 3, 9, 6, 1, 11, 2
7, 10, 4, 8, 3, 9, 6, 1, 2, 11
7, 4, 10, 8, 3, 9, 6, 1, 2, 11
7, 4, 8, 10, 3, 9, 6, 1, 2, 11
7, 4, 8, 3, 10, 9, 6, 1, 2, 11
7, 4, 8, 3, 9, 10, 6, 1, 2, 11
7, 4, 8, 3, 9, 6, 10, 1, 2, 11
7, 4, 8, 3, 9, 6, 10, 1, 2, 11
```


Can we do better than O(n^2)

MergeSort
- break the data in half
  - sort them
    - combine the halves
- this is recursive

O(n log n)

- the drawback to this sort is that it uses a ton of space

- The compareTO method
