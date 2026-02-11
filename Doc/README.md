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

### REPS = 100000

_LinkedList Add/Remove time_

| size | runtime (ms) |
|----|--------------|
| 1  | 14           |
| 10 | 12           |
| 100| 12           |
|1000| 14           |
|10000| 14           |
|100000| 17           |

_ArrayList Add/Remove time_

| size | runtime (ms) |
|----|--------------|
| 1  | 16           |
| 10 | 16           |
| 100| 24           |
|1000| 113          |
|10000| 1034         |
|100000| 13954        |

_LinkedList Access Time_

| size | runtime (ms) |
|----|--------------|
| 1  | 5            |
| 10 | 10           |
| 100| 16           |
|1000| 313          |
|10000| 4403         |
|100000| 42924        |

_LinkedList Access Time_

| size | runtime (ms) |
|----|--------------|
| 1  | 5            |
| 10 | 6            |
| 100| 6            |
|1000| 9            |
|10000| 7            |
|100000| 11           |

_Addition/Removal_

    For Adding/Removing items, LinkedLists show a near constant runtime. They take a constant number of steps
    to insert or delete any element from the list regardless of it's size (O(1)). However, an ArrayList has to refactor
    itself each time, scaling with the size of the elements rearranged (O(n)).

_Accessing_

    For accessing, however, ArrayLists are much faster. To access an element at a given index on a LinkedList, the program
    has to iterate through the list starting at the head up to the index, which scales with size (O(n)). However, ArrayLists
    keep track of the index of each element, so lookup can be done in one step (O(1)).
