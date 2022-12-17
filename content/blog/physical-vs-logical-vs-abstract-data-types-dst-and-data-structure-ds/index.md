---
title: "Physical vs Logical vs Abstract Data Types (DST) and data structure (DS)"
date: 2022-12-16
description: "Physical, logical, abstract data types and data structure terminology simplifed with examples"
tags: ["dsa"]
showTableOfContents: true
---

This articles breakdown the terminology used in trees data structure, as well as some types of trees and their use cases, to get familiar with them.

<!--more-->

All computer science is about abstraction as everything is binary, and thats why its sometimes hard to learn, lets break down this terminology.

## Abastract data types

Also known as ADT, lets start our discussion about the primitives or scalar types.

- Abstract data types is abstracting away 0 and 1 from us,
- Representation and operations, each data types, is represented in some specific way, and can have a set of operations to it.
    - 16 bit intger is 15 bit of 1 and 0, and the left most bit is wether its a signed or unsigned integer.
    - Arthmetic Operations can be done on integers addition, subtraction, multiplication division modulos
        - Relational operations, less than greater than, increment than decrement..ect
- Primitives or scalar types, is the programming language provided types, like integers, strings, floats..ect
- We dont concern our selves too much how internally this operations are performed.

When we learn programming languages, we mostly learn about representation of data, mostly scalar types, or primitive types and the operations we can do to them.

So the concept of representation and definition of data, and operations on the. while hiding the internal details is in essence abstract data types

For example in programming languages, we define classes, which has objects, and we give those special behaviours and different details, this is how we define them and there operations. for example we can create a class of linkedlists, with different operations

- Add(element, index) or inserrt(element, index)
- Append(element)
- Remove(element)
- Set(element)
- Get(index)
- Search(key)
- Sort()
- ….

This is how we create our own abstract data types, but the thing is, there is some very known and efficient data types, we call them data structure, they allow us to efficiently utilize the resources, the main memory in the most ideal way, and we extend the programming languages to perform what we want us, us developers.

## Physical data structure

Data structure is collection of data structure, so multiple data stored together.

This data structure defines how memory is allocated, they define how the memory will be organized in order for them to store the data.

### Arrays

- Most programming languages supports arrays
- its a collection of memory allocation, side by side, back to back.
- Arrays are fixed size, or arrays size is static, we cannot increase or decrease an array size after its creation, we can only assign to it, or desctruct it (deallocate the memory)
- Arrays can be created in the stack or the heap, we use a pointer to allocate arrays in the heap.
- We use arrays when we know the maximum number of elements we need

### Linedlist

- Lined lists are dynamic by nature, you can add more elements or delete them.
- its a collceiton of data, where each piece is called a node
- Each node holds data, and a pointer to the next node.
- Lined lists live in the heap, the head pointer can be in the stack.

## Logical data structure

This data structure, are an abstraction over the physical datastructure, Physical data structure store the data in memory, physically, but the logical data strucutre is the protocol, the discipline or the set of rules and policies we use to use the physical data structures in way we want for better organiztion of our data.

All operations we do to this data structure are defined also by the logic we set. the API.

This data structure can be split into two types, linear data structure, and non linear data structure.

### Linear data sturcture

linear data structure include

- Stack (LIFO)
- Queue (FIFO)

### Non linear data structure

- Tree
- Graph

### Tabluar

- Hash tables

## Big O notatian

Its how we analyse algorithms and operations on them, how efficient they are specially when we approach infinity. in respect of N input.

### Time complexity

To measure the performance of our data structure, our job is to find out how much work we do per N elements, means for example if to find a word in a dictionary takes you iterating through every single word, means thats Order of N, if you can find the word by just looking at a fraction of the book or a subset, there is high chances, its a log to the two of N, so time complexity is always in respect of our input, or how much element exists in the data we are working with, the job is not to find the exact time it takes, because that varies from machine to machine or from buzy processors to another..ect
Our job is to find the least amount of time we need to process N elements, we analyse the behaviour, how much more time we need to get the task done. a behaviour not an exact time.

### Space complexity

Many times, when we do something, we need extra memory than what we are working with, so in that case, we would have to consider that, because we dont always have extra memory, so thats the memory complexity it can be order of N or less or more, depends on the data type or algorithm we are working with.

- [https://www.bigocheatsheet.com/](https://www.bigocheatsheet.com/)
- [https://www-cs-faculty.stanford.edu/~knuth/taocp.html](https://www-cs-faculty.stanford.edu/~knuth/taocp.html)
- [https://en.wikipedia.org/wiki/Big_O_notation](https://en.wikipedia.org/wiki/Big_O_notation)
