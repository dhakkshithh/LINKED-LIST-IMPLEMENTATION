# LINKED-LIST-IMPLEMENTATION

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: DHAKSHITH BAVAN S

*INTERN ID*: CT04DF1802

*DOMAIN*: C PROGRAMMING

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTHOSH

*DESCRIPTION OF TASK 2*:
          A singly linked list is a dynamic data structure that consists of nodes, where each node contains data and a pointer to the next node in the sequence. Unlike arrays, linked lists are not stored in contiguous memory locations, making them more efficient for operations like insertion and deletion, especially when the data size is unknown at compile time. Task 2 involves implementing a singly linked list in C with three primary operations: insertion, deletion, and traversal.

In this program, we first define a structure called Node using the struct keyword. Each node in the linked list contains two elements: an integer data field that stores the actual data, and a pointer next that points to the next node in the list. A global pointer head is declared to keep track of the beginning of the list.

The insertion operation is implemented using the insert function. In this example, nodes are inserted at the beginning of the list. A new node is dynamically allocated using malloc, and its data is initialized with the provided value. The new node’s next pointer is set to the current head of the list, and then head is updated to point to the new node. This effectively places the new node at the front, pushing all other nodes down the list.

Deletion is handled by the delete function, which removes the first occurrence of a node that matches a given value. The function iterates through the list using two pointers: temp (to track the current node) and prev (to track the previous node). If the target node is found, the pointers are adjusted to bypass the node to be deleted. If the node to be deleted is the head itself, the head is updated to the next node. After adjusting the links, the memory allocated to the deleted node is freed using the free function. If the value is not found, a message is printed to indicate that the deletion could not be performed.

The traversal of the linked list is managed by the display function. It begins at the head of the list and iterates through each node until it reaches NULL (indicating the end of the list). At each step, the function prints the node’s data followed by an arrow (→) to visually represent the list's structure.

To execute this program:

    Save the code to a file named linked_list.c.

    Open a terminal or command prompt.

    Compile using GCC: gcc linked_list.c -o linked_list

    Run the program: ./linked_list

Expected output:
The program first inserts three values: 10, 20, and 30. Since each new node is inserted at the beginning, the list looks like: 30 → 20 → 10 → NULL. When the delete function is called to remove the node with value 20, it successfully finds and removes it, resulting in the updated list: 30 → 10 → NULL.

This task demonstrates a fundamental concept in data structures that underpins more complex structures like stacks, queues, and graphs. Understanding singly linked lists is essential for efficient memory management and for problems where the size of the dataset is unpredictable at compile time.

*OUTPUT

![Image](https://github.com/user-attachments/assets/c7c38af9-ee93-4bfe-aa1f-f876c5512c59)
