# 22. 
```diff
Create a program that produces n random values from the equation below, where m and s are the other inputs of the function 
```
<img width="285" alt="Screen Shot 2022-11-19 at 13 04 58" src="https://user-images.githubusercontent.com/111941990/202833393-77e60dfe-61d6-4a89-95e0-a13eb7f8ea16.png">


## Code 
```.py
import random
random.seed(1234)

def produce(n=5, m=3, s=2):
    #y=x**(1/2*(m/s)**2)
    print(f"|      x       |      y(x)    |")
    print(f"|{'°'*29}|")
    for i in range(5):
        x = random.randint(0, 100)
        m = 3
        s = 2
        y = round(x ** (1 / 2 * (m / s) ** 2),2)
        y_str=str(y).center(10)

        print(f"|  {str(x).center(10)}  |  {y_str}  |")

produce(n=5, m=3, s=2)
```

## Pycharm and Testing 
<img width="1439" alt="Screen Shot 2022-11-19 at 13 05 46" src="https://user-images.githubusercontent.com/111941990/202833420-e43db591-8c5f-4403-98e9-f5092d4bc812.png">


## Proof that A (A + B) = A 
<img width="408" alt="Screen Shot 2022-11-19 at 13 13 19" src="https://user-images.githubusercontent.com/111941990/202833615-42f63ae0-e75e-4e34-9794-f86e5eef5be7.png">

