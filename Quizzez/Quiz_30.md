# 30.

```diff
Using the data in the learning Log (Item 21), create a graph with a smoothed version where the smoothing window is every 4 points.

```

## Code
```.py
import matplotlib.pyplot as plt

h = [57.0, 56.0, 57.0, 56.0, 55.0, 55.0, 54.0, 54.0, 54.0, 53.0, 53.0, 54.0, 53.0, 53.0, 52.0, 52.0, 51.0, 51.0, 51.0, 50.0, 50.0, 49.0, 50.0, 49.0, 49.0, 48.0, 49.0, 49.0, 48.0, 48.0, 48.0, 49.0]
x = []
sample_per_window = 4
mean_per_window = []

for i in range(0,len(h), sample_per_window):
    mean_per_window.append(sum(h[i:i+sample_per_window])/sample_per_window)
    x.append(i)

plt.style.use("ggplot")
plt.scatter(x, mean_per_window)
plt.plot(x, mean_per_window, color="#FF00FF")
plt.ylabel("Relative humidity")
plt.xlabel("Samples")

plt.show()
```

## Pycharm 
<img width="886" alt="Screen Shot 2022-12-07 at 22 04 23" src="https://user-images.githubusercontent.com/111941990/206186685-a4d0585b-618b-4a8f-af77-77857e5c5066.png">

## Graph
<img width="423" alt="Screen Shot 2022-12-07 at 22 04 01" src="https://user-images.githubusercontent.com/111941990/206186718-57cbdcee-eb89-4e6c-833f-1a312f09ba3f.png">

## When was the internet first created? Remember to add your sources
"January 1, 1983 is considered the official birthday of the Internet. Prior to this, the various computer networks did not have a standard way to communicate with each other. "
#### MLA: 
A Brief History of the Internet. (n.d.). https://www.usg.edu/galileo/skills/unit07/internet07_02.phtml
