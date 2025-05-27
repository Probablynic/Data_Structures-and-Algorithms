Algorithms
  
- A clear set of step-by-step instructions that tells the computer what to perform producing the required output.

Variables
  
- A named storage that our programs can manipulate

- Each has a specific type which determines the size and layout in the use of memory

- Range of values that can be stored within that memory

- Set of operations that can be applied to the variable

- Declare first before they can be used

Types of Data Structures

Linear:

- Arrays, Stacks, Queues, Linked Lists.

Non-Linear:

- Trees, Graphs.

Dynamic:

- Dynamic Arrays, Hash Tables.

Types of Variables: Two data types available in Java:

1. Primitive Data Types - predefined by the language and named by a keyword
   
- byte     - an 8-bit (size) signed 2's complement integer. -128 up to 127(range).

- Short    - 16-bit signed 2’s complement integer., -32,768 up to 32,767.

- Int      - a 32-bit signed 2s complement integer; - 2,147,483,648 up to 2,147,483,647.

- long     - a 64-bit signed 2's complement integer.

- Float    - a single-precision 32-bit IEEE 754 floating point.

- Double   - a double-precision 64-bit IEEE 754 floating point.

- Boolean  - represents one bit of information. Only two possible values: true and false.
  
- Char     - a single 16-bit Unicode character. Used to store any character.


2. Reference Data Types / Non-Primitive Data Types
   
- created using defined constructors of the classes
  
- used to access objects
  
- declared to be of a specific type that cannot be changed.
  
  For example, Employee, Puppy etc.
  
- Class objects, and various type of array variables come under reference data type.

- Default value of any reference variable is null.

- A reference variable can be used to refer to any object of the declared type or any compatible type.
  For example: Animal animal = new Animal("giraffe");

Java Literals:

- a source code representation of a fixed value.
  
- represented directly in the code without any computation.
  
- can be assigned to any primitive type variable.
  
- For example: byte a = 68; char a = 'A‘ 

- byte, int, long, and short can be expressed in decimal(base 10), hexadecimal(base 16) or octal(base 8) number systems as well.
  
- Prefix 0 is used to indicate octal and prefix 0x indicates hexadecimal when using these number systems for literals.
  
- For example: int decimal = 100; int octal = 0144; int hexa = 0x64;

- String literals in Java are specified like they are in most other languages by enclosing a sequence of characters between a pair of double quotes.

- Examples of string literals are: "Hello World" "two\nlines" "\"This is in quotes\"“
  
- String and char types of literals can contain any Unicode characters. 

- For example: char a = '\u0001'; String a = "\u0001";

Java language supports few special escape sequences for String and char literals as well. They are:

Notation Character represented

-    \n         - Newline (0x0a)
   
-    \r         - Carriage return (0x0d)
   
-    \f         - Formfeed (0x0c)
   
-    \b         - Backspace (0x08)
   
-    \s         - Space (0x20)
   
-    \t         - tab
   
-    \"         - Double quote
   
-    \'         - Single quote
   
-    \\         - backslash
   
-    \ddd       - Octal character (ddd)
   
-    \uxxxx     - Hexadecimal UNICODE character (xxxx)
   

Data Abstraction

- Hiding implementation details.

- Focuses on functionality (what it does) over process (how it does).

- Real-world example: Driving a car without knowing engine mechanics.

Real-Life Examples of Data Abstraction

- ATMs: Perform cash withdrawal without knowing internal mechanisms.

- Mobile Apps: Focus on user interface, not backend code.

- Libraries in programming: Use functions without seeing internal code.

Abstract Data Types (ADTs)

- ADTs define operations and behavior without implementation.

Examples:

- Stack: push, pop, peek.

- Queue: enqueue, dequeue, front.

- List: add, remove, get.

Characteristics of ADTs

- Encapsulation: Combines data and operations.

- Modularity: Independent components.

- Flexibility: Multiple implementations possible.


Common ADT Implementations

- Stack: - Implementation: Array or Linked List.

