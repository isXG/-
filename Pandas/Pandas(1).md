<img width="1487" height="709" alt="image" src="https://github.com/user-attachments/assets/f2b7e715-495c-4da4-a004-f4f9219438c4" />

## 一.（1）对象的创建

### ①字典创建法

#### 例程,Serie需传入字典

```
import pandas as pa
dict_v = {'a':0 , 'b' : 0.25 , 'c' : 0.5 , 'd' : 0.75 , ' e' : 1}
print(dict_v) #创建字典
sr = pd.Series(dict_v)#用字典创建对象
print(sr)

```
<img width="585" height="182" alt="image" src="https://github.com/user-attachments/assets/062202ec-8b43-455f-afc1-39c488d62a41" />

### ②数组创建法

<img width="1442" height="150" alt="image" src="https://github.com/user-attachments/assets/b05a6320-a12f-4343-be81-3e044d410403" />

#### 例程,Series第一个传入值，第二个键

#### v可以是numpy中的数组，也可以是torch中的张量，index省略则默认从0开始

```
v = [0,1,2]
k = ['blue','chess','short']
sr = pd.Series(v,index = k)
print(sr)

```
<img width="255" height="125" alt="image" src="https://github.com/user-attachments/assets/4ee94e8f-208b-4d65-bc8c-8d26c09d4ae5" />

## 一.（2）一维对象的属性

<img width="889" height="88" alt="image" src="https://github.com/user-attachments/assets/68241d57-2bda-4671-ba2d-31be2fb1b33d" />

<img width="960" height="721" alt="image" src="https://github.com/user-attachments/assets/dae9dd73-64ad-43cb-9f61-9e537503087e" />

<img width="1545" height="313" alt="image" src="https://github.com/user-attachments/assets/7c4aafc7-25a1-46c7-a384-162f1b6f3938" />

## 一.（3）二维对象的创建----字典创建法，必须基于多个series对象

<img width="1464" height="295" alt="image" src="https://github.com/user-attachments/assets/e095cf52-7466-42c2-8a98-e683fbd65cd1" />

<img width="965" height="285" alt="image" src="https://github.com/user-attachments/assets/6e720371-1584-43f0-9e35-3b534869b03d" />

### 对原文的一些解释。一维的时候，创建的Series对象的key是沿着数直方向延伸的，如上图。

### 而DataFrame是二维对象。它的key，也就是列标签是沿着水平方向延展的。

### 例程

```
v_1 = [' male ', ' female' , ' male ']
i = ['1' , '2','3']
sr1 = pd.Series(v_1,i_1)
print(sr1)
v_2 = [56, 90 , 32]
i = ['1' , '2','3']#4,5,6
sr2 = pd.Series(v_2,i)
print(sr2)
df = pd.DataFrame({'性别':sr1,'年龄':sr2})
print(df)
```
<img width="1524" height="159" alt="image" src="https://github.com/user-attachments/assets/8ec0d97b-4c59-4e3f-8b0f-e614c3f92a80" />

<img width="224" height="320" alt="image" src="https://github.com/user-attachments/assets/20e29e27-3fcd-42bb-97cd-890503366809" />

<img width="230" height="396" alt="image" src="https://github.com/user-attachments/assets/297b3487-7353-41d0-9005-31934e52dacc" />

## 一.（3）二维对象的创建----数组创建法 pd.DataFrame(v,index = k,columns = c)

<img width="1482" height="202" alt="image" src="https://github.com/user-attachments/assets/3e54abac-6e12-4647-8f36-28516ff50c11" />

### 例程

```
v = np.array([[53,'female'],[64,'male'],[23,'male'])

```

### 上面这句相当于创建了这部分，也就是值的部分：

<img width="364" height="286" alt="image" src="https://github.com/user-attachments/assets/718dbd0d-acde-4fb4-9012-ffa5695eac78" />

```
v = np.array([[53,'female'],[64,'male'],[23,'male']])
i = ['1','2','3']
c = ['age','gender']
df = pd.DataFrame(v,index=i,columns=c)
print(df)

```
<img width="183" height="106" alt="image" src="https://github.com/user-attachments/assets/2cff5d63-6cff-47cc-8040-b820b1051e4d" />
<img width="1497" height="215" alt="image" src="https://github.com/user-attachments/assets/3994075b-005e-41de-a7bf-f4142cac4675" />

### 上一个例子不引入numpy也行，此处引入只是为了说明上面这个结论

## 一.（4）二维对象的属性----values index columns

![Uploading image.png…]()
