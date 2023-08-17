### Auto-boxing

Auto-boxing in JavaScript refers to the automatic conversion of primitive data types into their corresponding wrapper objects when necessary. In JavaScript, primitive data types include numbers, strings, booleans, symbols, null, and undefined. Wrapper objects are objects that encapsulate these primitive values and provide additional methods and properties.

Auto-boxing is a feature that allows you to treat primitive values as objects temporarily by accessing their methods and properties. When you attempt to call a method on a primitive value, JavaScript automatically converts the primitive value into a temporary wrapper object, allowing you to use the method. Once the operation is complete, the wrapper object is discarded.

Here's an example to illustrate auto-boxing:

```javascript
let num = 42;

// Using a method on a primitive number
let result = num.toString(); // Auto-boxing occurs here

console.log(result); // Output: "42"
```

In the example above, `num` is a primitive number, and we use the `toString()` method on it. JavaScript auto-boxes the primitive number into a temporary Number object, allowing us to use the `toString()` method. After the method call, the temporary object is discarded.

Auto-boxing is a convenient feature that allows you to work with methods and properties on primitive values as if they were objects. However, it's important to note that auto-boxing can introduce a small performance overhead, especially in cases where the same operation is performed repeatedly. In such cases, it's often more efficient to explicitly create wrapper objects if you need to access their methods multiple times.