- Queue: - Types: Circular Queue, Priority Queue.
  

Water Tank ADT Example

• Attributes: 

- Capacity: Max water.

- Current level: Current water.
              
• Methods:    

- add_water(amount).

- remove_water(amount).
              
- check_level().


/*

                            Types of Data Structure
                                   |
         ---------------------------------------------------
         |                                                 |
Primitive Data Structure                    Non-Primitive Data Structure
         |                                                 |
------------------------------------------------     ----------------------------
|        |        |         |                      Linear Data Structure     Non-Linear Data Structure
Integer  Float  Character  Boolean               |                          |
                                              -----------------------     ---------------------
                                              |    |     |     |         |                   |
                                           Arrays Linked Stack Queue   Trees              Graphs


*/

Stacks
- A stack is a data structure of ordered items such that items can be inserted and removed only at one end.
  
- A stack is a LIFO (Last-In/First-Out) data structure
  
- A stack is sometimes also called a pushdown store.

What can we do with a stack?

- push - place an item on the stack
  
- peek - Look at the item on top of the stack, but do not remove it
  
- pop - Look at the item on top of the stack and remove it

What happens if we try to pop an item off the stack when the stack is empty?

- This is called a stack underflow.

Interface IStack

- Interface Istack {
  boolean empty();
  void push(char c);
  char pop();
  char peek();
}

Implementing a Stack

There are two ways we can implement a stack:

- Using an array
  
- Using a linked list

Queue
- A data structure of ordered items such that items can be inserted only at one end and removed at the other end.
  
- A queue is called a FIFO (First in-First out) data structure.

What can we do with a queue?

- Enqueue - Add an item to the queue
  
- Dequeue - Remove an item from the queue

What are some applications of queues?

- Round-robin scheduling in processors
  
- Input/Output processing
  
- Queueing of packets for delivery in networks

Implementing a Queue

Just like a stack, we can implementing a queue in two ways:

- Using an array
  
- Using a linked list

Using an array to implement a queue is significantly harder than using an array to implement a stack. Why?

- Unlike a stack, where we add and remove at the same end, in a queue we add to one end and remove from the other.
  
- Front of the queue is stored as the head node of the linked list, rear of the queue is stored as the tail node.
  
- Enqueue by adding to the end of the list
  
- Dequeue by removing from the front of the list.

INTRODUCTION TO LINKED LISTS
UNDERSTANDING LINKED LIST STRUCTURES IN DATA STRUCTURES

LINKED LIST

- A linked list is a linear data structure.
  
- Unlike arrays, linked lists do not have a fixed size.
  
- Elements (nodes) are linked using pointers.
  
LINKED LISTS PURPOSE

- Dynamic memory allocation.
  
- Efficient insertions and deletions.
  
- No memory wastage compared to arrays.
  
- Used in applications like memory management, navigation systems, etc.

TYPES OF LINKED LISTS

- Singly Linked List (One-way linking)
  
- Doubly Linked List (Two-way linking)
  
- Circular Linked List (Last node points to first node)

SINGLY LINKED LIST - STRUCTURE

Each node contains:

- Data
  
- Pointer to the next node
  
Example Representation:

- head -> [Data | Next] -> [Data | Next] -> NULL

SINGLY LINKED LIST OPERATIONS

- Insertion
  
- Deletion
  
- Traversal

DOUBLY LINKED LIST - STRUCTURE

Each node contains:

- Data
  
- Pointer to the previous node
  
- Pointer to the next node
  
Example Representation:

- NULL <- [Prev | Data | Next] <-> [Prev | Data | Next] -> NULL

DOUBLY LINKED LIST - OPERATIONS

- Insertion: Can be done at the beginning, middle, or end.

- Deletion: More efficient than singly linked list.

- Traversal: Can traverse both forward and backward.

SUMMARY & CONCLUSION

- Linked lists provide dynamic memory management.
  
- Singly linked lists use one pointer per node.
  
- Doubly linked lists use two pointers, enabling bidirectional traversal.
  
- Choosing between them depends on the specific use case.
