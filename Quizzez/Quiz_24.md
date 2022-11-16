# Quiz 2

```diff
Create a program shows the graph of the parabola for 100 values of x in the interval -10 < x < 10   
```

## Code
```.py
import random
random.seed(1234)
x_out = []
y_out = []
st = -10
for i in range (100):
    x_out.append(st)
    y = 2*(st+5)**2
    y_out.append(y)
    st +=0.2
    print(f"|  {str(y).center(10)}  |  {y}  |")

from matplotlib import pyplot as plt
plt.style.use("Solarize_Light2")
plt.plot(x_out,y_out, color="#74d3ae")
plt.ylabel("$2(x+5)**2$")
plt.xlabel("x")

plt.show()
```


## Pycharm

## Graph
