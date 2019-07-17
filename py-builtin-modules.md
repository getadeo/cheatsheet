# namedtuple
```python
from collections import namedtuple

Person = namedtuple('Person', ['first', 'last', 'address'])
row = Person('Genesis', 'Tadeo', 'Valenzuela City')

row.first       # Returns 'Genesis'
row.last        # Returns 'Tadeo'
row.address     # Returns 'Valenzuela City'
```

# Counter, defaultdict
```python
from collections import Counter, defaultdict

c = Counter('tcctssssz')
c               # Returns Counter({'s': 4, 't': 2, 'c': 2, 'z': 1})
c['s'] += 10
c['t'] += 13
c               # Returns Counter({'t': 15, 's': 14, 'c': 2, 'z': 1})

d = defaultdict(list)
d['maling'].append(44)
d['itlog'].append(13)
d['maling'].append(33)
d               # Returns defaultdict(<class 'list'>, {'maling': [44, 33], 'itlog': [13]})
```