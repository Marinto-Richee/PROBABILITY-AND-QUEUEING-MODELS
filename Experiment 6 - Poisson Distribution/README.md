# Poisson Process

# Aim : 
To find the probability of that  (i) exactly 4 customers arrive (ii) more than 4 customers arrive (iii) fewer than 4 customers in 2 minute  arrival. Given that the customers arrive at a bank according to a Poisson process with mean rate of 3 per minute  during a time interval of 2 min. 


# Software required :  

Python

# Theory:

The Poisson process is one of the most widely-used counting processes. It is usually used in scenarios where we are counting the occurrences of certain events that appear to happen at a certain rate, but completely at random (without a certain structure). For example, suppose that from historical data, we know that earthquakes occur in a certain area with a rate of 2 per month. Other than this information, the timings of earthquakes seem to be completely random. Thus, we conclude that the Poisson process might be a good model for earthquakes. In practice, the Poisson process or its extensions have been used to model.

1. The number of car accidents at a site or in an area
2. The location of users in a wireless network
3. The requests for individual documents on a web server
 
# Procedure :

![image](https://user-images.githubusercontent.com/104613195/172528169-f26bdf76-f357-4c48-b806-a0a80da21cac.png)

# Program :
```python
# Developed by
# Register Number: 212220230031
# Name: Marinto Richee J

import numpy as np
import math
lambda_=3
time_interval=2
def pd(x):
    return (math.exp(-(lambda_*time_interval))*(lambda_*time_interval)**x)/(math.factorial(x))
print("The Probability that exactly 4 customers is {0:0.4f}".format(pd(4)))

p_4=[pd(i) for i in range(0,5)]
print("The Probability that more than 4 customers is {0:0.4f}".format(1-sum(p_4)))

p_4=[pd(i) for i in range(0,4)]
print("The Probability that less than 4 customers is {0:0.4f}".format(sum(p_4)))

```
# Results and Output : 
```
The Probability that exactly 4 customers is 0.1339
```
```
The Probability that more than 4 customers is 0.7149
```
```
The Probability that less than 4 customers is 0.1512
```
Hence a python program to find the probability of that  (i) exactly 4 customers arrive (ii) more than 4 customers arrive (iii) fewer than 4 customers in 2 minute  arrival. Given that the customers arrive at a bank according to a Poisson process with mean rate of 3 per minute  during a time interval of 2 min, has been done. 
