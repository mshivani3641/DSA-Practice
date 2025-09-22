Algorithm:
•	Insertion:
•	At the Beginning:
•	Create a new node and assign the given value to its data.
•	Set the next of the new node to point to the current head of the list.
•	Update the head of the list to be the new node. 
  
•	At the End:
•	Create a new node and assign the given value to its data, setting its next to NULL.
•	If the list is empty, set the head to the new node.
•	Otherwise, traverse the list to find the last node (whose next is NULL).
•	Set the next of the last node to point to the new node.

•	At a Specific Position:
•	Create a new node and assign the given value to its data, setting its next to NULL.
•	If the position is 1, insert at the beginning.
•	Otherwise, traverse the list to the node before the desired position.
•	Set the next of the new node to point to the node that was originally after the previous node.
•	Set the next of the previous node to point to the new node.
  
•	Deletion:
•	From the Beginning:
•	If the list is empty, return.
•	Store the current head in a temporary variable.
•	Update the head to point to the next node.
•	Deallocate the memory of the temporary node.
  
•	From the End:
•	If the list is empty, return.
•	If there's only one node, delete the head and set head to NULL. 
•	Otherwise, traverse the list to the second-to-last node.
•	Store the last node in a temporary variable.
•	Set the next of the second-to-last node to NULL. 
•	Deallocate the memory of the temporary node.
•	From a Specific Position or by Value:
•	If the list is empty, return.
•	If deleting the first node, follow the "From the Beginning" algorithm.
•	Otherwise, traverse the list to the node before the node to be deleted. 
•	Store the node to be deleted in a temporary variable.
•	Set the next of the previous node to point to the node after the deleted node.
•	Deallocate the memory of the temporary node.


•	Traversal:
•	Initialize a temporary pointer to the head of the list. 
•	While the temporary pointer is not NULL:
•	Access or process the data of the current node.
•	Move the temporary pointer to the next node.

•	Searching:
•	Initialize a temporary pointer to the head of the list. 
•	While the temporary pointer is not NULL:
•	Compare the data of the current node with the target value.
•	If a match is found, return true (or the node itself).
•	Move the temporary pointer to the next node.
•	If the loop finishes without finding the value, return false.

