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
plt.plot(x1,y1,label="line 1",linewidth=6)
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2",linewidth=6)
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title("Two lines on the same graph")
plt.legend()
```

![image](https://github.com/user-attachments/assets/ff140aa0-d05d-49ef-a8e9-7ce821b3843c)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='blue',linestyle='dashed',linewidth=4,marker='o',markerfacecolor='red',markersize=14)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Some Cool Customizations')
```
![image](https://github.com/user-attachments/assets/2833847b-cff9-4cb2-92c5-151736faf446)

```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896,]
plt.plot(years,apples,color='red',linewidth=5)
plt.plot(years,oranges,color='orange',linewidth=5)
plt.xlabel('YEAR')
plt.ylabel('Yields (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges'])
```
![image](https://github.com/user-attachments/assets/bef97fac-8390-48f0-accc-786b165748be)

```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=100,c='red')
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Scatter Plot')
```
![image](https://github.com/user-attachments/assets/ffc32218-d9b2-491d-b0cd-6cf2bff96053)

```
import matplotlib.pyplot as plt
x_values=[1,2,3,4,5,6,7,8,9,10]
y_values=[2,4,5,7,6,8,9,11,12,12]
plt.scatter(x_values,y_values,label='stars',marker='*',s=300,c='cyan')
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Scatter Plot Star')
plt.legend()
plt.savefig("StarScatter.png")
```
![image](https://github.com/user-attachments/assets/a6552a78-8cec-4c14-830e-01538fabe589)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6,7,8,9]
y=[1,4,9,16,25,36,49,64,81]
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Scatter Plot Star')
plt.subplot(2,2,1)
plt.plot(x,y,'ro--')
plt.subplot(2,2,2)
plt.plot(y,x,'g*--')
plt.subplot(2,2,3)
plt.plot(x,x,'bo')
plt.subplot(2,2,4)
plt.plot(y,y,'go')
```
![image](https://github.com/user-attachments/assets/52f208fb-cc63-4616-af1c-3befbb27f372)
```
X=np.arange(0,4*np.pi,0.1)
Y=np.sin(X)
plt.title("Sin Wave Form")
plt.plot(X,Y,linewidth=5,c='green',linestyle='dotted')
```
![image](https://github.com/user-attachments/assets/06eef755-e136-46f2-8fee-8eeb50fdccd8)

```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='red')
plt.fill_between(x,y2,color='blue')
plt.plot(x,y1,color='black')
plt.plot(x,y2,color='white')
plt.legend(['y1','y2'])
plt.show()

```
![image](https://github.com/user-attachments/assets/7828767b-084e-4b67-8a74-a793d00b33f2)
```
import matplotlib.pyplot as plt
height = [10,24,36,40,5]
names=['One','Two','Three','Four','Five']
c1=['g','b']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Bar Graph')
```
![image](https://github.com/user-attachments/assets/87cbefd1-0e17-4e24-af50-9c1635b3cb35)
```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='b')
plt.xlabel('X-AXIS')
plt.ylabel('Y-AXIS')
plt.title('Bar Graph')
```
![image](https://github.com/user-attachments/assets/7380ee63-a197-486f-8493-2d862440619d)

```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='orange',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no.of people')
plt.title('Histogram')
```
![image](https://github.com/user-attachments/assets/44355106-a0db-4c98-8e1f-5999d73704c0)

```
import matplotlib.pyplot as plt
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='grey',alpha=0.5)
plt.show()
```
![image](https://github.com/user-attachments/assets/d55a1988-1cc8-4abd-8643-27e860e7d6c3)
![image](https://github.com/user-attachments/assets/03ab0765-453f-4bbc-b379-35a74bddf21f)
```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Value')
ax.set_title('Box Plot')
```
![image](https://github.com/user-attachments/assets/3305f426-f370-40d6-96e4-c1009ac55b52)

```
import matplotlib.pyplot as plt
activities=['Eat','Sleep','Work','Play']
slices=[3,7,8,6]
colors=['yellow','blue','orange','red']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0.1,0,0),autopct='%1.1f%%')
plt.title('Pie Chart')
plt.show()
```
![image](https://github.com/user-attachments/assets/7e9cc623-9865-4318-9e89-050e02f5e362)

```
labels=['Python','C++','Ruby','Java']
sizes=[215,130,245,210]
colors=['orange','yellow','red','blue']
explode=(0.1,0,0.1,0)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True,startangle=90)
plt.axis('Equal')
plt.show()
```

![image](https://github.com/user-attachments/assets/311bd79f-ed84-48e2-bd83-b9ba87c2f49c)


# Result:
 Thus the process of data visualization has been carried out successfully.
