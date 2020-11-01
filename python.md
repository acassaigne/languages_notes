# Learning Python 

## dictionary

create empty dictionary from string keys

```python
my_dict = dict.fromkeys('0123456789')
```

## string 

replace characters in string.
It's about remove a characters set in string.

remove character e and l from hello. 

```python
import str
remove_characters = { 'e' : None, 'l': None}
"Hello".translate(str.maketrans(remove_characters))
```
