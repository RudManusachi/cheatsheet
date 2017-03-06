Machine Learning Շպարգալկա
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

#### երկու չափանի
```python
numpy.array([[1, 2], [3, 4]])
```

### Հատկություններ
#### Չափ
```python
a = numpy.array([[1, 2], [3, 4]])
a.size
```
