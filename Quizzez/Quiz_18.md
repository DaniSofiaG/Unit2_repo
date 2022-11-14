# 18. Create a function to help Lily

```.py
#Create a function to help Lily

def numberMatches(lenght:int,speed:int)->int:
    number_matches = str(round((lenght/(speed/100))/5))
    return number_matches

test1 = numberMatches(lenght= 12345, speed= 123)
print(f" {test1} matches")
```

<img width="1437" alt="Screen Shot 2022-11-14 at 13 53 49" src="https://user-images.githubusercontent.com/111941990/201578263-72821b76-a607-4643-a89c-ec879af079da.png">

