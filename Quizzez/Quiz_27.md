# 27
```diff

```

## Code
```.py

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
plt.show()
```

# Pycharm
