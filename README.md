# Sleeping Duck Tech Test

## Introduction
This is a code challenge I completed for Sleeping Duck as part of the application process.

All changes can be found in the file `after.html`.

Please see dev-log.md and my Trello board for details on how I worked through this code challenge and broke down the tasks.

## Questions

### Part 1
1. Passing a function allows access to the current state. In this case, we're accessing current items, then looping through them, only changing the value of complete once the condition is met.

2. Mapping over the array preserves immutability as well as creating a copy of the original items array to ensure that no unexpected behaviour occurs with `state.items`.

    The spread function is used to obtain all previous properties, i.e. `title, id, selected`. We can then update any properties that need to change by specifying them afterward.

### Part 2
1. If items are being added, moved or removed in an array, the index will change and refer to a different item in the array. It is best to have unique, permanent ids to avoid this issue, and can be done easily by adding it as a property to the item.

    I did this by prepending a string to the index (i.e. `id: item-${i}`).
