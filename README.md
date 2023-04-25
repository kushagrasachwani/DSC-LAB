# Link-list
A linked list is a data structure that consists of a sequence of nodes, where each node contains a data value and a reference (pointer) to the next node in the sequence. Linked lists are commonly used in computer programming for dynamic memory allocation and data storage.
# Singly linked list
In a singly linked list, each node has a reference to the next node in the sequence, but not to the previous node. The last node in the sequence has a reference to NULL. Here's an example of a singly linked list:

```
typedef struct node{
    int data;
    struct node* next;
}node;

node* head = NULL;

void insert(int value){
    node* new_node = (node*) malloc(sizeof(node));
    new_node->data = value;
    new_node->next = head;
    head = new_node;
}

void traverse(){
    node* current = head;
    while(current != NULL){
        printf("%d ", current->data);
        current = current->next;
    }
}
```

# Algorithm :
1. Create a structure node that has two members, one is info that is used to store the data items and another is next field that store the address of next node in the list.

2. Create starting pointer of the structure datatype.

3. Create a node, use the malloc function to dynamically allocate memory for the new node.

4. After creating the node, store the new item in the node using a pointer to that node.


5. Create function display , containing temp pointer pointing at the start node and further temp updates to new address.
# Screenshot
![p14](https://user-images.githubusercontent.com/126184012/234321022-2ea8bf07-9b69-4216-a333-c9dc46e5b7c6.png)

 # Application
 1. Dynamic memory allocation
2. Implemented in stack and queue
3. In undo functionality of softwares
4. Hash tables, Graphs
