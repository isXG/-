### 数组的函数

<img width="1415" height="325" alt="image" src="https://github.com/user-attachments/assets/a90f93ce-4eb3-4461-9467-e3bf5da769fb" />

- ❗❗❗混合运算时结果必为向量

<img width="1482" height="223" alt="image" src="https://github.com/user-attachments/assets/d795781f-0ad9-4c29-8893-24c1572215ee" />

- ❗❗❗不能是（1，5）×（5，1）。这里是线代里的矩阵运算，这样样会乘出来矩阵。
- 而根据刚刚学过的，混有向量时候1，运算结果必为向量。
  
 ##### 例程即运行结果：
 
```
import numpy as mp
arr1 = np.arange(5)
arr2 = np.arange(5)
print(arr1)
print(arr2)
print(np.dot(arr1,arr2))
```
<img width="342" height="91" alt="image" src="https://github.com/user-attachments/assets/23d219a1-2a7b-4a10-932c-44d3d893b88a" />


<img width="1455" height="235" alt="image" src="https://github.com/user-attachments/assets/55769f88-fe4f-4e21-b31b-9a0f91a8166d" />

##### 例程即运行结果：

```

arr1 = np.arange(5)
arr2 = np.arange(15).reshape(5,3)
print(arr1)
print(arr2)
print(np.dot(arr1,arr2))

```
<img width="162" height="231" alt="image" src="https://github.com/user-attachments/assets/80b701eb-04e8-41ea-826a-320d9db1432a" />

 -  相当于（1，5）×（5，3）=（1，3），且结果为向量
 -  
 -  <img width="1449" height="225" alt="image" src="https://github.com/user-attachments/assets/a0d9fed3-a200-4360-ad6c-3ad0a5eec66c" />
 
<img width="1422" height="201" alt="image" src="https://github.com/user-attachments/assets/5177e330-86d1-4b1b-a1cd-887c64386384" />

#### 和线代里一模一样不再赘述



