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
plt.plot(x1,y1,label='line1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/9fe3e76f-15c1-46ba-90b1-eae0986549a7)
```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/91fad8cb-a8cd-421e-88ea-b6788038e7bb)

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/2121dd7d-9996-454b-a11f-810d62fe0657)
```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/a3f97f86-81d4-4a9d-8213-df31074570ea)

```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]

```
```
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/6a571a7e-da7f-4a63-8fc6-cd7a0d08f57f)

```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/6371ec70-e867-40c4-975a-f4620a447fed)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/75989793-cf3f-499b-9193-a2b19b810516)

```
y
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/a67ee97f-816e-46ec-b700-af1ce6f40ec0)

```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/f69ddaed-ec98-4540-bc28-e7b82c4c6236)

```
y=x*x
y
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/d3d157af-1a4c-4b36-bd40-589c6dca9ba8)

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/9a51ad44-9499-4b6c-ab74-9fde34c490c8)

```
np.pi
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/ef67502a-19a8-4f3d-9bff-dd953661d07d)

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/9863501f-6ecb-4e36-9dc9-1190acb39831)
```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/4918e057-27f3-4ef3-a307-0b29ee4b57c7)

```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')

plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/465e5a95-840a-4ad8-bd8b-7ad3d6a24b22)

```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/3571b12c-0277-403b-8231-ab0a9851136b)

```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/c1b76b36-cab5-47cc-86c1-637569557409)


```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/5a5f0a8b-e58f-4632-8ce7-06c166dc16d1)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/e2ac0add-4c85-480e-9076-52b03629e2c0)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/4b6ca2c6-c074-48a7-b834-7cfc80df64ab)

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```

![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/8ed40a32-9f42-4fea-b3b8-92d9c822db26)

```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![image](https://github.com/Jeevapriya14/EXNO-5-DS/assets/121003043/f556d17b-a4cf-40e8-94f9-a4dfba38be50)




# Result:
 Thus, The implementation of data visualisation using matplotlib has been successfully verified!
