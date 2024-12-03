# Binary Trees

This repository contains implementations of binary tree data structures and operations, as defined in the project requirements. The project includes basic binary trees, Binary Search Trees (BSTs), AVL Trees, and Max Binary Heaps.

## Data Structures

All data structures are defined in the project's header file. Below is an overview of the data structures used.

### Basic Binary Tree

```c
/**
 * struct binary_tree_s - Binary tree node
 *
 * @n: Integer stored in the node
 * @parent: Pointer to the parent node
 * @left: Pointer to the left child node
 * @right: Pointer to the right child node
 */
struct binary_tree_s
{
    int n;
    struct binary_tree_s *parent;
    struct binary_tree_s *left;
    struct binary_tree_s *right;
};

typedef struct binary_tree_s binary_tree_t;

Binary Search Tree (BST)
A Binary Search Tree is implemented using the same structure as the basic binary tree.

typedef struct binary_tree_s bst_t;

AVL Tree
An AVL Tree is a self-balancing binary search tree that also uses the basic binary tree structure.

typedef struct binary_tree_s avl_t;

Max Binary Heap
A Max Binary Heap is a complete binary tree where the value of each node is greater than or equal to the values of its children.

typedef struct binary_tree_s heap_t;

Project Requirements
Tasks 0 to 23:
Deal exclusively with simple binary trees.
No specific rules like those of BSTs, AVL Trees, or Heaps are enforced.
General Notes:
All functions and data structures are implemented in C.
The header file contains all required type definitions and function prototypes.
File Structure
binary_tree.h: Header file containing all type definitions and function prototypes.
*.c: Source files containing implementations of various binary tree operations.
README.md: Project overview and documentation.
Compilation and Testing
All code should be compiled using gcc with the following flags:

gcc -Wall -Werror -Wextra -pedantic *.c -o binary_trees

Usage
Include the binary_tree.h header file in your programs to access the binary tree structures and functions. Here's an example:

#include "binary_tree.h"

int main(void)
{
    binary_tree_t *root;

    root = binary_tree_node(NULL, 42);
    printf("Root node value: %d\n", root->n);

    return (0);
}

License
This project is for educational purposes and is licensed under the MIT License.
Author
Shighi

Feel free to modify the contents based on additional project details or personal preferences.


