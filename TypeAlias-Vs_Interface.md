Type Aliases:

A type alias allows one to create a new for an existing type. It is declared using the 'type' keyword and it acts like a variable. Type holds a type definition instead of a runtime value. Type alias can not be reopened to add new values once it is created.

Type Aliases can be used for primitives like string or objects or arrays.


Interface:

Interface is a  powerful syntactical contract which  defines the "shape" of an object It specifies what properties and methods an object or class must have, along with their types, without providing the actual implementation. Interfaces exist only at compile-time for type checking and vanish completely once compiled to JavaScript.


Interface is similar to Type Alias but it is only applicable to object type.


When Should we use Type Alias or Interface:


Type Alias is when one need to work with primitives, union types, tuples and complicated mapped types and when there is need of intersection.

Interface is mostly used for object structures and especially for object oriented design or libraries that requires declaration merging.
