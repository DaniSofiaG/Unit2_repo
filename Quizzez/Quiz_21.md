# 21.
```diff
Using the function that produces the table of Truth for 3 inputs, add a column for the boolean equation
AB+(not B)+(notB C)
```

## Code 
```.py
A = True
B = True
C = True
print(f"| A | B | C | AB+(not B)+(notB C) |")
print("°", "-"*9,"°", "-"*19, "°")

for i in range(8):
    if i % 1 == 0:
        C = not C

    if i % 2 == 0:
        B = not B

    if i % 4 == 0:
        A = not A

    equation= A and B or (not B) or (not B and C)
    print(f"| {int(A)} | {int(B)} | {int(C)} | {int(equation):^19} |")
```

## Pycharm 
<img width="1440" alt="Screen Shot 2022-11-19 at 11 44 52" src="https://user-images.githubusercontent.com/111941990/202830638-f3465e21-0d4c-44fd-a5d9-4e5877d8888f.png">
