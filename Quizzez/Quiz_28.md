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
import matplotlib.pyplot as plt

data = {
    "x": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16,17, 18, 19],
    "y": [24, 1, 2, 25, 26, 21, 23, 34, 49, 2, 19, 32, 7, 17, 36, 7, 45, 28, 40, 46]
    }

'''devide = str(data).split("]")

y = (devide[1] [8: -1])
x = (devide[0] [7: 75])
print(list(x))'''

data_list=list(data.values())
x = (int(data_list[0]))
y = (int(data_list[1])

plt.plot(x, y)
plt.show()
```

## Pycharm
<img width="525" alt="Screen Shot 2022-12-15 at 9 55 15" src="https://user-images.githubusercontent.com/111941990/207747113-0cc4a07a-540e-44c3-87fa-755d0ed91b4b.png">


## Graph

