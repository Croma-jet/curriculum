# Pretty print data structures
author: catalin

levels:

  - basic

  - advanced

  - medium

type: normal

category: feature

notes: ''

links:

  - '[pymotw.com](https://pymotw.com/2/pprint/){website}'

---
## Content

**Python** provides a way of generating eye pleasing representations of data structures when printing by using the `pprint` module.

Import the module:
```python
import pprint
```

You can use the `pprint()` function to print your data structure.
```python
# data = our data structure
pprint.pprint(data)

```

The module also provides a way of formatting data structures into strings for other purposes (e.g. logging):
```python
data = [(x, {y: y * y for y in range(2)})
        for x in range(4)]
print(pprint.pformat(data, width=19))

```
Instead of a single line our output will be:
```python
[(0, {0: 0, 1: 1}),
 (1, {0: 0, 1: 1}),
 (2, {0: 0, 1: 1}),
 (3, {0: 0, 1: 1})]

```

You can even check if an object is **readable**:
```python
print(pprint.isreadable(data))
# True
```

In addition, a `PrettyPrinter` object can be created.

---
## Revision

What library provides pretty printing of data structures in *Python*? ???

* `pprint`
* `draw`
* `superdraw`