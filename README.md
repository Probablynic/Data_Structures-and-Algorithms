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
