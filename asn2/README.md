Assignment 2
============

1. Write a method that reverses a [`std::string`](http://en.cppreference.com/w/cpp/string/basic_string). With and without iterators.
2. Write a method that does an operation on each element of a container, like [`std::vector`](http://en.cppreference.com/w/cpp/container/vector). Could be lower/upper casing or replacing the value, but solve using a functor, a function pointer and a lambda.
3. Write a template method for converting something (`typename T`) into an `std::string`. Make template specializations for the different types you want to support to convert into `std::string`. But at least include `bool`, `int` and `float`. Use [`std::assert()`](http://en.cppreference.com/w/cpp/error/assert) when no specialization can be used.
4. Finally, do a similar approach using [`std::ostringstream`](http://en.cppreference.com/w/cpp/io/basic_ostringstream).