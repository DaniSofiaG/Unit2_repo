# 33.

```.diff
```

## Code 
```.py 
# Quiz33
from matplotlib import pyplot as plt
from matplotlib.gridspec import GridSpec

from library_unit2 import download, get_sensor, smoothing

plt.style.use('Solarize_Light2')
readings = download()
sensors = [6, 8, 9, 10]

sensor_data = []
for s in sensors:
    data = get_sensor(readings, s)
    x, data_smth = smoothing(data[0:501])
    sensor_data.append(data_smth)

mean_per_hour = []
for i in range(len(sensor_data[0])):
    # in line for loop
    d = [sensor_data[x][i] for x in range(len(sensors))]
    mean_per_hour.append(sum(d) / len(sensors))
 ```
 
 ## Pycharm
 
