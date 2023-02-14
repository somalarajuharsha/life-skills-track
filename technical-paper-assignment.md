<!-- title -->
# **Basic Data Types and Data Structures with code samples in JAVASCRIPT**

## **JavaScript Data Types :**

 Every Variable has a data type that tells what kind of data is being stored in a variable.

 There are two types of data types in JavaScript namely Primitive data types and Non-primitive data types.

### **Primitive Data Types :**

 In JavaScript, a primitive value, primitive data type is data that is not an object and has no methods or properties.

 primitive data type values are immutable value because there is no way to change a primitive value once it gets created.

1. Boolean
2. Number
3. Bigint
4. String
5. Undefined
6. Null
7. Symbol

#### **boolean**

boolean represents boolean value either false or true.
Booleans can only have two values : true or false.
we can assign boolean values: 0 or 1 (0 = false and 1 = true).

three types of opertators used in boolean

==  equal to

\>  greater than

<  less than

* **example** :

    let value = true;

    let firstNum = 100;
    let secondNum = 100;
    let thirdNum = 250;

    console.log(firstNum == secondNum);     // Returns true
    console.log(firstNum == thirdNum);       // Returns false

#### **Number**

JavaScript has only one type of number.

Numbers can be written with or without decimals.

All JavaScript numbers are stored as decimal numbers i.e; floating point.

Unlike many other programming languages, JavaScript does not define different types of numbers like integers, short, long, double, float etc.

##### **opertators used in numbers**

\+ Addition

\- Subtraction

\* Multiplication

\/ Division

\% Modulus

\+\+ Increment

\-\- Decrement

* example :

    let num1 = 100.14;    // A number with decimals
    let num2 = 400;       // A number without decimals
    let num2 = 7_00_000;   // we can  separate numbers using '_'

    Extra large or extra small numbers can be written with scientific (exponent) notation:

    let value1 = 983e4;    // 9830000
    let value2 = 983e-4;   // 0.0983

    const number1 = 3/0;
    console.log(number1); // Infinity

    // strings can't be divided by numbers
    const number2 = "abc"/3;
    console.log(number3);  // NaN

#### **bigint**
  
JavaScript BigInt variables are used to store big integer values or large number values that are too big to be represented by a normal JavaScript Number.

To create a BigInt, append n to the end of an integer

A BigInt can not have decimals.

Operators that can be used on a JavaScript Number can also be used on a BigInt.

* example :

    let num1 = 9999999999999999n;
    let num2 = BigInt(999999999999999);  //explicitly typing
    console.log(num1+9);   //error = can't mix bigint and other type
    console.log(num1+9n);  //99999999999999999n

#### **String**

String is a set of characters or represents sequence of characters in a programming language.

we can use single or double quotes to write a string in javascript.

we can also use quotes inside a string and double quotes in string without keeping them matched.

we represent backslash (\) escape character to turn special character into string character.

* example :

    let text1 = "somalaraju harsha";  
    let text2 = 'using single quotes';  
    let line1 = "It's a pretty good day";  
    let text = "i am very much excited to become \"software developer\".";

    console.log("Text1 is " + text1); //somalaraju harsha
    console.log("Text2 is " + text2); //using single quotes
    console.log("Line1 is " + line1); //i am very much excited to become "software developer".

#### **Undefined**

undefined represents 'value is not assigned’.

A variable in JavaScript that is without any value defined has a value of undefined.

The datatype of a variable that holds an undefined value is also 'undefined'.

The purpose of an undefined datatype is to denote an absence of a meaningful value.

typeof undefined is undefined

* example :

let value;   // its value is 'undefined' and type is 'undefined'
let num = 100;
num = undefined;   // its value is now 'undefined' and type is 'undefined'
console.log(num);   //undefined

#### **null**

This data type can hold only one possible value that is null.

It denote something that does not exist.

You can empty a variable that holds any data by setting it to null without changing the datatype.

type of null is object

* example :

    let value = null;
    console.log("Value is " +value);   //value is null

#### **Difference between undefined and null :**

Although undefined and null are both valid values in JavaScript, for most practical purposes, they denote empty values and carry no information.

JavaScript treats both of these values as equivalent to each other but treats their datatypes as different, which is demonstrated below.

null == undefined                    // Evaluates to true

#### **Symbol**

Symbol is a built-in object.

To create a new primitive Symbol, we write Symbol() with an optional string.

It refers to the ‘key’ of the key-value pair of an object.

const vehicle1 = Symbol();

const vehicle2 = Symbol("car");

const vehicle3 = Symbol("car");

This code will creates three new Symbols.

### **Non-primitive data types:**

In javascript data types that are derived from primitive data types of the JavaScript language are known as non-primitive data types.
It is also known as derived data types or reference data types.
Non-primitive data types are mutable values because we can change the value after creation.

#### **Object:**

Object in Javascript is having properties and methods.
Everything is an object in javascript.

ways to create an object in javascript:

let gen = new Object();  //generic way object

let mycar = new Car();   //user defined object

let empty = {};          // literal notation way empty object

let square = { length : 40,  height : 40,  'total area' : 80
};                   // key : value pair

