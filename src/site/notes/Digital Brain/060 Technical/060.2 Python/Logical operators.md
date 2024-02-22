---
{"dg-publish":true,"permalink":"/digital-brain/060-technical/060-2-python/logical-operators/"}
---

In Python, logical operators are used to combine conditional statements. There are three logical operators: `and`, `or`, and `not`.

The `and` operator returns `True` if both operands are `True`, and `False` otherwise. For example:

```
x = 5
y = 10
if x > 0 and y < 20:
    print("Both conditions are True.")
```

In this example, the `and` operator combines two conditional statements (`x > 0` and `y < 20`). Since both conditions are `True`, the `print` statement will be executed.

The `or` operator returns `True` if at least one operand is `True`, and `False` otherwise. For example:

```
x = 5
y = 10
if x < 0 or y > 20:
    print("At least one condition is True.")
```

In this example, the `or` operator combines two conditional statements (`x < 0` and `y > 20`). Since the second condition is `True`, the `print` statement will be executed.

The `not` operator is used to negate a conditional statement. It returns `True` if the statement is `False`, and `False` if the statement is `True`. For example:

```
x = 5
if not x > 10:
    print("x is not greater than 10.")
```

In this example, the `not` operator negates the conditional statement `x > 10`. Since the statement is `False`, the `print` statement will be executed.

It's worth noting that logical operators have a specific order of precedence. `not` is evaluated first, followed by `and`, and finally `or`. However, it's always best to use parentheses to make the order of evaluation explicit and avoid potential confusion.

[[Digital Brain/060 Technical/060.2 Python/060.2 Python MOC\|060.2 Python MOC]]