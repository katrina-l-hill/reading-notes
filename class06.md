# Class 06 – JS Object Literals; The DOM

## Reading Overview 05

### Understanding the Problem Domain is the Hardest Part of Programming

- The author believes that the hardest part of learning to code is figuring out what all the information needed to identify a problem, i.e., the problem domain.
- He continued to use his protein tracker application to teach his courses because it was a coding problem that was already solved and didn’t need any further modifications.
- In addition, he found that the application was something that he could easily teach, and it was well understood by students.
- Writing code is like putting together a jigsaw puzzle. In order to put together a puzzle, you group the pieces together into manageable groups such as, the major components, color, and border pieces.
- When you have a difficult puzzle where you can’t put the pieces into manageable groups, you can’t see the big picture of the puzzle, or the problem domain.
- Understanding the problem domain is essential to writing code. You need have a good understanding of what the problem is and what you need to do to solve it in order to write the appropriate code.
- In order to understand the problem domain and make programing easier, you need to: “make the problem domain easier,” and “get better at understanding the problem.”

### What’s the Difference between Primitive Values and Object References in JavaScript?

- Data types in JavaScript fall into one of two categories: primitive values and object references.
- In order to understand JavaScript, you must fully understand the difference between primitive values and object references.
- There are 8 different data types in JavaScript: Boolean, null, undefined, number, BigInt, string, symbol, and objects.
- Objects in JavaScript include arrays, functions, and dates.
- One difference between primitive values and object references is primitive values contain values, while object references contain reference to objects.
- Another difference between primitive values and object references is mutability, where primitive values are immutable (i.e., cannot be changed) and object references are mutable (i.e., can be changed).
- The loose equality (==) operator returns true if the values of two item being compared are the same.
- The strict equality (===) operator will return true if the values and the types of the two objects being compared are the same.
- The computer’s memory address sees objects on both sides of the strict equality sign (===) as being different.
- In order to check whether the contents, not the reference, of two objects are the same you need to either: 1. Iterate through the object and check that each key and value match. (This can be tricky because an object’s property can be an object in itself.); 2. Convert the object to a suitable primitive before doing the equality check.
- When possible, it’s recommended to use the strict equality operator versus the loose equality operator to avoid unexpected code behavior.

### JavaScript book

#### Object Literals

- Objects group together a set of variables and functions to create a model of something recognizable in in the real world.
- In an object, variables become known as properties. If a variable is part of an object, it’s called a property.
- Properties tell us about the object. For example, the name of a hotel or the number of rooms the hotel has.
- Each hotel has its own name and its own number of rooms.
- In an object, functions become known as methods. If a function is part of an object, it’s called a method.
- Methods represent tasks that are associated with the object. For example, finding the number of available rooms be subtracting the number of booked rooms from the total number of rooms in the hotel.
- In an object, properties and methods have a name and value, called a key.
- An object cannot have two keys with the same name because keys are used to access their corresponding values.  
- The value of a property can be a string, Boolean, number, array, or be another object.

#### Document Object Model

- The Document Object Model (DOM) is an interface that identifies how HTML content is displayed and how JavaScript accesses and updates the web pages contents.
- The DOM cover two primary areas: making a model of the HTML page and accessing and changing the HTML page.
- The DOM is called an object model because the DOM tree (model) is made of objects.
- The DOM tree is a model of a web page.
- Each node is an object with methods and properties.
- Every node is a descendent of the document node.
- Any changes made to the DOM tree are reflected in the browse.
- Accessing and updating the DOM tree can be done in two steps: locate the node that represents the element you want, and use its context, child elements, and attributes.
