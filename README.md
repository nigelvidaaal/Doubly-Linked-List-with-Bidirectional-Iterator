# Doubly-Linked List in C++  

A fully implemented **Doubly-Linked List** in C++ with a **bidirectional iterator**. This project demonstrates key concepts of **Object-Oriented Programming (OOP)**, **templates**, and **memory management** in C++.  

---

## Features

- Generic **template-based** linked list supporting any data type.
- Fully functional **Node insertion** and **deletion**.
- Supports **push_front**, **push_back**, **pop_front**, **pop_back**, and **insert/erase at iterator positions**.
- Implements a **bi-directional iterator** for traversal.
- Overloaded operators:
  - `==` and `!=` for comparing two lists.
  - Assignment (`=`) and move semantics.
- Memory-safe with proper handling of **dynamic allocation and deallocation**.
- Includes **swap**, **clear**, and **size** functions.

---

## Files

- `llist2.hpp` – Header file containing the class definition and all member functions.
- `main.cpp` (optional) – Example usage/testing of the doubly-linked list.

---

## Usage

```cpp
#include "llist2.hpp"
#include <iostream>

int main() {
    LList<int> list = {1, 2, 3, 4};

    // Insert element at the beginning
    list.push_front(0);

    // Iterate through the list
    for(auto it = list.begin(); it != list.end(); ++it) {
        std::cout << *it << " ";
    }

    return 0;
}
