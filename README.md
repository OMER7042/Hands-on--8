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


Task 2: QUEUE

Initialization:
The Queue class is initialized with a specified length for the queue.
It creates an array (data) to store the elements, and sets two pointers (head_index and tail_index) to keep track of the front and rear of the queue.
The length of the queue is stored in the length attribute.

Queue Operations:
enqueue_element: Adds an element to the rear of the queue. It checks if the queue is full before adding.
dequeue_element: Removes and returns the element from the front of the queue. It checks if the queue is empty before dequeuing.
get_head_element and get_tail_element: Returns the element at the front and rear of the queue, respectively.
get_element_at_index_behind_head: Returns the element at a specified index behind the head of the queue.
get_number_of_elements: Returns the number of elements currently in the queue.

Printing Queue Details:
print_queue_details: Displays various details about the queue, including the elements in the queue, whether it's empty or full, the number of items, and the head and tail elements.

Main Function:
The main part of the code demonstrates the functionality of the queue.
It initializes a queue with a length of 10 and prints its initial details.
It enqueues 3 random numbers into the queue, prints the details, then attempts to enqueue 7 more (resulting in a queue overflow).
It prints the details again, showing the queue as full.
It dequeues 5 items from the queue, updates the details accordingly, and prints the number of items remaining in the queue.
