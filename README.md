# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='first line',linewidth=6)
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='second line',linewidth=6)
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('two lines on same graph')
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/7d950bf6-89ba-4ab1-98cd-6448f9404d2b)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='blue',linestyle='dashed',linewidth=4,marker='o',markerfacecolor='red',markersize=14)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Some cool customization')
plt.show()
```

![image](https://github.com/user-attachments/assets/84d89287-93df-45c9-84c7-9a59ab12572e)

```
years = range(2000, 2012)
apples = [0.895, 0.91, 0.919, 0.926, 0.929, 0.931, 0.934, 0.936, 0.937, 0.9375, 0.9372, 0.939]
oranges = [0.962, 0.941, 0.930, 0.923, 0.918, 0.908, 0.907, 0.904, 0.901, 0.898, 0.9, 0.896]

plt.plot(years, apples, color='red', linewidth=5)
plt.plot(years, oranges, color='orange', linewidth=5)
plt.xlabel('YEAR')
plt.ylabel('Yields (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples', 'Oranges'])
```

![image](https://github.com/user-attachments/assets/c1c4e5cc-ec85-4191-bd11-47080d2c5647)

```
import matplotlib.pyplot as plt

x_values = [0, 1, 2, 3, 4, 5]
y_values = [0, 1, 4, 9, 16, 25]

plt.scatter(x_values, y_values, s=100, c='red')
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Scatter Plot')
plt.show()
```

![image](https://github.com/user-attachments/assets/2993d3ed-00f9-4052-96bd-21fd8f2df39e)

```
import matplotlib.pyplot as plt

x_values = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
y_values = [2, 4, 5, 7, 6, 8, 9, 11, 12, 12]

plt.scatter(x_values, y_values, label='stars', marker='*', s=300, c='blue')
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Scatter Plot Star')
plt.legend()
plt.savefig("StarScatter.png")
```

![image](https://github.com/user-attachments/assets/f242cb96-0902-49b5-aff9-852dfd86443b)

```

import matplotlib.pyplot as plt
x=[1,2,3,4,5,6,7,8,9]
y=[1,4,9,16,25,36,49,64,81]
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Scatter Plot Star')
plt.subplot(2,2,1)
plt.plot(x,y, 'ro--')
plt.subplot(2,2,2)
plt.plot(y,x,'g*--')
plt.subplot(2,2,3)
plt.plot(x,x,'bo')
plt.subplot(2,2,4)
plt.plot(y,y,'go')
```

![image](https://github.com/user-attachments/assets/9c268c41-b2e3-4bfe-b6ef-1766d08ac1f8)

```

import numpy as np
np.pi
X=np.arange(0,4*np.pi,0.1)
Y=np.sin(X)
plt.title("Sin Wave Form")
plt.plot(X,Y, linewidth=5,c='green', linestyle='dotted')
```

![image](https://github.com/user-attachments/assets/38b33efe-d1f3-419d-8c8f-d14d92e12629)

```

import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='red')
plt.fill_between(x,y2, color='blue')
plt.plot(x,y1,color='black')
plt.plot(x,y2,color='white')
plt.legend (['y1', 'y2'])
plt.show()
```

![image](https://github.com/user-attachments/assets/1bb3492d-71d2-41bf-b502-7f7011c5b25f)

```

import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['One', 'Two', 'Three', 'Four', 'Five']
c1=['g', 'b']
plt.bar(names, height, width=0.8, color=c1)
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Bar Graph')
```

![image](https://github.com/user-attachments/assets/5385cbc9-ad03-49b7-86bc-dbe890169f0c)
```

x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2, color='y')
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Bar Graph')
```

![image](https://github.com/user-attachments/assets/369df10b-4d29-4790-b4fa-073f51e71480)

```

import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist (ages, bins, range, color='orange',histtype='bar', rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no.of people')
plt.title('Histogram')
```

![image](https://github.com/user-attachments/assets/f5e9c901-7e05-4915-906b-296f2ae1ab88)

```
import matplotlib.pyplot as plt
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10, color='grey', alpha=0.5)
plt.show()
```
![image](https://github.com/user-attachments/assets/710e18d8-3288-480b-8888-2488d98fab62)

```

import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0, scale=1,size=100)
data
```

![image](https://github.com/user-attachments/assets/f2e7ee91-00ff-4942-9aa9-ed5b53022c94)

```

fig, ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Value')
ax.set_title('Box Plot')
```
![image](https://github.com/user-attachments/assets/5a850251-6afc-482a-ae9d-3e3ac1cb4b25)

# Result:
 Include your result here
