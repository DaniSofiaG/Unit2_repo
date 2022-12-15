# 31.

```diff
Connect to the server and download the recordings data. From the data, build a linear model between t=610 and t=800 
 
```

## Code
```.py
import numpy as np
import requests
from matplotlib import pyplot as plt


req = requests.get('http://192.168.6.142/readings')
data = req.json()
readings = data['readings'][0]

#DATA
temp = []
for sample in readings:
    if sample['sensor_id']==5:
        temp.append(sample['value'])
x = np.arange(0,190)
hum2 = temp[610:800]

#QUADRATIC MODEL y2
a,b,c = np.polyfit(x,hum2, 2)
for i in x:
    y2 = ((x**2)*a) + (b*x) + c

#LINEAR MODEL y3
m,b = np.polyfit(x,hum2, 1)
for i in x:
    y3 = (m*x)+b

#GRAPHING
fig=plt.figure(figsize=(9,6))
plt.subplot(2,1,1) #DATA
plt.plot(temp)
plt.xlabel('Time')
plt.ylabel('Temperature')

plt.subplot(2,1,2) #MODEL
plt.scatter(x,hum2)
line1, = plt.plot(y3,c="green",label="Linear")
line2, = plt.plot(y2,c='red', label='Quadratic')
plt.xlabel('Time')
plt.ylabel('Temperature')
plt.legend(handles=[line1, line2])

plt.show()
```

## Pycharm
<img width="792" alt="Screen Shot 2022-12-15 at 9 22 19" src="https://user-images.githubusercontent.com/111941990/207743584-1f290fe7-98f3-4d21-b78f-16bd19ad2f88.png">
<img width="459" alt="Screen Shot 2022-12-15 at 9 22 24" src="https://user-images.githubusercontent.com/111941990/207743592-f1603b2c-39a0-4a75-bc3d-ebe224933037.png">


## Graphing 

<img width="364" alt="Screen Shot 2022-12-15 at 9 19 23" src="https://user-images.githubusercontent.com/111941990/207743314-bf626484-b3e3-4d7a-87d5-b0defa5ed60b.png">
