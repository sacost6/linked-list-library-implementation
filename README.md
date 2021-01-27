## linked-list-library-implementation

# Some Requirements
For this program, we were required to implement a linked list class which had some requirements as follows:

* Write a function which returns the length of the calling list in O(1) time
* Write a function that constructs a new list of the same length as the calling object with the value stored at
position i of the new list is the MAXIMUM value in the suffix (or tail) of the calling list starting from position i in O(n) time
* Write a function that removes all elements of the calling list which are less than or equal to parameter value in THETA(n) time
* Write a function that concatenates the calling list and parameter list without copying parameter list in O(1) time

# Solutions
This project was written as a header for a singly Linked List. In order to implement the following requirements, my solutions were as follows:

* Within the Linked List class, an integer value was required to keep track of the size. This value was incremented
or decreased depending on whether something was added or deleted into the list. A getter function was used to
return the size of the calling list.
* Using a reverse helper function, I obtain a new list that is the reverse list of the calling list. Then, I keep track of the
smallest number encountered beginning at the end of the calling list going backwards. I fill a new list with the smallest
number encountered and return this.
* Able to delete all matching values in the calling list by simply traversing the calling list starting at the head and deleting
all values matching the parameter. Was not able to create new nodes for this but simply relinking exisiting nodes.
* Able to concatenate two existing lists by simply re-linking the end of the calling node and the head of parameter list.
