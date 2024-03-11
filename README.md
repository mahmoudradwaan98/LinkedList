# LinkedList
Linked List implementation using  C 

1- Linear Data structure, Dynamic allocation, No memory unused

2- Elements are linked using pointers

3- Elements are not stored at Contiguous memory locations

               Node 1            Node 2            Node 3
4-  Head --> (Data , Next) --> (Data , Next) --> (Data , Next) --> NULL

   Each node contains a reference link to the next node in the List

5- Linked List Types: Single, Double, Circular

6- Linked List node creation :

typedef struct node{

	u32 value;            // Data
	struct node * Next;   // address of next element 

}node_t;

7- Steps to add a node to Linked List End :

	a- Create a new node
	b- assign data, Next = NULL
	c- traverse through the linked list to reach the final node
	d- assign final node`s next to the new node 

8- Steps to add a node to Linked List Middle :

	a- Create a new node
	b- assign data, Next = NULL
	c- assign ptr to the head of the node
	d- get preposition node
	e- assign new node`s next to the preposition node 

9- Disadvantages of the Linked list : 

1- Extra memory space for a pointer is required with each element of the list

2- Random access is not allowed. we have to access elements sequentially starting from the first node (we can not use binary search with LinkedList with its default implementation )

3- searching for an element is costly and requires O(n) time complexity 

4- Not Cache friendly since array elements are contiguous locations, a locality of reference does not exist in the linked list. 

5- sorting LinkedList is complex and costly -->  it takes a lot of time to traverse and change the pointers.

6- reverse traversing is not possible in a single linked list, it will be confusing when we work with pointers

7- Direct access to an element is impossible in the linked list as an array by index.







