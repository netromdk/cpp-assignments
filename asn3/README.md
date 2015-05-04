Assignment 3
============

1. Implement a very simple tree node class where each node has a value (let’s say an integer value) and optionally children (sub nodes).
 1. Construct a simple tree using your class (not too tall) and write a recursive method to write all values (from each node) to stdout. Choose a different value for each node when you create the tree so that you can see the order they are visited.
 2. Write a recursive method that dumps the tree into a string format to visualize it.
Write a recursive method that calculates the sum of all numbers in the tree. Then do the same using a non-recursive method and see the difference to accomplish the same result. What is it and why do you like your recursive solution better? If not, why?
 3. What’s the height of the tree (the amount of levels)? Write a method for calculating it. Keep in mind that the tree can be uneven. If you know that each node can only have a certain amount of children can you say from that what the height of the tree is? Imagine that each node can only have two children at max. If there are 8 leaves how tall is the tree?
2. Implement Visitor pattern on the tree assignment. Create an abstract interface to define a NodeVisitor.
 1. Make a visitor that prints the tree. Try to visualize the tree levels, like indentation level.
 2. Make a visitor that counts the sum of the tree.
 3. Make a visitor that calculates the height of the tree.