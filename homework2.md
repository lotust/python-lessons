# Homework 2

Counting.

_Hint_: `dir([])`

1. Find the 10 most common words in _Pride and Prejudice_:
```py
import urllib2
response = urllib2.urlopen('https://www.gutenberg.org/files/1342/1342-0.txt')
all_text = response.read()
```
my answer:

```import urllib2

response = urllib2.urlopen('http://www.gutenberg.org/files/1342/1342-0.txt')
all_text = response.read()

#myanswer
from collections import Counter
pride = all_text.split()
prejudice = Counter(pride).most_common(10)
print prejudice

pride_words = all_text.split() 
prejudice_dict = {}
def wordcounter(pridelist):
    for i in pridelist:
        if i in prejudice_dict:
            prejudice_dict[i] += 1
        else:
            prejudice_dict[i] = 1
def wordsorter(prejudice_dict):
    sorted_prejudice = [(value, key) for key, value in prejudice_dict.items()]
    sorted_prejudice.sort(reverse=True)
    print sorted_prejudice[:10]

wordcounter(pride_words)
wordsorter(prejudice_dict)
```

2. Find the average, median, and mode in this list.
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

