

## What are Data Structures?
A **data structure** is a systematic way of organizing, managing, and storing data so it can be accessed and modified efficiently.  
They are fundamental to computer science, as they directly impact the **performance** of algorithms in terms of **time** and **space**.



## Arrays
An **array** is a **linear data structure** that stores elements in **contiguous memory locations**.  
Each element is identified by an **index**, starting from `0` in most programming languages.

### Characteristics
- Fixed size (cannot grow or shrink once declared).
- Random access: directly access an element in **O(1)** time using index.
- Insertion and deletion can be costly since elements may need shifting.

### Example (C-style)
```c
int arr[5] = {10, 20, 30, 40, 50};
```

## Linked Lists
A linked list is a linear data structure where elements (called nodes) are stored in non-contiguous memory locations.

Each node contains two parts:
- Data
- Pointer (reference) to the next node

## Types of Linked Lists
- **Singly Linked List:** Each node points to the next.
- **Doubly Linked List:** Each node has pointers to both the previous and next nodes.
- **Circular Linked List:** Last node points back to the first.

## Characteristics
- Dynamic size (nodes can be added or removed at runtime).
- Sequential access (need to traverse from head node).
- Extra memory required for storing pointers.

## Example (Singly Linked List Node in C)

```c
struct Node {
    int data;
    struct Node* next;
};
```

## Linked List Visualization (Singly)
[10 | next] → [20 | next] → [30 | next] → [40 | next] → NULL



# Time & Space Complexity

## Time Complexity Notations

## Big-O Notation (O)
- Represents the **upper bound** of an algorithm's running time.  
- Describes the **worst-case scenario**.  


## Theta Notation (Θ)
- Represents the **tight bound** of an algorithm's running time.  
- Describes the **average-case or typical performance**.

## Omega Notation (Ω)
- Represents the **lower bound** of an algorithm's running time.  
- Describes the **best-case scenario**.


## Summary Table

| Notation | Meaning              | Scenario        |
|----------|-------------------|-------------------|
| O(n)     | Upper bound        | Worst-case         | 
| Θ(n)     | Tight bound        | Average/typical    | 
| Ω(n)     | Lower bound        | Best-case          |


## Arrays
- **Access**: Θ(1)  
- **Search**: O(n) for linear search, O(log n) if sorted with binary search  
- **Insertion**: O(n)  
- **Deletion**: O(n)  



## Linked Lists
- **Access**: O(n) (sequential traversal only)  
- **Search**: O(n)  
- **Insertion (at head/tail with pointer)**: Θ(1)  
- **Deletion (with pointer to node)**: Θ(1)  



## Space Complexity
- **Arrays**: Θ(n) (only data)  
- **Linked Lists**: Θ(n) for data + Θ(n) for pointers → effectively Θ(2n)  


# Arrays vs Linked Lists Comparison

| Feature                  | Arrays                              | Linked Lists                         |
|---------------------------|-------------------------------------|---------------------------------------|
| **Memory Allocation**     | Contiguous                         | Non-contiguous                        |
| **Size Flexibility**      | Fixed                              | Dynamic                               |
| **Access Time**           | Θ(1) (direct access by index)      | O(n) (sequential traversal)           |


