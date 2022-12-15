# Quiz 25
```diff
Create a program shows the graph of the function below for 100 values of x in the interval -10 < x < 10
```

## Code
```.py
import random
random.seed(1234)

x_axis = []
y_axis = []
st = -10
for i in range (100):
    x_axis.append(st)
    y = abs(st)
    y_axis.append(y)
    y_str = f"{y:2f}"
    st +=0.2

from matplotlib import pyplot as plt
plt.style.use("Solarize_Light2")
plt.plot(x_axis, y_axis, color = "#FF56A5")
plt.xlabel("x")
plt.ylabel("$f(x) = |x|$")
plt.show()
```

## Pycharm
<img width="930" alt="Screen Shot 2022-11-16 at 17 05 00" src="https://user-images.githubusercontent.com/111941990/202125798-5ae925b1-ca2d-45c5-9bab-98b18905472f.png">


## Graph
<img width="469" alt="Screen Shot 2022-11-16 at 17 04 29" src="https://user-images.githubusercontent.com/111941990/202125858-b5fe4799-2c11-43bf-8bda-c0951ddda4d7.png">

## Convert FFA5 to Decimal 
<img width="578" alt="Screen Shot 2022-12-15 at 20 53 58" src="https://user-images.githubusercontent.com/111941990/207852859-9325587e-05e1-4af4-86a9-90544e2b0e82.png">

