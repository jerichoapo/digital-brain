---
{"dg-publish":true,"permalink":"/digital-brain/060-technical/060-2-python/append/"}
---

The `append()` function in Python is used to add an element at the end of a list. It modifies the original list by adding the specified item as a new element. Here's how it works:

Syntax:
```python
list_name.append(element)
```

- `list_name` is the name of the list to which you want to append the element.
- `element` is the value you want to add to the list.

Example:
```python
fruits = ["apple", "banana", "orange"]
fruits.append("grape")
print(fruits)
```

Output:
```
["apple", "banana", "orange", "grape"]
```

In the example above, we have a list called `fruits` initially containing three elements. We use the `append()` function to add the string `"grape"` to the end of the list. After the `append()` operation, the `fruits` list now contains four elements, including the newly added `"grape"`.

[[Digital Brain/060 Technical/060.2 Python/060.2 Python MOC\|060.2 Python MOC]]