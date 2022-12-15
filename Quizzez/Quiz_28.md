# 28.
```diff
Create a graph for the x, y data below:

data =  {
'x': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19],
'y': [24, 1, 2, 25, 26, 21, 23, 34, 49, 2, 19, 32, 7, 17, 36, 7, 45, 28, 40, 46]
}  
```

## Code
```.py
from matplotlib import pyplot as plt

data = {
    "x": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19],
    "y": [24, 1, 2, 25, 26, 21, 23, 34, 49, 2, 19, 32, 7, 17, 36, 7, 45, 28, 40, 46]
    }

plt.plot(data["x"], data["y"])
plt.title("Quiz028")
plt.show()
```

## Pycharm
<img width="698" alt="Screen Shot 2022-12-15 at 21 21 52" src="https://user-images.githubusercontent.com/111941990/207858288-3884df09-c2a7-4ec1-9361-401d32a26e58.png">


## Graph
<img width="368" alt="Screen Shot 2022-12-15 at 21 21 12" src="https://user-images.githubusercontent.com/111941990/207858271-39022424-badd-4396-b1ed-265a1465d435.png">
