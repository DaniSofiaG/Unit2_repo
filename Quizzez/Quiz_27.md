# 27.
```diff
Create a errorbar graph for the data below. You will need to calculate the mean and standard deviation first.

sensorA = [16, 24, 24, 9, 23, 26, 26, 23, 25, 14]  
sensorB = [2, 19, 25, 10, 11, 24, 17, 7, 24, 17]  
sensorC = [15, 11, 24, 21, 6, 2, 18, 27, 1, 16]  
```

## Code
```.py

import numpy as np
import matplotlib.pyplot as plt
sensorA = [16, 24, 24, 9, 23, 26, 26, 23, 25, 15]
sensorB = [2, 19, 25, 10, 11, 24, 17, 7, 24, 17]
sensorC = [15, 11, 24, 21, 6, 2, 18, 27, 1, 16]
x = []
z = []
p = []

for i in range(len(sensorA)):
    x.append(i)
plt.plot(x, sensorA, color="#F67E7D")

for n in range(len(sensorB)):
    z.append(n)
plt.plot(z, sensorB, color="#FF00FF")

for k in range(len(sensorC)):
    p.append(k)
plt.plot(p, sensorC, color="#54c6eb")
mean = []
std = []
max_v = []
min_v = []
for n in range (len(sensorB)):
    data = [sensorA[n], sensorB[n], sensorC[n]]
    mean.append(sum(data)/3)
    std.append(np.std(data))
    min_v.append(min(data))
    max_v.append(max(data))
plt.errorbar(x, mean, std)
plt.fill_between(x, max_v, min_v,color="#65c6eb", alpha=0.7)

plt.show()
```

## Pycharm
<img width="1439" alt="Screen Shot 2022-12-05 at 8 21 33" src="https://user-images.githubusercontent.com/111941990/205521885-7d670f52-98a7-42c9-867f-9d3568ca2b57.png">

## Graph
<img width="409" alt="Screen Shot 2022-12-05 at 8 19 34" src="https://user-images.githubusercontent.com/111941990/205521809-480c9323-8057-4c40-84a2-bf5aac216903.png">

## Convert the following rgb color to hex color: red=250, green=100, blue=10



