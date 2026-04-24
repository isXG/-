## 数学函数
<img width="1459" height="155" alt="image" src="https://github.com/user-attachments/assets/d550c6c2-b2af-4a58-bb6f-9ced64f0195a" />

## 1️⃣绝对值函数np.abs()

#### 例程即结果：

```
arr_v = np.array([-10,0,10])
abs_v = np.abs(arr_v)
print("原数组是：",arr_v)
print("加上绝对值后：",abs_v)
```
<img width="432" height="72" alt="image" src="https://github.com/user-attachments/assets/617d886f-aef7-4c11-a58a-fd5ec239ba1d" />

## 2️⃣三角函数np.sin(),np.cos(),np.tan()

#### 例程即结果：

```
theta = np.arange(3)*np.pi/2
sin_v = np.sin(theta)
cos_v = np.cos(theta)
tan_v = np.tan(theta)
print(sin_v)
print(cos_v)
print(tan_v)
#np.pi代表常量Π
```
<img width="594" height="101" alt="image" src="https://github.com/user-attachments/assets/268fe8f7-0f3f-4a63-bc3a-69a22e8da9f1" /> 

## 3️⃣ 指数函数①表示e的x次方：使用np.exp(x)②其余用 a**x

#### 例程即结果：

```
x = np.arange(1,4)
print("x是：",x)
print("e的x次幂是：",np.exp(x))
print("2的x次幂是：",2**x)
```
<img width="591" height="86" alt="image" src="https://github.com/user-attachments/assets/1ab9ff96-8660-409f-9651-b354a891f1b7" />

## 4️⃣对数函数np.log()

### 换底公式

<img width="260" height="117" alt="image" src="https://github.com/user-attachments/assets/12f09d1f-061c-4af0-bf4d-d04ddd11c7a3" />

#### 例程即结果：

```
x = np.array([1,10,100,1000])
print("x =",x)
print("log(x) =",np.log(x))
print("log10(x) =",np.log(x)/np.log(10))
```

<img width="614" height="107" alt="image" src="https://github.com/user-attachments/assets/2f0bfc9a-f8a9-4f07-a093-c29b4cfcb6ed" />

## 5️⃣聚合函数

<img width="1351" height="153" alt="image" src="https://github.com/user-attachments/assets/60693be5-666c-4b0e-bdb5-5d88413cafef" />

### ①最大值函数np.max()与最小值函数np.min() 

<img width="1122" height="805" alt="image" src="https://github.com/user-attachments/assets/716b24d0-9a4a-4aca-9cf3-d27769e6921d" />

#### axis = 0,表示按列去比较，输出最大值。axis = 1代表按行比较，输出最大值。

#### 不要axis代表求整体最大值

### 求和和求积函数

<img width="1155" height="548" alt="image" src="https://github.com/user-attachments/assets/06209a02-60c2-4981-9685-3bfe302e6a36" />

### 均值和标准差函数

<img width="1362" height="555" alt="image" src="https://github.com/user-attachments/assets/e3a5d336-05c0-48a5-95f0-d8c2bec262cf" />
<img width="1351" height="233" alt="image" src="https://github.com/user-attachments/assets/9a61b8fc-5f16-459d-b80a-70f3ca6b4948" />





