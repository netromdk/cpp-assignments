Assignment 4
============

1. Write your own templated class called Vector that should work similar to an `std::vector`. Think about how you will store and manage the data elements internally. In the end try to compare your Vector to `std::vector`. Implement at least the following:
 1. Constructors:
    1. No arguments which makes an empty Vector.
    2. `(size, value)` which creates a Vector of that size and with each value being that value.
    3. **Optional:** (input iterator first, input iterator last) to create a Vector with the values from “first” to “last” from the other container.
 2. `isEmpty()` - checking if it’s empty or not.
 3. `size()` - the number of elements in the Vector.
 4. `capacity()` - the capacity of the Vector, which means the number of elements it can hold before the internal size needs to be made larger.
 5. `clear()` - remove all elements and free the memory used.
 6. `T operator[](int)` - access element at position and return copy.
 7. `const T &operator[](int)` - access element at position and return const reference of the element.
 8. `append(T)` - append an element at the end to the Vector.
 9. **Optional:** `prepend(T)` - insert an element at the beginning of the Vector.
 10. **Optional:** `insert(int, T)` - insert an element at a specific position of the Vector.
 11. `remove(T)` - Remove all elements equal to the argument.
 12. `removeAt(int)` - remove element at position.
 13. **Optional:** `shrinkToFit()` - make capacity == size but you cannot remove any elements or modify them, however reallocation is allowed.
 14. Try out your new Vector class:
    1. Test Vector<int> with 500,000,000 elements. Verify your methods work as you expect. Also try std::vector<int> with the same 500,000,000 elements, is it faster/more efficient? Why?
    2. Test Vector<int>. Add 10000 elements, remove 4000, check size/capacity, add 8000, check size/capacity, remove 10000. Now see what the capacity is? Might be a good idea to implement shrinkToFit() and revisit how you allocate and control your capacity.