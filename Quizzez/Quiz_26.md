# Quiz 26
```diff
Create a program that ① show the graph and ②create a linear (H_model = m*h+b) for the data below:
h = [57.0, 56.0, 57.0, 56.0, 55.0, 55.0, 54.0, 54.0, 54.0, 53.0, 53.0, 54.0, 53.0, 53.0, 52.0, 52.0, 51.0, 51.0, 51.0, 50.0, 50.0, 49.0, 50.0, 
     49.0, 49.0, 48.0, 49.0, 49.0, 48.0, 48.0, 48.0, 49.0]
```

## Code
```.py
import matplotlib.pyplot as plt
import numpy as np

h = [57.0, 56.0, 57.0, 56.0, 55.0, 55.0, 54.0, 54.0, 54.0, 53.0, 53.0, 54.0, 53.0, 53.0, 52.0, 52.0, 51.0, 51.0, 51.0, 50.0, 50.0, 49.0, 50.0, 49.0, 49.0, 48.0, 49.0, 49.0, 48.0, 48.0, 48.0, 49.0]
x = []

for i in range(1, 33):
    x.append(i)

plt.scatter(x, h, color="#FF00FF")
plt.ylabel("Relative Humidity %")
plt.xlabel("Samples")


m, b = np.polyfit(x, h, 1)
print(f"Liner equation is y={m:.2f}x+({b:.2f})")

x_model = [1, 36]
y_model = []
for i in x_model:
    y_model.append(m * i + b)

plt.plot(x_model, y_model, color="purple")
plt.show()
```

## Pycharm 
<img width="1439" alt="Screen Shot 2022-11-16 at 16 50 28" src="https://user-images.githubusercontent.com/111941990/202119669-882d0bd0-a25e-4c4b-98e2-dac67f7cfc65.png">


## Graph
<img width="369" alt="Screen Shot 2022-11-16 at 16 39 38" src="https://user-images.githubusercontent.com/111941990/202117916-0cc2349b-ee2c-4884-bf05-3ea0d2a53bb1.png">
