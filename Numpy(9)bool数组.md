 ## 布尔型数组
 
<img width="1329" height="263" alt="image" src="https://github.com/user-attachments/assets/deee793e-4a9e-4df7-9086-ba2379dfbb1a" />

#### 数组与数字比较例程即结果：

```
arr = np.arange(1,7).reshape(2,3)
print(arr)
print(arr>=4)
```
<img width="375" height="128" alt="image" src="https://github.com/user-attachments/assets/1540ea34-58bc-491e-91f5-1bae17ab96e0" />

#### 也可以将同维数组比较：

```
arr1 = np.arange(1,6)
arr2 = np.flipud(arr1)
print(arr1)
print(arr2)
print(arr1>arr2)
```
<img width="372" height="90" alt="image" src="https://github.com/user-attachments/assets/e15720d1-4b34-4483-be31-58fcd210045b" />

## 还可以同时检查多个条件

<img width="1317" height="146" alt="image" src="https://github.com/user-attachments/assets/06057ac8-7450-4e08-a976-45a2abf5b8f4" />

### ❗❗❗Numpy中的与或非是&，|，~  

## 布尔数组中True的数量

## np.sum()：统计布尔数组中true的个数

## np.any()：布尔型数组里有一个true就返回true。

## np.all()：布尔数组里全为true才返回true


<img width="1462" height="153" alt="image" src="https://github.com/user-attachments/assets/cbf00c26-b130-4160-8f55-df3999e40bf4" />

```
arr = np.random.normal(0,1,10000)
num = np.sum(np.abs(arr)<1) #统计正态分布中绝对值小于1的个数
print(num)

```
## 布尔型数组还可作为掩码

```
arr = np.arange(1,13).reshape(3,4)
print(arr)
print(arr>4)
print(arr[arr>4]) #bool数组作为索引
```
### ❗❗❗矩阵进行掩码操作后变为向量

## 满足条件的元素所在位置

## 此时可用np.where()

```
arr = np.random.normal(500,70,1000)
print(np.where(arr>650))
```
<img width="878" height="86" alt="image" src="https://github.com/user-attachments/assets/b267d594-5bf6-44f7-a14a-0649eccc8c9e" />
<img width="434" height="68" alt="image" src="https://github.com/user-attachments/assets/f5de4222-0581-4449-af71-bf202168590d" />

