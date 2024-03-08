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

TASK 2 : STACK

1. Initialization: We start by creating an empty stack with a fixed size of 10. This stack will hold integer values.

2. Pushing Random Numbers: We randomly generate three numbers and add them to the stack using the `push_element()` function. Each time we push an element onto the stack, it gets added on top of the existing elements.

3. Printing Stack Details: After pushing the initial three numbers, we print out the details of the stack. This includes showing the elements in the stack, whether the stack is empty or full, the number of items in the stack, and the first and last items in the stack.

4. Pushing More Numbers: We generate seven more random numbers and push them onto the stack. Since the stack has a fixed size of 10, it becomes full after adding these numbers.

5. Printing Updated Stack Details: We print out the stack details again to see the changes. We can observe that the stack is now full.

6. Accessing Element at Index 5: We retrieve the element at index 5 (the 6th element in the stack). This demonstrates how we can access specific elements in the stack.

7. Popping Elements: We pop five elements from the stack using the `pop_element()` function. Each time we pop an element, it is removed from the top of the stack.

8. Printing Updated Stack Details: We print out the stack details once more to see the updated state of the stack after popping elements.

9. Conclusion: The code demonstrates the basic operations of a stack data structure, including pushing, popping, and accessing elements. It also handles scenarios such as stack overflow and underflow gracefully, printing appropriate messages when these situations occur.

TASK 2: SINGLY LINKED LIST
Node Class:
- The `Node` class represents an individual element (or node) in the linked list.
- Each node has two attributes: `data` to store the value of the node, and `next` to store the reference to the next node in the list.
- The `__str__` method is overridden to provide a string representation of the node, displaying its data value and the address of the next node if it exists.

SinglyLinkedList Class:
- The `SinglyLinkedList` class represents the linked list itself.
- It has attributes including `length` to store the maximum length of the list and `head` to point to the first node in the list.
- The class provides methods to perform various operations on the linked list.

Methods:
1. is_empty(): Checks if the linked list is empty by verifying if the `head` attribute is `None`.
2. number_of_nodes(): Returns the total number of nodes in the linked list by traversing the list and counting the nodes.
3. insert(node): Inserts a new node at the end of the list. If the list is full, it prints a message indicating that the linked list is full.
4. delete(node): Deletes a specified node from the list. If the list is empty, it prints a message indicating an underflow condition. It updates the `head` attribute if the node to be deleted is the head, otherwise, it traverses the list to find the previous node and updates its `next` reference.
5. head_node(): Returns the head node of the list.
6. tail_node(): Returns the tail node of the list by traversing the list until it reaches the last node.
7. node_at_index(index): Returns the node at the specified index position in the list.
8. print_details(): Prints the details of the linked list including the nodes, whether the list is empty, the number of items in the list, the head element, and the tail element.

Main Code:
- In the main block, a `SinglyLinkedList` object is created with a maximum length of 10.
- Initially, the details of the empty list are printed.
- Random numbers are then generated and inserted into the list using the `insert` method.
- The details of the list are printed after each insertion.
- Similarly, random numbers are inserted, and the list details are printed again.
- The item at index 5 is retrieved and printed.
- Finally, the tail element is removed from the list five times, and the list details are printed after each removal. The number of items in the list is printed at the end.
