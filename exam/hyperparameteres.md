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
> **l1_ratio** [доля L1-регуляризации], **alphas** [список коэффициентов регуляризации], **cv** [число фолдов для CV], **fit_intercept**,**max_iter**

## MinMaxScaler() 
> **eature_range** [диапазон, обычно (0, 1)], **copy** [копировать ли данные]

## StandardScaler()
> **with_mean** [вычитать ли среднее], **with_std** [делить ли на стандартное отклонение], **copy**

## least_squares()
> **fun** [функция ошибок], **x0** [начальное приближение], **method** ['trf', 'dogbox', 'lm'], **loss** [функция потерь ('linear', 'huber', 'soft_l1')], **bounds**[ограничения на параметры]

## OneHotEncoder() 
## ColumnTransformer()
> **transformers** [список (name, transformer, columns)], **remainder** [что делать с остальными ('drop', 'passthrough')]

## LogisticRegression()
> **penalty** ['l1', 'l2', 'elasticnet', 'none'], **C** [обратная сила регуляризации], **max_iter**

## PCA()
> **n_components** [число компонент или доля дисперсии], **svd_solver** ['auto', 'full', 'randomized'], **random_state**

## KernelPCA()
> **n_components**, **kernel** ['rbf', 'poly', 'sigmoid', 'cosine'], **gamma** [ширина ядра (RBF)], **degree** [степень полинома], **coef0** [смещение ядра], **fit_inverse_transform** [обратное преобразование]

## SVC()
> **C** [штраф за ошибки], **kernel** ['linear', 'rbf', 'poly', 'sigmoid'], **gamma** [радиус влияния точки], **degree** [степень полиномиального ядра], **coef0** [смещение ядра], **max_iter**

## KMeans() 
> **n_clusters**, **init** ['k-means++' или 'random'], **n_init** [число перезапусков], **max_iter**, **random_state**

## DBSCAN() 
> **eps** [радиус соседства], **min_samples** [минимум точек для кластера], **metric** [метрика расстояния], **algorithm** [способ поиска соседей]