console.log(square);             //{ length : 40, height : 40, 'total area' : 80 }

console.log(square.length);      //40

console.log(square.height);      //40

console.log(square['total area']);  //80

#### **Array:**

An array is a special variable, which can hold more than one value.

An array in JavaScript is an object data type. Thus it holds its value in a key-value pair.

An array can hold many values under a single name, and we can access the values by referring to an index number.

We can have objects in an Array.

we can have functions in an Array.

we can have arrays in an Array

const items = [item1, item2, ...];  //creating an array

const fruits = ["Banana", "Orange", "Apple", "Mango"];

## **JavaScript Data Structures :**
  
Data Structure is the way of storing and organizing the data in such a way that it can be used efficiently.

To efficiently manage that data, we need data structures.

Data structures helps to solve problems in a more efficient way, both in terms of time and memory

1. Stack
1. Queue
1. Linked List
1. Set
1. Hash Table
1. Tree
1. Trie
1. Graph

### **stack**

Stack follows the principle of LIFO (last In, first out).

#### **COMMON METHODS OF STACK IN JAVASCRIPT**

push: Input a new element.

pop : Remove the top element, return the removed element.

peek : Return the top element.

length : Return the number of element(s) in the stack.

#### **Queue**

Queue is similar to stack. The only difference is that queue uses the FIFO principle (first in, first out).

##### **QUEUE METHODS IN JAVASCRIPT**

enqueue: Enter queue, add an element at the end.

dequeue: Leave queue, remove the front element and return it.

front: Get the first element.

isEmpty: Determine whether the queue is empty.

size: Get the number of element(s) in queue.

* PRIORITY QUEUE

    Queue has another advanced version. Allocate each element by priority and it will be sorted according to the priority level:

#### **Linked List**

A linked list is a chained data structure.

Each node consists of two pieces of information.

The data consists of the node and the pointer to the next node.

Linked List is a linear data structures with serialized storage.

##### **LINKED LIST METHODS**

size: Return the number of node(s).

head: Return the element of the head.

add: Add another node in the tail.

remove: Remove a certain node.

indexOf: Return the index of a node.

elementAt: Return the node of an index.

addAt: Insert a node at a specific index.

removeAt: Delete a node at a specific index.

#### **Set**

Set is a collection of distinct objects that are well-defined, and it allow to add data to a container.

A set does not allow repeating elements and is not indexed.

##### **SET METHODS IN JAVASCRIPT**

values: Return all elements in a set.

size: Return the number of elements.

has: Determine whether an element exists.

add: Insert elements into a set.

remove: Delete elements from a set.

union: Return the intersection of two sets.

difference: Return the difference of two sets.

subset: Determine whether a certain set is a subset of another set.

#### **Hash Table**

A hash table is a key-value data structure.

A hash represents the value of the corresponding key.

A hash points to a smaller subgroup of the table, which is called a storage bucket.

The storage bucket is then searched for the key that was originally entered.

It then returns the values associated with the key.

HASH TABLE METHODS IN JAVASCRIPT

add: Add a key-value pair.

remove: Delete a key-value pair.

lookup: Find a corresponding value using a key.

#### **Tree**

Tree data structure is a non-linear multi-layer data structure in contrast to array, stack and queue.

This structure is highly efficient during insert and search operations.

It proves to be highly efficient for several operations, such as insert and search.

A tree has a root node, and other nodes branch from this root node, a root node has various child nodes, which have references to all the elements And then there are more child nodes branching off from child nodes, and this continues.

**TREE DATA STRUCTURE EXPLANATION :**

root: Root node of a tree; no parent node for root

parent node: Direct node of the upper layer; only has one

child node: Direct node(s) of the lower layer; can have multiple

siblings: Share the same parent node

leaf: Node with no child

Edge: Branch or link between nodes

Path: The edges from a starting node to the target node

Height of Node: Number of edges of the longest path of a specific node to leaf node

Height of Tree: Number of edges of the longest path of the root node to the leaf node

Depth of Node: Number of edges from root node to specific node

Degree of Node: Number of child nodes

#### **Trie**

Trie is also a type of search tree.

Trie stores the data step-by-step each node in the tree represents a step.

The steps in the tree are represented by nodes.

##### **METHODS OF TRIE IN JAVASCRIPT**

add: Insert a word into the dictionary tree.

isWord: Determine whether the tree consists of a certain word.

print: Return all words in the tree.

#### **Graph**

Graphs can be represented in two ways. One is called the adjacent list, wherein the left side consists of all the nodes and the right side consists of the connected nodes.

There are graphs divide into two groups directed graphs and undirected graphs.

* _**Reference Links :**_

    [w3schools](https://www.w3schools.com/js/)

    [free code camp](https://www.freecodecamp.org/news/what-is-javascript/)

    [telusko javascript](https://www.youtube.com/watch?v=PlbupGCBV6w&list=PLsyeobzWxl7rrvgG7MLNIMSTzVCDZZcT4)

    [moshhamadani javascript](https://www.youtube.com/watch?v=W6NZfCO5SIk)
