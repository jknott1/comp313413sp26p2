# TODO: Non-Code Questions

## TestIterator
1. Also try with a `LinkedList` - does it make any difference?

The difference in data structure didn't affect the running of the tests. They all ran and stll passed as each stucture filled the same requirements

2. What happens if you use `list.remove(Integer.valueOf(77))`?

The program throws a "ConcurrentModificationException" error. A method can't iterate through a list without altering it or else it throws that error.

## TestList

1. Also try with a `LinkedList` - does it make any difference?

Same as Test Iterator (1)

2. What does this method do?

it removes the element at index 5

3. What does this one do?

This one removes the first instance of the specified value if it exists in the list.

## TestPerformance:

