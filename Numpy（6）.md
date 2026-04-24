## 数组的运算
<img width="1347" height="535" alt="image" src="https://github.com/user-attachments/assets/b6dada20-c3a6-46e9-b253-a76efa0c6a42" />

### 例程
```
arr = np.arange(1,9).reshape(2,4)
print(arr+10)
print(arr-10)
print(arr*10)
print(arr/10) //加减乘除
print(arr*2) //平方
print(arr//6)取整
print(arr%6)
```
<img width="1423" height="214" alt="image" src="https://github.com/user-attachments/assets/b0f9b5d7-f48c-432b-9615-fc86d8856ad0" />
### 例程
```
arr1 = np.arange(1,9,-1).reshape(2,4)
arr2 = -arr1
print(arr1)
print(arr2)
```
```
print(arr1 + arr2)
print(arr1 - arr2)
print(arr1*arr2)
print(arr1/arr2)
print(arr1**arr2)
```
- 事实上，数组与系数和数组与数组的运算并无太大差异。
- <img width="1437" height="336" alt="image" src="https://github.com/user-attachments/assets/97ce23fc-d8d8-4522-91ad-81b51576341d" />
<img width="1458" height="261" alt="image" src="https://github.com/user-attachments/assets/7b873567-9930-47ce-afa0-9c953bedd306" />
### 例程即演示结果：
  ```
  import numpy as np
arr1 = np.array([-100,0,100]) //创建一个向量
print(arr1)
arr2 = np.random.random((10,3)) // 创建一个10行三列的随机矩阵
print(arr2)
print(arr1 *arr2) //广播
```
<img width="533" height="575" alt="image" src="https://github.com/user-attachments/assets/b9ccaa11-8720-464e-a223-266f5c4290a3" />
- 分析结果：随机矩阵第一列都乘以了向量的第一个数-100，第二列第三列也是，这就是广播。
#### ❗❗❗向量和矩阵运算时，向量的列数必须和矩阵列数相等才能广播。感性理解：竖着复制了矩阵的列数次。
<img width="1437" height="302" alt="image" src="https://github.com/user-attachments/assets/bc06d0f0-4e53-4aaf-89a0-6c4444bb513e" />
### 列矩阵广播同理，不再赘述。
#### ❗❗❗要求列矩阵的行数必须和矩阵的行数相同。
  


