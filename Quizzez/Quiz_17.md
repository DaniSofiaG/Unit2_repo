# 17.
```diff
Create a function that produces the average world length of the input list
```


## Code
```.py
def word_length(words:list) -> int:
    addition = 0
    for i in range(len(words)):
        addition = addition + len(words[i])

    average = addition / len(words)
    return average


# TESTING
test_1 = word_length(words=["hello", "main"])
print(test_1)

test_2 = word_length(words=["Peru","France", "Nepal"])
print(test_2)

test_3 = word_length(words=["Computer Science", "Art"])
print(test_3)

test_4 = word_length(words=["one", "two"])
print(test_4)
```


## Pycharm and Testing
<img width="1440" alt="Screen Shot 2022-11-19 at 14 46 03" src="https://user-images.githubusercontent.com/111941990/202836686-1810d337-94f2-46ad-b26a-906d20c9a775.png">

## Flow Chart
<img width="435" alt="Screen Shot 2022-11-22 at 13 37 29" src="https://user-images.githubusercontent.com/111941990/203222839-637fab33-489c-47ca-8c1a-fdd7efdacb19.png">

