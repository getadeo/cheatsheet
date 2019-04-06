# String

## Indexing

```python
s = 'Genesis'
print(s[3])

# Output:
# 'e'
```

## Slicing
```python
s = 'computer'

print(s[1:4])
print(s[1:6:2])
print(s[3:])
print(s[:5])
print(s[-1])
print(s[-3])
print(s[:-2])

## Output:
# omp
# opt
# puter
# compu
# r
# t
# comput
```

## Adding/Concatenating


```python
s = 'uni' + 'corn'

print(s)

# Output:
# unicorn
```

## Multiplying

```python
s = 'jump' * 3

print(s)

# Output:
# jumpjumpjump
```

# Checking membership

```python
s = 'unicorn'

print('u' in s)
print('u' not in s)

# Output:
# True
# False
```

## length

```python
s = 'unicorn'

print(len(s))

# Output:
# 7
```

## minimum

```python

# Note: Can be Alpha or Numberic. But cannot be mixed.

s = 'unicorn'

print(min(s))

# Output:
# c 
```

# maximum

```python

# Note: Can be Alpha or Numberic. But cannot be mixed.

s = 'unicorn'

print(max(s))

# Output:
# u
```

## sort

```python
s = 'unicorn'

print(sorted(s))

# Output:
# ['c', 'i', 'n', 'n', 'o', 'r', 'u']
```

## count(item)

```python
s = 'elephant'

print(s.count('e'))

# Output:
# 2
```

## index(item)

```python
s = 'elephant'

print(s.index('e'))

# Output:
# 0
```

# f-strings

```python
name = "Genesis"
age = 26

print(f"Hello, I am {name} and I am {age} years old.")

# Output:
# Hello, I am Genesis and I am 26 years old.
```


# List

## Indexing
```python
l = ['adobo', 'sinigang', 'dinuguan']
print([l[1]])

## Output:
# ['sinigang']
```

## Adding/Concatenating

```python
l = ['dragons', 'elves'] + ['knights']

print(l)

# Output:
# ['dragons', 'elves', 'knights']

```

## Multiplying

```python
l = [3, 17] * 3

print(l)

# Output:
# [3, 17, 3, 17, 3, 17]
```

## Checking membership

```python
l = ['dragons', 'elves', 'knights']

print('dog' not in l)

# Output:
# True
```

## Iterating

```python
# Item
l = [3, 17, 2019]
for item in l:
    print(item * 2)

# Output:
# 6
# 34
# 4038

# Index & Item
l = [3, 17, 2019]
for index, item in enumerate(l):
    print(index, item)

# Output:
# 0 3
# 1 17
# 2 2019
```

## length

```python
l = ['elves', 'dragons', 'knights']

print(len(l))

# Output:
# 3
```

# minimum

```python

# Note: Can be Alpha or Numberic. But cannot be mixed.

l = ['elves', 'dragons', 'knights']

print(min(l))

# Output:
# dragons
```

# maximum

```python

# Note: Can be Alpha or Numberic. But cannot be mixed.

l = ['elves', 'dragons', 'knights']

print(max(l))

# Output:
# knights
```

# sum

```python
l = [2, 3, 17, 2019]

print(sum(l))
print(sum(l[-2:]))

# Output
# 2041
# 2036
```

# sort

```python

# Note:
# sorted(l) returns a new sorted list without changing the original list
# l.sort() puts the items of l in sorted order

l = ['elves', 'dragons', 'knights']

print(sorted(l))

l.sort()

print(l)

# Output:
# ['dragons', 'elves', 'knights']
# ['dragons', 'elves', 'knights']

```

## count(item)

```python
l = ['elves', 'dragon', 'knights', 'dragon']

print(l.count('dragon'))

# Output:
# 2

```

## index(item)

```python
l = ['elves', 'dragon', 'knights', 'dragon']

print(l.index('dragon'))

# Output:
# 1

```

## unpacking

```python

# Note: Number of varibales must exactly match the length of the list

l = ['elves', 'dragon', 'knights']

a, b, c = l

print(a)
print(b)
print(c)

# Output:
# elves
# dragon
# knights
```

## constructors

```python
l = list()
l = ['elves', 'dragon', 'knights']
l = list(<tuple>)
```

## List Comprehension

```python

l = [i for i in range(19)]

print(l)

# Output:
#  [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18]

l = [z**2 for z in range(10) if z > 4]

print(l)

# Output:
# [25, 36, 49, 64, 81]
```

## delete

```python

l = [1, 2, 3, 4, 5]

del(l[1])
print(l)

del(l)
print(l)

# Output:
# [1, 3, 4, 5]
# NameError: name 'l' is not defined

```

## append

```python
l = [1, 2, 3, 4, 5]
l.append(6)

print(l)

# Output:
# [1, 2, 3, 4, 5, 6]
```

