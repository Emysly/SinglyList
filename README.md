# SinglyList
## A program to create and display a singly linked list


The singly linked list is a linear data structure in which each element of the list contains a pointer which points to the next element in the list. Each element in the singly linked list is called a node. Each node has two components: data and a pointer next which points to the next node in the list. The first node of the list is called as head, and the last node of the list is called a tail. The last node of the list contains a pointer to the null. Each node in the list can be accessed linearly by traversing through the list from head to tail.

Java Program to create and display a singly linked list
Consider the above example; node 1 is the head of the list and node 4 is the tail of the list. Each node is connected in such a way that node 1 is pointing to node 2 which in turn pointing to node 3. Node 3 is again pointing to node 4. Node 4 is pointing to null as it is the last node of the list.

Psuedocode
Create a class Node which has two attributes: data and next. Next is a pointer to the next node.
Create another class which has two attributes: head and tail.
addNode() will add a new node to the list:
Create a new node.
It first checks, whether the head is equal to null which means the list is empty.
If the list is empty, both head and tail will point to the newly added node.
If the list is not empty, the new node will be added to end of the list such that tail's next will point to the newly added node. This new node will become the new tail of the list.
a. display() will display the nodes present in the list:
Define a node current which initially points to the head of the list.
Traverse through the list till current points to null.
Display each node by making current to point to node next to it in each iteration.



--------------------------------------------------------------------------------------------------------------------------------------------------------------------

# CountNodes
## Java program to create a singly linked list of n nodes and count the number of nodes

In this program, we need to create a singly linked list and count the nodes present in the list.

Java program to create a singly linked list of n nodes and count the number of nodes
To accomplish this task, traverse through the list using node current which initially points to head. Increment current in such a way that current will point to its next node in each iteration and increment variable count by 1. In the end, the count will hold the value which denotes the number of nodes present in the list.


Algorithm
Create a class Node which has two attributes: data and next. Next is a pointer to the next node in the list.
Create another class which has two attributes: head and tail.
addNode() will add a new node to the list:
Create a new node.
It first checks, whether the head is equal to null which means the list is empty.
If the list is empty, both head and tail will point to the newly added node.
If the list is not empty, the new node will be added to end of the list such that tail's next will point to a newly added node. This new node will become the new tail of the list.
a. countNodes() will count the nodes present in the list:


Define a node current which will initially point to the head of the list.
Declare and initialize a variable count to 0.
Traverse through the list till current point to null.
Increment the value of count by 1 for each node encountered in the list.
a. display() will display the nodes present in the list:

Define a node current which will initially point to the head of the list.
Traverse through the list till current points to null.
Display each node by making current to point to node next to it in each iteration.

-----

Java program to create a singly linked list of n nodes and display it in reverse order
In this program, we need to create a singly linked list and display the list in reverse order.

Original List

![](https://static.javatpoint.com/corebasic/programs/images/java-program-to-create-a-singly-linked-list-of-n-nodes-and-display-it-in-reverse-order.png)

Reversed List

![](https://static.javatpoint.com/corebasic/programs/images/java-program-to-create-a-singly-linked-list-of-n-nodes-and-display-it-in-reverse-order2.png)

One of the approaches to solving this problem is to reach the end the of the list and display the nodes from tail to head recursively.

Algorithm
Create a class Node which has two attributes: data and next. Next is a pointer to the next node in the list.
Create another class which has two attributes: head and tail.
addNode() will add a new node to the list:
Create a new node.
It first checks, whether the head is equal to null which means the list is empty.
If the list is empty, both head and tail will point to the newly added node.
If the list is not empty, the new node will be added to end of the list such that tail's next will point to the newly added node. This new node will become the new tail of the list.
a. reverse() will reverse the order of the nodes present in the list.

This method checks whether node next to current is null which implies that, current is pointing to tail, then it will print the data of the tail node.
Recursively call reverse() by considering node next to current node and prints out all the nodes in reverse order starting from the tail.
a. display() will display the nodes present in the list:

Define a node current which will initially point to the head of the list.
Traverse through the list till current points to null.
Display each node by making current to point to node next to it in each iteration.

