# Hands-on--8
This is a repository of "UTA ID:1002201193". With student email "mxo1193@mavs.uta.edu".



Task 1: ith quicksort working 

Random Array Generation:
The code generates a random array of 10 integers between 0 and 100 using the rand.randint function from the random module.

Selection of ith Order Statistic:
It randomly selects a value for i (between 1 and the length of the array) to search for the ith order statistic.
For example, if i is 5, the code aims to find the 5th smallest element in the array.

Quicksort and Partitioning:
The code utilizes a partitioning function to rearrange elements in the array such that elements less than the chosen pivot are placed to the left, and elements greater than the pivot are placed to the right.
The quickselect function recursively partitions the array based on the pivot until the ith order statistic is found.

Validation:
After finding the ith order statistic using quickselect, the code performs a validation step to ensure correctness.
It creates a copy of the original array and sorts it using the sort() method.
It then compares the ith element of the sorted array with the ith order statistic obtained from quickselect.
If both values match, it indicates that the ith order statistic was correctly identified.

Output:
The code prints the original array, the chosen value of i, the ith order statistic obtained from quickselect, and the ith order statistic obtained from the sorted array during validation.

Result:
Finally, the code displays whether the ith order statistic obtained from quickselect matches the one obtained from the sorted array during validation.
