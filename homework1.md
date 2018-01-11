# Homework 1
Strings and arrays. Learn about
```py
# find methods that exist on strings and arrays
dir('')
dir([])

# print documentation on a thing called `stuff`
help(stuff)

# list indexing
a = [1, 2, 4]
b = a[2] # b == 4

# list/string slicing
a = 'hello there'
b = a[4:8] # b == 'o th'
```

1. Make a variable called `well_formed`. It should begin with a capital letter, and not have leading/trailing whitespace. Start from this code:
```py
poorly_formed = '   boop '
```

2. Download a list of words, and find the 1000th word. Start with this.
```py
import urllib2
response = urllib2.urlopen('https://github.com/dwyl/english-words/raw/master/words.txt')
all_text = response.read()
```

3.
