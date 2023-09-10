# Functions

## Function Declarations vs Expressions
![Alt text](../Images/image-66.png)

## Hoisting
Hoisting is when Js engine execute the Function Declaration code, it will move the Function Declaration to top, eventhough we call the function before it is defined. That cannot be done in Function Expression

![Alt text](../Images/image-67.png)

## Arguments
use arguments object.This is useful when we want to use a varying number of paremeters in a function.

![Alt text](../Images/image-68.png)


## The Rest Operator
use ...args

when we apply the rest operator to a parameter of a function, we can pass varying number of arguments and the rest operator will take all of them and put them in an array.

![Alt text](../Images/image-69.png)

Calculating discount in item cart
![Alt text](../Images/image-70.png)

rest ...args must be last formal parameter.

## Default Parameter
![Alt text](../Images/image-71.png)

So we want to have a default value for rate, and years. We can achieve thar using logical OR.

![Alt text](../Images/image-72.png)

This is a newer way to achieve the same thing introduced in ES6

![Alt text](../Images/image-73.png)

we can pass the value in the parameter,but make sure that it is placed last,or each parameter after that should be initialized to a value as well.

## Getter and Setters
![Alt text](../Images/image-74.png)

We want to code once, and call that function multiple times in other places. But the way above is read only and we cant change outside of the code block.

![Alt text](../Images/image-75.png)

## Try and Catch
Error handling - defensive programming
use throw keyword
we throw the error and catch that error. 

```
const person = {
    firstName: 'Mohd',
    lastName: 'Syakir',
    set fullName(value) {
        if (typeof value !== 'string')
            throw new Error('Value is not a string.');

        const parts = value.split(' ');
        if (parts.length !== 2)
            throw new Error('Enter a first and last name.');

        this.firstName = parts[0];
        this.lastName = parts[1];
    }
}

try {
    person.fullName = '';
}

catch (e) {
    alert(e);
}

console.log(person);
```

## Local Vs Global Scope
avoid define global constant or variables

## Let Vs Var
The issue with the var keyword is that when we declare a variable with var, the scope is not limited to the code block which is it's defined but limited to the function that it's defined.

var => function-scoped
ES6 (ES2015): let, const => block-scoped

![Alt text](../Images/image-76.png)

when var is initialized globally, it will be attached to the global window. 

same as the function sayHi() {} in the image. 

