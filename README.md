# Singly linked list

Linked List can be defined as collection of objects called nodes that are randomly stored in the memory.
A node contains two fields i.e. data stored at that particular address and the pointer which contains the address of the next node in the memory.
The last node of the list contains pointer to the null.
![image](https://user-images.githubusercontent.com/125941580/230759816-dcf6549d-54d8-4a91-8942-bc02cd8abd67.png)

# Why use linked list over array?

1.Better use of Memory: From a memory allocation point of view, linked lists are more efficient than arrays. Unlike arrays, the size for a linked list is not pre-defined, allowing the linked list to increase or decrease in size as the program runs.
2.Fast Insertion/Deletion Time: Inserting a new node to the beginning or end of a linked list takes constant time (O(1)) as the only steps are to initialize a new node and then update the pointers. Likewise, if there were a tail pointer (similar to the head pointer) insertion to the end of the linked list would also be O(1). Similarly, deletion of the nodes at the beginning and end of the linked list take constant time while deleting a node in the middle of the linked list takes linear time.

# Algorithm :
1.Create a structure node that has two members, one is info that is used to store the data items and another is next field that store the address of next node in the list.

2.Create starting pointer of the structure datatype.

3.Create a node, use the malloc function to dynamically allocate memory for the new node.

4.After creating the node, store the new item in the node using a pointer to that node.

 newnode1->data=2;  // newnode1 accessing the data variable of struct node.
 newnode1->next=newnode2; // Address of next node stored in variable next of struct node.
 
5.Create function display , containing temp pointer pointing at the start node and further temp updates to new address.

   struct node *temp;
   temp=start;
   temp=temp->next; // address of next stored in temp
   
  # Linked List Applications
  
1.Dynamic memory allocation
2.Implemented in stack and queue
3.In undo functionality of softwares
4.Hash tables, Graphs
