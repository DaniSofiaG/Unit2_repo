# Quiz 24

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
<img width="1435" alt="Screen Shot 2022-11-16 at 17 38 48" src="https://user-images.githubusercontent.com/111941990/202131122-8c30808d-3d53-4ce8-8077-54f3d37a9c17.png">


## Graph
<img width="639" alt="Screen Shot 2022-11-16 at 17 38 08" src="https://user-images.githubusercontent.com/111941990/202131152-6c27a95b-b2ef-4d2a-a397-905576a28681.png">

## Circuit Diagram
```diff
not(bit0 bit1 + not (bit0 + bit1)) 
```
![Untitled drawing](https://user-images.githubusercontent.com/111941990/202322520-1e3e3624-373b-4ce7-aa6a-5e4f57961c5f.jpg)


