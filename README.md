# Unexpected Behavior with Direct Attribute Assignment in Ruby

This repository demonstrates a subtle but common error in Ruby related to assigning values to attributes directly without explicitly defining a setter method.  In Ruby, unlike some other languages, simply assigning a value to an attribute outside of a defined method does not modify the object's internal state. 

The `bug.rb` file shows how this can lead to unexpected behavior. The `bugSolution.rb` file provides the correct way to handle attribute assignment.

## How to reproduce the bug:

1. Clone this repository.
2. Run `ruby bug.rb`.
3. Observe that the value does not update as expected.

## How to solve the bug:

Refer to `bugSolution.rb` for the solution.  The key is to either define a setter method (`value=`) or use instance variables consistently within defined methods.