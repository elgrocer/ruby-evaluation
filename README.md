# elGrocer Evaluation - Block implementation

## Goal

Your task is to **complete the implementation of the `Block` class** (`block.rb`) so that the specs (`block_spec.rb`) run green.

`Block` provides an abstraction for performing boolean operations on a numerical range. It is used for calculating the interaction of free and busy time periods on a schedule.

 A `Block` is a __Value Object__ which has a starting value (called `top` or `start`) and an ending value
 (called `bottom` or `end`). These properties are numeric values which could
 represent points in time, or an arbitrary numeric scale.

 `Block`s can be combined and subtracted from one another to yield other blocks
 or arrays of blocks depending on whether the original blocks are contiguous or not.

 For example:

 ```
   # Addition of overlapping ranges:
   Block.new(3, 8) + Block.new(5, 12) == Block.new(3, 12)

   # Subtraction of one block from the middle of another:
   Block.new(5, 25) - Block.new(10, 20) == [Block.new(5, 10), Block.new(20, 25)]
```

The specs are provided, but the implementation is incomplete. Implement the remaining methods on `Block` so that all the tests pass. Try to make your solution as elegant and readable as possible.

Good luck!

## Installation

```
bundle install
rspec spec
```

## Instructions
1. Clone this repo and push the solution along with the code on your personal repo and send us the link of that repo.
2. Questions will not be entertained except those related to code setup.
3. Check out a new branch to do your work.
4. Run `rspec spec/block_spec.rb` to view the specs for the `Block` class.
5. Fill in the missing method implementations for the `Block` class to make all the specs run green. Do not change the spec files.
6. Try to refactor your solution to remove any obvious code smells. Don't worry about making it perfect. First make your code correct, and then refactor to the extent necessary that your solution is clear and maintainable. Manage your time wisely and stop when its good enough.
7. Your commits should be elaborative and self explanatory to describe the changes.
8. Please commit your changes to your working branch frequently so I can get a sense of your development process.
9. Your solution would be rejected if it does not have frequent commits. The commit messages should be brief and self-explanatory.

## Hints

1. You will find it helpful to make use of the existing query methods that have already been implemented for you.

## Assessment

I will evaluate your solution based on:

1. Correctness (does it satisfy the test cases?)
2. Elegance (is the solution clean, clear and well factored?)
3. Process (did you take a systematic approach to solving the problem?)
