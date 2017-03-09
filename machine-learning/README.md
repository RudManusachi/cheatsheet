Machine Learning Հուշաթերթիկ
----------------

# NumPy: Numerical Python

Հիմնական փաթեթներից մէկը գիտնական օգտագործման համար

Փաթեթը ներմուծելու համար
```python
import numpy
```
սովորաբար կարճ անունով ներմուծելու

```python
import numpy as np
```
## Array

### Ստեղծել
#### դատարկ զանգուած # երկարությամբ
```python
numpy.empty(0)
numpy.empty(10)
```
#### զրո արժեքով զանգուած ստեղծել # երկարությամբ
```python
numpy.zeros(0)
numpy.zeros(10)
```
#### նոյն կերպով մէկ արժեքով զանգուած
```python
numpy.ones(10)
```
### սկզբնարժեքաված զանգուած
#### միաչափ զանգուած
```python
numpy.array([1, 2, 3])
```
պատահական թվերով a ից b միջակայքից, # չափ

```python
a=1
b=5
numpy.random.uniform(a, b, 5)
```

#### երկու չափանի
```python
numpy.array([[1, 2], [3, 4]])
```
պատահական թվերով a ից b միջակայքից, [#տող, #սյուն ]

```python
a=1
b=5
numpy.random.uniform(a, b, [2,4])
```

### Հատկություններ
#### Չափ
```python
a = numpy.array([[1, 2], [3, 4]])
a.size
```
####մատրից տեղափոխել (Transpose)
```python
A= numpy.random.uniform(0,100,[2, 4])
A.T
```

#### Scalar արտադրանքը
վեկտորները պէտքէ իրար համապատասխան չափ ունենան
```python
a= numpy.random.uniform(0, 100, 5)
b= numpy.random.uniform(0, 100, 5)
numpy.inner(a, b)
```

####մատրից բազմապատկում
մատրիցները պէտքէ բավարարեն մատրից բազմապատկման չափսերի կանոնը: nxm * mxr = nxr
```python
A= numpy.random.uniform(0,100,[5, 2])
B= numpy.random.uniform(0,100,[2, 4])
numpy.matmul(A, B)
```
