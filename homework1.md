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
well_formed = poorly_formed.strip().capitalize()
```

2. Download a list of words, and find the 1000th word. Start with this.
py
import urllib2
response = urllib2.urlopen('https://github.com/dwyl/english-words/raw/master/words.txt')
all_text = response.read()
word_list = all_text.split()
print word_list[999]

3. Find how many vowels are in the text above.
letter_list = list(all_text)
def vowel_counter(abc):
  vowelcount = 0
  for i in abc:
    if i == "a":
      vowelcount += 1
    elif i == "e":
      vowelcount += 1
    elif i == "i":
      vowelcount += 1
    elif i =="o":
      vowelcount += 1
    elif i =="u":
      vowelcount += 1
  return vowelcount
print vowel_counter(letter_list)
