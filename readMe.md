The purpose of this module is to teach about callbacks!

Read the instruction carefully below, each function has it specific requirement

NOTE: run npm i

In the terminal run npm run test

filter - Return all elements of an array that pass a truth test.

reject - Return all elements of an array that don't pass a truth test.

uniq - Produce a duplicate-free version of the array.

map - Return the results of applying an iterator to each element.

reduce - Reduces an array or object to a single value by repetitively calling
iterator(accumulator, item) for each item. accumulator should be
the return value of the previous iterator call.

You can pass in a starting value for the accumulator as the third argument
to reduce. If no starting value is passed, the first element is used as
the accumulator, and is never passed to the iterator. In other words, in
the case where a starting value is not passed, the iterator is not invoked
until the second element, with the first element as its second argument.

Example:
var numbers = [1,2,3];
var sum = reduce(numbers, function(total, number){
return total + number;
}, 0); // should be 6

    var identity = reduce([5], function(total, number){
      return total + number * number;
    }); // should be 5, regardless of the iterator function passed in
           No accumulator is given so the first element is used.
