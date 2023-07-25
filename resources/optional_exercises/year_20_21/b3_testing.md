# Block 3 - Testing optional exercise

In this exercise, we are going to implement some tests on the *HomeAutomation* project implemented in block 2 (not the JavaFX version).

> **IMPORTANT NOTE**: you MUST use the classes from the solution provided by us, instead of your own classes.

We are going to focus only on `Blind` class. Regarding this class inside the original project, you are asked to:

* Define a document (PDF or ODT format) with the test for `raise(int percent)` and `lower(int percent)` methods. Think about all the different situations in which a blind can be with these methods, and try to make sure that they act as expected with these test cases. For each test case, you must prove an identifier, name, preconditions, input data and expected result.
* Create a test class called `BlindTest` inside `test` source folder (you have to create this new source folder in the original project). This test class must have test methods for EVERY method inside `Blind` class, including the constructor and the `toString` methods. In the test methods for `raise(int percent)` and `lower(int percent)` you must apply the test cases defined in the document explained above. In the rest of test methods, you just need to test them with a simple test case. For instance, regarding `raise()` method, you can just create a new blind and try to raise it completely, and then check if the final percent is 100.

## What to deliver?

You must deliver a ZIP/RAR file containing the *HomeAutomation* project modified with the `test` source folder and the `BlindTest` test class. Also, this file must contain the PDF/ODT document with the test cases specified for `raise(int percent)` and `lower(int percent)` methods.

## Evaluation criteria

This exercise will be evaluated as follows:

* Test case table for `raise(int percent)` and `lower(int percent)` methods: 2 points (1 point each)
* Test methods inside `BlindTest` class will be evaluated as follows:
  * Test methods for constructor, `toString`, `getPercent()`, `raise()` and `lower()` methods: 1 point each
  * Test methods for `raise(int percent)` and `lower(int percent)` methods: 1,5 points each
