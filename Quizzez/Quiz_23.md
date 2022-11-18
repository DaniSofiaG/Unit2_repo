# Quiz 23
```diff
Create a program that produces the graph for the function in Quiz #22  
```

## Code
```.py
import random
random.seed(1234)

def produce_two(n=int, m=int, s=int):
    #y=2(x+
    x_out = []
    y_out = []
    print(f"|      x       |      y(x)    |")
    print(f"|{'°'*29}|")
    for i in range(n):
        x = random.randint(0, 100)
        x_out.append(x)
        m = 3
        s = 2
        y = round(x ** (1 / 2 * (m / s) ** 2),2)
        y_out.append(y)
        y_str=str(y).center(10)

        print(f"|  {str(x).center(10)}  |  {y_str}  |")
    return y_out, x_out

from matplotlib import pyplot as plt

y, x= produce_two(n=100, m=3, s=2)
plt.plot(x, y, color="red", marker="+")
plt.xlabel("Variable x")
plt.ylabel("$y=x^{1/2(m/s)^2}$")
plt.show()
```

## Pycharm
<img width="654" alt="Screen Shot 2022-11-16 at 17 49 46" src="https://user-images.githubusercontent.com/111941990/202133558-71b03467-0308-4217-8f9e-d2a79d9947d9.png">
<img width="1387" alt="Screen Shot 2022-11-16 at 17 50 03" src="https://user-images.githubusercontent.com/111941990/202133532-abe47e07-a81f-4bce-8581-d61fc1bd07f3.png">

## Graph
<img width="419" alt="Screen Shot 2022-11-16 at 17 44 29" src="https://user-images.githubusercontent.com/111941990/202133655-73e197fc-f337-4ec8-b29c-9d05f6da1ca4.png">

## Truth table for: A(A ⊕ B)  
<img width="956" alt="Screen Shot 2022-11-18 at 17 21 20" src="https://user-images.githubusercontent.com/111941990/202654904-9f253861-9e7f-428c-96b3-d3250dda168d.png">





