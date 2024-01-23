# 0x1B. C - Sorting algorithms & Big O

## Project Description

This project aims to implement and understand various sorting algorithms in the C programming language. It is to be completed in teams of two, with a focus on pair programming for the mandatory part. The project must be started by Jan 17, 2024, 6:00 AM, and should be completed by Jan 24, 2024, 6:00 AM. The checker was released on Jan 19, 2024, 12:00 AM, and an auto-review will be launched at the deadline.

## Learning Objectives

Upon completion of this project, you should be able to:

- Implement at least four different sorting algorithms.
- Explain the concept of Big O notation and evaluate the time complexity of an algorithm.
- Select the best sorting algorithm for a given input.
- Understand what constitutes a stable sorting algorithm.

## Resources

Before starting the project, make sure to read or watch materials on sorting algorithms, Big O notation, and related topics. Some suggested resources include:

- Sorting algorithm documentation.
- Big O notation explanations.
- Sorting algorithms animations.
- "15 sorting algorithms in 6 minutes" (Note: This video may trigger seizures/epilepsy and is not required for the project).
- CS50 Algorithms explanation by David Malan.
- Additional reading on sorting algorithms.

## Requirements

### General

- Allowed editors: vi, vim, emacs.
- All files will be compiled on Ubuntu 20.04 LTS using gcc with the options `-Wall -Werror -Wextra -pedantic -std=gnu89`.
- All files should end with a new line.
- A README.md file at the root of the project folder is mandatory.
- Code should follow the Betty style and will be checked using `betty-style.pl` and `betty-doc.pl`.
- Avoid using global variables.
- No more than 5 functions per file.
- Unless specified otherwise, do not use the standard library. Functions like printf, puts, etc., are forbidden.
- Prototypes of all functions should be included in the header file called `sort.h`.
- Push the header file and ensure it is include guarded.
- A list/array does not need to be sorted if its size is less than 2.

### GitHub

- There should be one project repository per group. Cloning/forking a project repository with the same name before the second deadline may result in a 0% score.

## Data Structure and Functions

The project provides the following functions:

```c
#include <stdlib.h>
#include <stdio.h>

/**
 * print_array - Prints an array of integers
 *
 * @array: The array to be printed
 * @size: Number of elements in @array
 */
void print_array(const int *array, size_t size);

/**
 * print_list - Prints a list of integers
 *
 * @list: The list to be printed
 */
void print_list(const listint_t *list);
```

Additionally, a doubly linked list structure is provided:

```c
/**
 * struct listint_s - Doubly linked list node
 *
 * @n: Integer stored in the node
 * @prev: Pointer to the previous element of the list
 * @next: Pointer to the next element of the list
 */
typedef struct listint_s
{
    const int n;
    struct listint_s *prev;
    struct listint_s *next;
} listint_t;
```

Ensure that the prototypes for `print_array` and `print_list` are included in the `sort.h` header file.

## Big O Notation

Understand and use the following notations:

- O(1)
- O(n)
- O(n!)
- O(n^2) - n square
- O(log(n)) - log(n)
- O(n * log(n)) - n * log(n)
- O(n + k) - n + k

Use the short notation without constants. Example: O(nk) or O(wn) should be written as O(n).

## Tests

To test sorting algorithms with large sets of random integers, consider using Random.org.

## Contact

For any questions or clarifications, contact Victor Ochuba.
