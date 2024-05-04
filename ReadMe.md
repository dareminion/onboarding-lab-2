# Week 2 Lab: System Verilog

## Make Note

Three different testing approaches

* Exhaustive
    * For smaller components this is easier to implement as there are not as many values to test through
    * Can be a time consuming test if the module has many different steps or a larger input. 
* Inital values
    * For larger registers, this is better than exhaustively testing because the amount of values would increase the testing time
    * The test would have to incorporate a reasonable set of test values over the range the module uses for inputs to ensure the module is working correctly
    * Could potentially miss one or two values that end up producing an error
* Random Values
    * Similar advantages as with the previous approach
    * Random values over many cycles slowly means there is more coverage than just using some set of values
    * Could still miss a critical functioning point alongside edge cases that may not be covered

These different test can be used in combination or standalone depening on the module that we are trying test. Most likely a combination of these tests would be able to test for the majority of inputs without having to exhaustively go through every bit.

