---
description: https://github.com/caleberi/devon-hash-table
---

# Devon

This project involves the design and implementation of a hash table data structure using an associative array API. Hash tables are fundamental data structures known for their efficiency in insert, search, and delete operations. The project is particularly focused on creating a string-based hash table with chaining to handle collisions, ensuring scalable performance across various use cases.

#### Key Features:

* **Hash Table with Chaining**: Utilizes chaining to manage collisions effectively, maintaining efficiency even in densely populated hash tables.
* **Dynamic Resizing**: Implements dynamic resizing to balance memory usage and performance, including both upscaling and downscaling based on the number of elements.
* **Double Hashing**: Employs a double hashing technique for effective index determination, reducing the likelihood of collision.
* **Associative Array API**: Provides a clear and intuitive API for hash table operations, including insertion, deletion, and lookup.
* **Robust Memory Management**: Ensures proper memory allocation and deallocation to prevent leaks and manage resources efficiently.

#### Components:

* **Hash Table Node (`hash_table_node`)**: Represents individual entries in the hash table, storing key-value pairs.
* **Hash Table Structure (`hash_table`)**: Encapsulates the core data structure, managing an array of pointers to `hash_table_node` items, along with metadata like size and count.
* **Helper Functions**: Includes functions for creating, resizing, and deleting hash table items and the table itself.

#### Technical Details:

* **Hash Functions**: Implements robust hash functions and double hashing for efficient key indexing.
* **Memory Allocation**: Utilizes dynamic memory allocation for flexible table resizing and efficient memory usage.
* **C Language**: Written in C for performance and fine-grained control over memory management.

#### Usage:

This hash table implementation can be employed in various applications requiring efficient key-value storage and retrieval. It is suitable for tasks like caching, indexing, and associative arrays in software systems where performance is critical.

#### Author:

* **Hebronace**
* **Date**: April 5, 2019

This project showcases the practical application of fundamental computer science concepts and demonstrates proficiency in data structure implementation, memory management, and performance optimization.
