# 20. 
```diff
Create a function that produces the table of Truth for 3 inputs:
```

## Code
```.py
def get_truth():
    A = True
    B = True
    C = True
    print(f"| A | B | C |")
    print("°", "-"*9,"°")

    for i in range(8):
        if i % 1 == 0:
            C = not C

        if i % 2 == 0:
            B = not B

        if i % 4 == 0:
            A = not A

        print(f"| {int(A)} | {int(B)} | {int(C)} |")

    return A, B, C

table = get_truth()
print(table)
```

## Pycharm and testing

<img width="1440" alt="Screen Shot 2022-11-18 at 19 42 14" src="https://user-images.githubusercontent.com/111941990/202686168-08bcbb60-a154-4997-bb89-e07ebbf41a0d.png">

## Truth table and circuit: Light = S1S2+(S2+S3(notS1))S1 
<img width="968" alt="Screen Shot 2022-11-22 at 13 54 06" src="https://user-images.githubusercontent.com/111941990/203224943-f361845d-e5a3-4338-96c0-5b96c2526d4b.png">


<img width="1276" alt="Screen Shot 2022-11-18 at 21 33 57" src="https://user-images.githubusercontent.com/111941990/202706053-23268710-8e7c-4ec1-8333-77cbc71f70d3.png">

