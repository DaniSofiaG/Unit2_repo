# 18. Create a function to help Lily

```.py
#Create a function to help Lily

def numberMatches(lenght:int,speed:int)->int:
    number_matches = str(round((lenght/(speed/100))/5))
    return number_matches

test1 = numberMatches(lenght= 12345, speed= 123)
print(f" {test1} matches")
```
