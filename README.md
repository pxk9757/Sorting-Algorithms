# Argue selection sort correctness.
 Selection sort is a simple sorting algorithm that works by repeatedly finding the minimum element in the unsorted portion of the array and swapping it with the first element of the unsorted portion. This process is repeated until the entire array is sorted. To argue the correctness of selection sort, we can use loop invariants. A loop invariant is a condition that is true before and after each iteration of a loop. We can use loop invariants to prove that a sorting algorithm is correct by showing that the loop invariant holds before the first iteration of the loop, that the loop invariant is maintained by each iteration of the loop, and that the loop invariant implies that the array is sorted when the loop terminates. For selection sort, we can use the following loop invariant: At the start of each iteration of the outer loop, the subarray arr[0..i-1] is sorted and contains the i smallest elements of the original array.

 We can prove that this loop invariant holds as follows:
Before the first iteration of the outer loop, the subarray arr[0..0] contains only one element, which is trivially sorted.
Each iteration of the inner loop finds the smallest element in the unsorted portion of the array and swaps it with the first element of the unsorted portion. This ensures that the subarray arr[0..i-1] is sorted and contains the i smallest elements of the original array.
When the outer loop terminates, the entire array is sorted because the subarray arr[0..n-1] contains all the elements of the original array and is sorted.
Therefore, we can conclude that selection sort is correct because it maintains the loop invariant that the subarray arr[0..i-1] is sorted and contains the i smallest elements of the original array, and this loop invariant implies that the array is sorted when the loop terminates.


# SortBenchmarker
A program that benchmarks common sorting algorithms and displays their overall performance


# Steps to run benchmarks

1. Clone the repository (or download the code)
2. Change directory to the cloned directory
3. Make sure you have python and pip installed (preferably in a virtual environment)
4. run `pip install -r requirements.txt`

## You're All Set
### Run `python main.py` to get started



## Author
### Priyanka Kondamadugu