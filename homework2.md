# Homework 2

Counting.

_Hint_: `dir([])`

1. Find the 10 most common words in _Pride and Prejudice_:
```py
import urllib2
response = urllib2.urlopen('https://www.gutenberg.org/files/1342/1342-0.txt')
all_text = response.read()
```

2. Find the [average, median, and mode](http://www.purplemath.com/modules/meanmode.htm) in this list.
```py
numbers = [
  37, 17, 4, 11, 17, 16, 22, 1, 5, 55,
  15, 4, 6, 1, 7, 17, 45, 19, 1, 30,
  8, 20, 22, 59, 15, 5, 2, 4, 7, 19,
  22, 13, 15, 59, 2, 2, 57, 11, 2, 4,
  4, 9, 2, 5, 24, 8, 52, 10, 20, 57,
  10, 20, 33, 11, 14, 7, 54, 42, 7, 49
]
```

