---
title: "Basics of Programming"
date: 2023-02-17 12:45:00 +0500
LastModifierDisplayName: AbuTurab
LastModifierEmail: thesajid@proton.me
collapsibleMenu: true
alwaysOpen: false
weight: 3
---

## **Interpreted and Compiled Programming Languages**

### Programming Languages

- Common programming languages categories:
	- Interpreted
	- Compiled
- Many programming languages are compiled and interpreted
- The developer determines which languages is best suited for the project

### **Interpreted programming**
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming.webp)
  
- Some interpreted programming languages are outdated
- Some are more versatile and easier to learn languages
- Interpreted programming languages need an  interpreter to translate the source code
- Translators are built into the browser or require a program on your computer to interpret the code

#### Interpreted programming examples
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-1.webp)

### **Compiled programming**

- Programs that you run on your computer
- Packaged or compiled into one file
- Usually larger programs
- Used to help solve more challenging  problems, like interpreting source code
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-2.webp)

#### Examples
  
  Examples of compiled programming languages are:
- C, C++ and C# are used in many operating systems, like Microsoft. Windows, Apple macOS, and Linux
- Java works well across platforms, like the Android OS

#### Compiled programming
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-3.webp)

## **Comparing Compiled and Interpreted Programming Languages**

### Choosing a programming language
  
  Developers determine what programming language is best to use depending on:
- What they are most experienced with and trust
- What is best for their users
- What is the most efficient to use

### **Programming Languages**
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-4.webp)

#### Interpreted Programming Languages

- Also called script code or scripting, used to automate tasks
- Interpreter programs read and execute the source code line by line
- The source code need to be executed each time
- Runs on almost any OS with the right interpreter

#### Compiled programming languages

- Also called programming languages
- Used for more complex programs that complete larger tasks
- Larger programs installed on the computer or device
- Longer time to write the code but runs faster
- Grouped into one downloadable file

##### Interpreted vs. compiled
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-5.webp)

##### Programming Language examples

  **C, C++, C#**:
- Compiled programming language
- C is the original language, C++ and C# are variations
- Case sensitive
- Basis for Windows and many operating systems
- Takes more time to learn and use for coding but requires less memory and code runs faster
  
  **Java**:
- Compiled programming language
- Case-sensitive, object-oriented programming language
- Requires Java Virtual Machine (JVM) to run the code
- Programming language for Android OS
- Cross-platform language that runs the same code on macOS, Windows and Linux
  
  **Python**:
- Interpreted programming language
- Scripting language
- General-use, case-sensitive
- Used with Windows, macOS, and Linux OSes and with server-side web app code
- Requires Python engine to interpret code
  
  **JavaScript**:
- Interpreted
- Scripting language that runs on client side web browsers
- Case insensitive
- Simple scripts are run with HTML
- Complex scripts are run in separate files
- Not to be confused with Java, the compiled programming language
  
  **HTML**:
- Interpreted
- HyperText Markup Language
- Mostly case-insensitive
- Uses tags to format web pages on client-side web browsers

## **Query and Assembly Programming Languages**

### Programming language levels

- High-level programming languages
	- More sophisticated
	- Use common English
	- SQL, Pascal, Python
- Low-level programming languages
	- Use simple symbols to represent machine code
	- ARM, MIPS, X86

### **Query languages**

- A query is a request for information from a database
- The database searches its tables for information requested and returns results
- Important that both the user application making the query and the database handling the query are speaking the same language
- Writing a query means using predefined and understandable instructions to make the request to a database
- Achieved using programmatic code (query language/database query language)
- Most prevalent database query language is SQL
- Other query languages available:
	- AQL, CQL, Datalog, and DMX

#### SQL vs. NoSQL

- NoSQL (not only SQL)
- Key difference is data structures
- SQL databases:
	- Relational
	- Use structured, predefined schemas
- NoSQL databases:
	- Non-relational
	- Dynamic schemas for unstructured data

#### How does a query language work?
  
  Query language is predominantly used to:
- Request data from a database
- Create, read, update, and delete data in a database (CRUD)
- Database consists of structured tables with multiple rows and columns of data
  
  When a user performs a query, the database:
  1. Retrieves data from the table
  2. Arranges data into some sort of order
  3. Returns and prevents query results

#### Query statements

- Database queries are either:
	- Select commands
	- Action commands (CREATE, INSERT, UPDATE)
- More common to use the term “statement”
- Select queries request data from a database
- Action queries manipulate data in a database
#### Common query statements
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-6.webp)

#### Query statement examples

- SELECT * FROM suppliers;
- SELECT name FROM suppliers, WHERE name = ‘Mike’;
- CREATE DATABASE products;
- DROP TABLE suppliers;
- ALTER TABLE suppliers;
- DROP COLUMN firstname;
- SELECT AVG(purchases);
- FROM suppliers;

### **Assembly languages**

- Less sophisticated than query languages, structured programming languages, and OOP languages
- Uses simple symbols to represent 0s and 1s
- Closely tied to CPU architecture
- Each CPU type has its own assembly language

#### Assembly language syntax

- Simple readable format
- Entered one line at a time
- One statement per line
  
```armasm
{label} mnemonic {operand list} {;comment}
mov TOTAL, 212 ;Transfer the value 212 in the memory variable TOTAL
```

#### Assemblers

