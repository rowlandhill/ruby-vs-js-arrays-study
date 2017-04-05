# Ruby vs. JavaScript: Arrays Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

## Required Readings

-   [Ruby](https://github.com/ga-wdi-boston/ruby)
-   [Ruby Arrays](https://github.com/ga-wdi-boston/ruby-arrays)
-   [JavaScript Reference Types](https://github.com/ga-wdi-boston/js-reference-types)
-   [JavaScript Array Methods](https://github.com/ga-wdi-boston/js-array-methods)

## Array#push vs. Array.prototype.push()

What are the similarities and differences between Ruby's and JavaScript's `push`
Array methods?

Similarities:

```md
Both Ruby's and JavaScript's push array methods add an element to the end of
an array.
```

Differences:

```md
Ruby's push array method returns the modified array, allowing method chaining.

JavaScript's push array method returns the length of modified array.
```

## Array#pop vs. Array.prototype.pop()

What are the similarities and differences between Ruby's and JavaScript's `pop`
Array methods?

Similarities:

```md
Both Ruby's and JavaScript's pop array methods remove an element at the end of
an array and return nil and undefined, respectively, if the array is empty.
```

Differences:

```md
Ruby's pop array method accepts a number, n, as an argument that removes the
last n elements (or less) of the array and returns them.

JavaScript's pop array method doesn't accept any arguments.
```

## Array#shift vs. Array.prototype.shift()

What are the similarities and differences between Ruby's and JavaScript's
`shift` Array methods?

Similarities:

```md
Both Ruby's and JavaScript's shift array methods remove the first element of an
array and return nil and undefined, respectively, if the array is empty.
```

Differences:

```md
Ruby's shift array method accepts a number, n, as an argument that removes the
first n elements (or less) of the array and returns them.

JavaScript's shift array method doesn't accept any arguments.
```

## Array#unshift vs. Array.prototype.unshift()

What are the similarities and differences between Ruby's and JavaScript's
`unshift` Array methods?

Similarities:

```md
Both Ruby's and JavaScript's unshift array methods add elements to the beginning
of an array.
```

Differences:

```md
Ruby's unshift array method returns the modified array, allowing method
chaining.

JavaScript's unshift array method returns the length of the modified array.
```

## Array#map vs. Array.prototype.map()

Using Ruby's and JavaScript's `map` Array methods, create a new array consisting
of the squares of the existing array.

Ruby:

```ruby
array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

squares = array.map { |number| number ** 2 }
```

JavaScript:

```javascript
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

const squares = array.map(number => number ** 2);
```

## Array#reduce vs. Array.prototype.reduce()

Using Ruby's and JavaScript's `reduce` Array methods, find the product of the
numbers in the given array.

Ruby:

```ruby
array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

product = array.reduce(1) { |accumulator, number| accumulator * number }
```

JavaScript:

```javascript
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

const product = array.reduce((accumulator, number) => accumulator * number, 1);
```

## Array#select vs. Array.protoype.filter()

Using Ruby's `select` Array method and JavaScript's `filter` method, create a
new array consisting of the odd numbers of the existing array.

Ruby:

```ruby
array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

odds = array.select { |number| number.odd? }
```

JavaScript:

```javascript
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

const odds = array.filter(number => number % 2 === 1);
```
