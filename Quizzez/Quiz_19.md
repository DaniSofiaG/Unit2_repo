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
Test_1 = get_l3tt3rs(msg="Hello World")
print(Test_1)

Test_2 = get_l3tt3rs(msg="Why did I choose CS?")
print(Test_2)

Test_3 = get_l3tt3rs(msg="Remember the Figure Caption")
print(Test_3)
```

## Pycharm & Testing
<img width="1440" alt="Screen Shot 2022-11-18 at 18 47 16" src="https://user-images.githubusercontent.com/111941990/202672737-df567662-e34c-4fcf-8fd9-5fb611a74430.png">
<img width="1440" alt="Screen Shot 2022-11-18 at 18 46 59" src="https://user-images.githubusercontent.com/111941990/202672509-f2781e06-1ffa-4e77-adaf-9d29f9e224eb.png">


## Boolean Circuit: AB + not(B+C) + B(notC notA)
<img width="1267" alt="Screen Shot 2022-11-18 at 17 54 14" src="https://user-images.githubusercontent.com/111941990/202661442-887dc3ff-2ab3-42a4-b6fe-9955638fd324.png">



