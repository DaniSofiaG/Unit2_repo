# 29. 

```diff
Create a function that receives a dictionary with letters in the alphabet as keys and a string. The functions returns the dictionary with a count as value for the occurrence of each letter:
```

## Code
```.py
def count_letters(lexicon, msg):

    for letter in msg:
        if letter in lexicon.keys():
            lexicon[letter]+=1

    return lexicon

#Testing
letters = {"w": 0, "l": 0, "c": 0}
test1 = count_letters(letters, "hello world")
print(test1)

vowels = {"a": 0, "i": 0, "u": 0, "e": 0, "o": 0}
test1 = count_letters(vowels, "hello world")
print(test1)
```

## Pycharm & Testing
<img width="1211" alt="Screen Shot 2022-12-07 at 21 59 42" src="https://user-images.githubusercontent.com/111941990/206185885-d5708796-c94c-4b8a-92a8-64bca3068030.png">


## How many colors could you represent in a 6 bit computer?
<img width="937" alt="Screen Shot 2022-12-15 at 9 50 52" src="https://user-images.githubusercontent.com/111941990/207746651-612062b8-0a15-4b51-9bea-9509d075219b.png">
