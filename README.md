[1]

1
An array of 6 integers is being sorted in non-decreasing order using Quicksort.
Suppose the algorithm has just finished the first pass of partitioning and pivot swapping thus changing the content of the original array into the following array:
[13, 11, 9, 2, 10, 15]
From the resulting array above, determine how many integers could have been the pivot?
Note: elements == pivot are partitioned to the right.

Enter a number =(1)

2
How many comparison(s) is/are required to sort an array of n=6 integers: [13, 14, 15, 17, 18, 16] using this version of Selection Sort?
for (i = 0; i < n-1; ++i) {
  cur_min = i;
  for (j = i+1; j < n; ++j)
    if (A[j] < A[cur_min]) // each execution of this if-statement is counted as one comparison
      cur_min = j;
  swap(A[i], A[cur_min]);
}

Enter a number=(15)

3
Rearrange the integers to produce the content of the array A=[12, 23, 11, 25, 13] with n integers after 2 passes of this version of Selection Sort.
for (i = 0; i < 2; ++i) { // 2 passes
  cur_min = i;
  for (j = i+1; j < n; ++j)
    if (A[j] < A[cur_min])
      cur_min = j;
  swap(A[i], A[cur_min]);
}

[11,12,23,25,13]

4
How many comparison(s) is/are required to sort an array of n=8 integers: [16, 15, 14, 19, 20, 17, 13, 18] using this version of Bubble Sort?
for (j = 0; j < n-1; ++j)
  for (i = 0; i < n-j-1; ++i)
    if (A[i] > A[i+1])
      swap(A[i], A[i+1]);

28

5
How many swap(s) is/are required to sort an array of n=3 integers: [5, 21, 16] using this version of Bubble Sort?
for (j = 0; j < n-1; ++j)
  for (i = 0; i < n-j-1; ++i)
    if (A[i] > A[i+1])
      swap(A[i], A[i+1]);

Enter number =(1)

6
Rearrange the integers to produce the content of the array A=[26, 8, 19, 29, 16] with n integers after 2 passes of this version of Bubble Sort.
for (j = 0; j < 2; ++j) // 2 passes
  for (i = 0; i < n-j-1; ++i)
    if (A[i] > A[i+1])
      swap(A[i], A[i+1]);

    [8,16,26,19,29]

7
Rearrange the integers to produce the content of the array A=[16, 12, 13, 8, 1, 4] with n integers after 3 passes of this version of Insertion Sort.
for (i = 1; i <= 3; ++i) { // 3 passes
  e = A[i]; j = i;
  while (j > 0) {
    if (A[j-1] > e)
      A[j] = A[j-1];
    else
      break;
    j--;
  }
  A[j] = e;
}

[1,4,8,12,13,16]
