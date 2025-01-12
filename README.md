# Ruby Getter Method Limitation

This example demonstrates a common pitfall in Ruby when working with getter methods.  If you only define a getter method (e.g., `value`) without a corresponding setter method (e.g., `value=`), attempting to assign a new value through the getter will not modify the instance variable's value.  The assignment occurs within the method's scope as a new local variable.

**To fix this, you need to define both getter and setter methods if you want to allow external modification of the instance variable.**