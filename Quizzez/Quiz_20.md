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
<img width="1200" alt="Screen Shot 2022-11-18 at 21 03 13" src="https://user-images.githubusercontent.com/111941990/202701020-5b29920d-fbf3-401c-894c-4844b708876e.png">

