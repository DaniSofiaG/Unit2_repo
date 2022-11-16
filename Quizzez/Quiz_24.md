# Quiz 2

```diff
Create a program shows the graph of the parabola for 100 values of x in the interval -10 < x < 10   
```

## Code
import random
random.seed(1234)

def produce_three():
    x = []
    y = []
    equation_out= []
    st=-10
    str=10
    for i in range(100):
        x.append(st)
        st +=0.2
        y.append(abs(x[i]))
        equation= round(2 * (st + 5)**2)
        equation_out.append(equation)

        print(f"|  {str(equation).center(10)}  |  {y}  |")
    return y, x

from matplotlib import pyplot as plt

y, x= produce_three()
plt.plot(x,y)
plt.sohow()

## Pycharm

## Graph
