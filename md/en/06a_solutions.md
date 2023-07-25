# Software testing

## Introduction to software testing - Exercise solutions

> **Exercise 1:** 
> 
> Design test cases to check the behavior of a function that returns a boolean indicating if the number specified as a parameter is even or not.

As we are not relying on any particular programming language, we must also take into account some additional invalid inputs, such as parameters that are not numbers. We could also check if the method deals with both positive and negative values. So a possible table for these test cases could be this one:

|ID|Name|Data|Expected result|
|---|---|---|---|----|
|U1|PositiveEven|number=2|true|
|U2|NegativeEven|number=-14|true|
|U3|ZeroEven|number=0|true|
|U4|PositiveOdd|number=3|false|
|U5|NegativeOdd|number=-27|false|
|U6|InvalidInputString|number="Hello"|Exception thrown|
|U7|InvalidInputFloat|number=3.14|Exception thrown|

We have omitted both columns *Preconditions* (since there's no particular precondition for any test case) and *Steps* (since user doesn't have to type anything). Besides, *Actual result* column has been omitted for simplicity (since it is going to be empty until we run this test).
