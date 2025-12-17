# Гиперпараметры основных штук в python, которые мы использовали

## LinearRegression() 
``` python
from sklearn.linear_model import LinearRegression
```
> **fit_intercept**=True [свободный член в модели] , **copy_X**=True [нужно ли копировать данные перед обучением], **n_jobs**=None [количество ядер CPU для параллельных вычислений], **positive**=False [заставляет все коэффициенты быть неотрицательными]

 ##  PolynomialFeatures()
 ```python
 from sklearn.preprocessing import PolynomialFeatures
 ```
> **degree** [степень полиномиальных функций], **include_bias** [если установлено True, включается столбец смещения (столбцец из единиц)], **interaction_only** [только ли взаимодействия генерируются, или степени отдельных функций тоже]

## LassoCV()
> **fit_intercept**, **alphas** [диапазон значений регуляризации, которые пытается найти модель], **cv** [количество фолдов в кросс-валидации], **max_iter**  [максимальное количество итераций]

## ElasticNetCV() 
## MinMaxScaler() StandardScaler()
## least_squares()
## OneHotEncoder() ColumnTransformer()
## LogisticRegression()
## PCA() KernelPCA()
## SVC()
## KMeans() 
## DBSCAN() 