- Assembly languages are translated using an assembler instead of a compiler or interpreter
- One statement translates into just one machine code instruction
- Opposite to high-level languages where one statement can be translated into multiple machine code instructions
  
  Translate using mnemonics:
- Input (INP), Output (OUT), Load (LDA), Store (STA), Add (ADD)
  
  Statements consist of:
- Opcodes that tell the CPU what to do with data
- Operands that tell the CPU where to find the data

## **Understanding Code Organization Methods**

### **Code organization is important**
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-7.webp)
  
  Planning and organizing software design:
- Enables writing cleaner, more reliable code
- Helps improve code base
- Reduce bugs and errors
- Has a positive impact on program quality
- Provides consistent and logical format while coding

#### Pseudocode vs. flowcharts
  
  | Pseudocode                                                                | Flowcharts                                                                |
  | ------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
  | Informal, high-level algorithm description                                | Pictorial representation of algorithm, displays steps as boxes and arrows |
  | Step-by-step sequence of solving a problem                                | Used in designing or documenting a process or program                     |
  | Bridge to project code; follows logic                                     | Good for smaller concepts and problems                                    |
  | Helps programmers share ideas without extraneous waste of a creating code | Provide easy method of communication about logic behind concept           |
  | Provides structure that is not dependent on a programming language        | Offer good starting point for project                                     |

#### Flowcharts

- Graphical or pictorial representation of an algorithm
- Symbols, shapes, and arrows in different colors to demo a process of program
- Analyze different methods of solving a problem or completing a process
- Standard symbols to highlight elements and relationships
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-8.webp)
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-9.webp)

#### Flowchart software

- Provides ability to create flowcharts
- Drag functionality
- Easy-to-use interface
- Team collaboration creating flowcharts
  
  **Examples**:
- Microsoft Visio
- Lucidchart
- Draw.io
- DrawAnywhere

#### Pseudocode advantages

- Simply explains each line of code
- Focuses more on logic
- Code development stage is easier
- Words/phrases represent lines of computer operations
- Simplifies translation
- Code in different computer languages
- Easier review by development groups
- Translates quickly and easily to any computer language
- More concise, easier to modify
- Easier than developing a flowchart
- Usually less than one page

## **Branching and Looping Programming Logic**

### Introduction to programming logic
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-10.webp)

### Boolean expressions and variables
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-11.webp)

### Branching programming logic
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-12.webp)
  
  Branching statements allow program execution flow:
- if
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-13.webp)
- if-then-else
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-14.webp)
- Switch
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-15.webp)
- GoTo

### Looping programming logic
  
  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-16.webp)

  There are three basic loop statements:
- **While loop**: Condition is evaluated before processing, if true, then loop is executed
- **For loop**: Initial value performed once, condition tests and compares, if false is returned, loop is stopped
- **Do-While loop**:Condition always executed after the body of a loop

## **Introduction to Programming Concepts, Part 1**

### What are identifiers?

- Software developers use identifiers to reference program components
	- Stored values
	- Methods
	- Interfaces
	- Classes
- Identifiers store two types of data values:
	- Constants
	- Variables

### **What are containers?**

- Special type of identifier to reference multiple program elements
	- No need to create a variable for every element
	- Faster and more efficient
- Examples:
	- To store six numerical integers – create six variables
	- To store 1,000+ integers – use a container

#### Arrays

- Simplest type of container
- Fixed number of elements stored in sequential order, starting at zero
- Declare an array
	- Specify data type (Int, bool, str)
	- Specify max number of elements it can contain
- Syntax
	- Data type > array name > max array size [ ]

    ```array
    int my_array[50]
    ```


#### Vectors

- Dynamic size
- Automatically resize as elements are added or removed
	- a.k.a. ‘Dynamic arrays’
- Take up more memory space
- Take longer to access as not stored in sequential memory
- Syntax
	- Container type/data type in <>/name of array

	  ```vector
	  vector <int> my_vector;
	  ```

## **Introduction to Programming Concepts, Part 2**

### **What are functions?**

- Consequence of modular programming software development methodology
	- Multiple modular components
- Structured, stand-alone, reusable code that performs a single specific action
- Some languages refer to them as **subroutines, procedures, methods, or modules**

#### How functions work
  
  1. Functions take in data as input
  2. Then process the data
  3. Then return the result as output

#### Types of functions

- Standard library functions – built-in functions
	- if, else, while, print
- User-defined functions – you write yourself
	- Once a function is written, you can use it over and over
- Blocks of code in a function are identified in different ways
	- Use {}
	- Use begin-end statements
	- Use indentations

#### Using function
  
1. Define a function (create)
  - Function keyword, unique name, statements
1. Call a function (invoke)
  - Specified actions are performed using supplied parameters
2. Declare a function (some programming languages)
  - C, C++

### What are objects?

- Objects are key to understanding object-oriented programming (OOP)
- OOP is a programming methodology focused on objects rather than functions
- Objects contain data in the form of properties (attributes) and code in the form of procedures (methods)
- OOP packages methods with data structures
	- Objects operate on their own data structure

	![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-17.webp)

Objects in programming
- Consist of states (properties) and behaviors (methods)

  ![Basics of Programming](/notes/ibm-it-support/Basics%20of%20Programming-18.webp)

- Store properties in field (variables)
- Expose their behaviors through methods (functions)