## extend

```python
l = [1, 2, 3, 4, 5]
l2 = [6, 7, 8]

l.extend(l2)

print(l)

# Output:
# [1, 2, 3, 4, 5, 6, 7, 8]
```

## insert

```python
l = [1, 2, 3, 4, 5]
l.insert(6, 7)

print(l)

l.insert(1, ['G','J'])

print(l)

# Output:
# [1, 2, 3, 4, 5, 7]
# [1, ['G', 'J'], 2, 3, 4, 5, 7]

```

## pop

```python
l = [1, 2, 3, 4, 5]
l.pop()

print(l)

print(l.pop())

print(l)

# Output
# [1, 2, 3, 4]
# 4
# [1, 2, 3]
```

## remove
```python
l = [1, 2, 3, 4, 5]
l.remove(3)

print(l)

# Output:
# [1, 2, 4, 5]
```

## reverse

```python
l = [1, 2, 3, 4, 5]
l.reverse()

print(l)

# Output:
# [5, 4, 3, 2, 1]
```

# Tuples

* Support all operations for Sequences.
* Immutable, but member objects may be mutable.
* If the contents of a list should not change, use a tuple to prevent items from accidentaly being added, changed or deleted.
* Tuples are more efficient than lists due to Python's implementation.

## constructors

```python
t = ()              # no-item tuple
t = (1, 2, 3)
t = 1, 2, 3         # parenthesis are optional
t = 2,              # single-item tuple

l = [1, 2, 3, 4, 5]
l = tuple(l)        # tuple from list

```

## immutable

```python
t = (1, 2, 3)
del(t[1])           # error!

t[1] = 5            # error!

t = ([1, 2], 3)     # 2-item tuple: list and int
del(t[0][1])

print(t)

# Output:
# TypeError: 'tuple' object doesn't support item deletion
# TypeError: 'tuple' object does not support item assignment
# ([1], 3)
```

# Sets

## constructor


```python

st = {3, 5, 3, 5}   # {5, 3}
print(st)

st = set()          # empty set

l = [3, 5, 3, 5]
st = set(l)      # new set from the list
                    # strips duplicates
print(st)

# Output
# {3, 5}
# {3, 5}

# Set Comprehension:
st = {3*i for i in range(10) if i>5}

print(st)

# Output:
# {24, 18, 27, 21}
```

## basic set operations

| Description                  | Code                      |
|------------------------------|---------------------------|
| Add item to set st           | st.add(item)              |
| Remove item from set st      | st.remove(item)           |
| Get length of set st         | len(st)                   |
| Check membership in st       | item in st item not in st |
| Pop random item from set st  | st.pop()                  |
| Delete all items from set st | st.clear()                |


## standard mathematical set operations

| Set Function         | Description             | Code         |
|----------------------|-------------------------|--------------|
| Intersection         | AND                     | set1 $ set2  |
| Union                | OR                      | set1 \| set2  |
| Symmetric Difference | XOR                     | set1 ^ set2  |
| Difference           | In set1 but not in set2 | set1 - set2  |
| Subset               | sets2 contains set1     | set1 <= set2 |
| Superset             | set1 contains set2      | set1 >= set2 |


# Dictionary

## constructors

```python
d = {'name': 'Genesis', 'age': 26, 'hometown': 'Valenzuela'}

d = dict([('name', 'Genesis'), ('age', 26), ('hometown', 'valenzuela)])

d = dict(name='Genesis', age=26, hometown='Valenzuela')
```

## basic dict operations

| Description                                            | code                    |
|--------------------------------------------------------|-------------------------|
| Add or change item in dict d                           | d['name'] = 'Dominic'   |
| Remove item from dict d                                | del d['name']           |
| Get length of dict d                                   | len(d)                  |
| Check membership in d (only looks in keys, not values) | item in x item not in x |
| Delete all items from dict d                           | d.clear()               |
| Delete dict d                                          | del d                   |

## accesing keys and vallues in a dict

```python
d = {'name': 'Genesis', 'age': 26, 'hometown': 'Valenzuela'}

print(d.keys())
print(d.values())
print(d.items())

print(26 in d.values())

# Output
# dict_keys(['name', 'age', 'hometown'])
# dict_values(['Genesis', 26, 'Valenzuela'])
# dict_items([('name', 'Genesis'), ('age', 26), ('hometown', 'Valenzuela')])
# True

```

## iterating a dict
```python

d = {'name': 'Genesis', 'age': 26, 'hometown': 'Valenzuela'}

for key in d:
    print(key, d[key])

# Output:
# name Genesis
# age 26
# hometown Valenzuela

for k, v in d.items():
    print(k, v)

# Output:
# name Genesis
# age 26
# hometown Valenzuela
```