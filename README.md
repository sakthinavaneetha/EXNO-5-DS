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
![image](https://github.com/user-attachments/assets/2bb9e8d2-5df8-4f1b-ae24-56116928cf3f)


import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
![image](https://github.com/user-attachments/assets/675fec77-bea6-4b40-8175-2b1029ae8145)


yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
![image](https://github.com/user-attachments/assets/99eb09f9-430f-41ea-9ad9-a306d0d3064e)


years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
![image](https://github.com/user-attachments/assets/ab843827-e236-4cf3-b7e3-278d02e45c6e)


years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);
![image](https://github.com/user-attachments/assets/f06dcecd-094a-43cf-af15-4f39b287e0bc)

plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
![image](https://github.com/user-attachments/assets/1e1fc4b2-d1b1-413c-bb3b-c5036e7565fa)


import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
![image](https://github.com/user-attachments/assets/ff0c20ff-9ddd-4f1b-96db-516c2855a34c)


y
![image](https://github.com/user-attachments/assets/77cfe5e5-b44d-46fb-9572-a41a55628eb2)


plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
![image](https://github.com/user-attachments/assets/711ff4f3-75cf-4e72-8b57-e82b27effc64)


y=x*x
y
![image](https://github.com/user-attachments/assets/927a3aad-edd9-4687-920c-9a03f4320940)


plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
![image](https://github.com/user-attachments/assets/cc60d9c5-201f-4aab-8cee-61d8860a3a09)


np.pi
![image](https://github.com/user-attachments/assets/098c9a02-9d2c-495a-ba6a-0848a756dfdd)


x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
![image](https://github.com/user-attachments/assets/c8d9e2e7-41e8-4200-ad20-a89d948174a6)


import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
![image](https://github.com/user-attachments/assets/e461e63c-7d5a-4ef5-945a-7e666a0b0d55)


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
![image](https://github.com/user-attachments/assets/40264a1a-aa4b-44e8-8e74-a90879a362d8)


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
![image](https://github.com/user-attachments/assets/4f28f956-0ff6-4555-9713-2026aab4e85b)


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
![image](https://github.com/user-attachments/assets/4406fc32-0568-4741-ac30-54fe4f6472fb)


import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
![image](https://github.com/user-attachments/assets/3ad1be21-7176-42ab-9e4a-de8c0223bfaf)


import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
![image](https://github.com/user-attachments/assets/0aa50508-4c4f-455d-87be-983a0d19124d)


fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
![image](https://github.com/user-attachments/assets/738d2b4f-6c30-47a4-95f4-d08f36528c65)


labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
![image](https://github.com/user-attachments/assets/fa1836dd-82e6-4ab3-b88a-305f85241384)


activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
![image](https://github.com/user-attachments/assets/1b3a075f-7a02-4a01-b74e-6e8d116cc6b3)


# Result:
Thus, The implementation of data visualization using matplotlib has been successfully verified.
