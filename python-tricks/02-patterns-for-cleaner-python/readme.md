Assert

```python
def apply_discount(product, discount):
    price = int(product['price'] * (1.0 - discount))
    assert 0 <= price <= product['price']
    return price
```

```python
shoes = {'name': 'Fancy Shoes', 'price': 14900}
apply_discount(shoes, 1.25)
```

Output if following

```python
Traceback (most recent call last):
  File "/Users/yauheni.sarokin/PycharmProjects/notes/python-tricks/02-patterns-for-cleaner-python/example-01.py", line 9, in <module>
    apply_discount(shoes, 1.25)
  File "/Users/yauheni.sarokin/PycharmProjects/notes/python-tricks/02-patterns-for-cleaner-python/example-01.py", line 3, in apply_discount
    assert 0 <= price <= product['price']
AssertionError

```
