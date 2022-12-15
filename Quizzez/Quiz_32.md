# 32.

```diff
Compare the data from sensor#9 and 10 with smoothing of 12 samples.
```

## Code
```.py
import requests
import matplotlib.pyplot as plt
import numpy as np

plt.style.use("Solarize_Light2")
req = requests.get('http://192.168.6.142/readings')
data = req.json()
readings = data["readings"][0]
print(len(readings))


T = []
K = []
for sample in readings:
    if sample["sensor_id"] == 9:
        T.append(sample["value"])

    if sample["sensor_id"] == 10:
        K.append(sample["value"])

# slice temperature to the regioun of interest
t_temp = T[0: 600]
xof_t = []
for i in range(len(t_temp)):
    xof_t.append(i)

k_temp = K[0: 600]
xof_k = []
for i in range(len(k_temp)):
    xof_k.append(i)

#Smoothing

samples_per_hour = 12
mean_per_hour = []
standard_per_hour = []
x_per_hour = []
hour = 0
for i in range(0, len(T), samples_per_hour):
    data = T[i:i + samples_per_hour]
    mean_per_hour.append(sum(data)/samples_per_hour)
    standard_per_hour.append(np.std(data))
    x_per_hour.append(hour)
    hour += 1

k_samples_per_hour = 12
k_mean_per_hour = []
k_standard_per_hour = []
k_x_per_hour = []
k_hour = 0
for i in range(0, len(T), k_samples_per_hour):
    data = T[i:i + k_samples_per_hour]
    k_mean_per_hour.append(sum(data) / k_samples_per_hour)
    k_standard_per_hour.append(np.std(data))
    k_x_per_hour.append(hour)
    k_hour += 1

# difference as comparison
diff = []
for m in range(len(mean_per_hour)):
    d = k_mean_per_hour[m]-k_mean_per_hour[m]
    diff.append(d)

#Graphing
plt.subplot(2,1,1)
plt.plot(T)
plt.subplot(2,1,2)
plt.plot(K)



plt.show()
```

## Pycharm & Testing
<img width="770" alt="Screen Shot 2022-12-15 at 9 13 03" src="https://user-images.githubusercontent.com/111941990/207742636-2f1008c5-1897-4942-ad52-4d0df8e4547e.png">
<img width="738" alt="Screen Shot 2022-12-15 at 9 13 11" src="https://user-images.githubusercontent.com/111941990/207742659-b3bd74dd-8005-4930-a97a-364cc2fc0291.png">
<img width="536" alt="Screen Shot 2022-12-15 at 9 13 27" src="https://user-images.githubusercontent.com/111941990/207742672-fd1f5679-b93e-4d3d-be10-8b51f6f50f67.png">

## Graphing
<img width="622" alt="Screen Shot 2022-12-15 at 9 14 19" src="https://user-images.githubusercontent.com/111941990/207742716-c805c7fa-be4d-4fb6-963f-5603fc96c685.png">

## What are the three main operators used in boolean logic?
```diff
And
```
```diff
Or
```
```diff
Not
```
<img width="182" alt="Screen Shot 2022-12-15 at 9 15 44" src="https://user-images.githubusercontent.com/111941990/207742868-13faf30e-0979-4a17-8924-8c1d343ce633.png">

