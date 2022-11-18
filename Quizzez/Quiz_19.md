# 19. 
```diff
Create a function that changes the vowels in a string to numbers such as a=4,e=3,i=1,o=0 and space by _
```

## Code
```.py
def get_l3tt3rs(msg:str):
    output = ""
    vocals_integers = {" ": "_",
                       "a": "4",
                       "e": "3",
                       "i": "1",
                       "o": "0",
                        }
    for i in msg:
        if i in vocals_integers:
            output = output + vocals_integers[i]

        if i not in vocals_integers:
            output = output + i

    return output

#TESTING
#1
case1 = get_l3tt3rs(msg="Hello World")
print(case1)
#2
case2 = get_l3tt3rs(msg="Why did I choose CS?")
print(case2)
#3
case3 = get_l3tt3rs(msg="Remember the Figure Caption")
print(case3)
## Pycharm & Testing
```

## Pycharm & Testing
<img width="1106" alt="Screen Shot 2022-11-18 at 18 41 35" src="https://user-images.githubusercontent.com/111941990/202671370-6925714f-5997-4275-ae69-b1c9aae2b820.png">
<img width="1106" alt="Screen Shot 2022-11-18 at 18 41 35" src="https://user-images.githubusercontent.com/111941990/202671383-b56884fd-1943-408f-9e10-694b5976f161.png">


## Boolean Circuit: AB + not(B+C) + B(notC notA)
<img width="1267" alt="Screen Shot 2022-11-18 at 17 54 14" src="https://user-images.githubusercontent.com/111941990/202661442-887dc3ff-2ab3-42a4-b6fe-9955638fd324.png">



