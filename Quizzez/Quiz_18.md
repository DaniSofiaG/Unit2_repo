# 18. Create a function to help Lily

```.py
#Create a function to help Lily

def numberMatches(lenght:int,speed:int):
    number_matches = str(round((lenght/(speed/100))/5))
    return number_matches

test1 = numberMatches(lenght= 12345, speed= 123)
print(f" {test1} matches")
```


<img width="1437" alt="Screen Shot 2022-11-14 at 13 56 10" src="https://user-images.githubusercontent.com/111941990/201578567-7ee0d727-8c4a-474e-9e3a-ec89549b130d.png">
