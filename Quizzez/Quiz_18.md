# 18. 
```diff
Create a function to help Lily
```
<img width="417" alt="Screen Shot 2022-11-19 at 11 07 12" src="https://user-images.githubusercontent.com/111941990/202829333-9462b934-3b99-47f7-8410-a17ce8f65eec.png">

# Code

```.py
#Create a function to help Lily
def numberMatches(lenght:int,speed:int):
    number_matches =((lenght/(speed/100))/5)

    if not number_matches % 2 == 0:
        addition= number_matches + 1
        matches = str(round(addition))
    else:
        if number_matches % 2 == 0:
            matches = str(round(number_matches))

    return matches

#TESTING
test1 = numberMatches(lenght= 100, speed= 100)
print(f" {test1} matches")

test2 = numberMatches(lenght= 250, speed= 110)
print(f" {test2} matches")

test3 = numberMatches(lenght= 500, speed= 150)
print(f" {test3} matches")
```

## Pycharm and Testing
<img width="1440" alt="Screen Shot 2022-11-19 at 11 00 53" src="https://user-images.githubusercontent.com/111941990/202829093-5cd7b618-4006-49b8-8a5c-273bb250a771.png">


## Flow Chart 
<img width="503" alt="Screen Shot 2022-11-19 at 11 06 41" src="https://user-images.githubusercontent.com/111941990/202829301-2b6ea923-6d96-4acd-aef9-83172aeab6c9.png">


