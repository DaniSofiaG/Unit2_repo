# Quiz 23

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
