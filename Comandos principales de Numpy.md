## A) NumPy – Creación y manipulación de arreglos

### Ejemplo 1: Crear un array
```python
import numpy as np
a = np.array([10, 20, 30])
print(a)
```
**Resultado:**
```
[10 20 30]
```
### Ejemplo 2: Usar reshape
```python
b = np.array([1, 2, 3, 4, 5, 6])
b_reshaped = b.reshape((2, 3))
print(b_reshaped)
```
**Resultado:**
```
[[1 2 3]
 [4 5 6]]
```
### Ejemplo 3: Concatenar arreglos
```python
import numpy as np
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
concatenado = np.concatenate((a, b))
print(concatenado)
```
**Resultado:**
```
[1 2 3 4 5 6]
```
### Ejemplo 4: Operaciones básicas
```python
import numpy as np
a = np.array([10, 20, 30])
b = np.array([1, 2, 3])

suma = a + b
multiplicacion = a * 2
print("Suma:", suma)
print("Multiplicación:", multiplicacion)
```
**Resultado:**
```
Suma: [11 22 33]
Multiplicación: [20 40 60]
```

### Ejemplo realizado desde la herramienta Google Colab
<img width="1226" height="770" alt="Captura de pantalla 2025-08-23 184013" src="https://github.com/user-attachments/assets/94e52a56-7c74-47a7-b328-84c7125040cb" />


# B) NumPy – Operaciones estadísticas y funciones avanzadas

###Ejemplo 1: Calcular media, desviación estándar y suma
```python
import numpy as np
datos = np.array([5, 10, 15, 20, 25])
print("Media:", np.mean(datos))
print("Desviación estándar:", np.std(datos))
print("Suma:", np.sum(datos))
```
**Resultado:**
```
Media: 15.0
Desviación estándar: 7.0710678118654755
Suma: 75
```
###Ejemplo 2: Usar arange y linspace
```python
print("Arange:", np.arange(0, 10, 2))
print("Linspace:", np.linspace(0, 1, 5))
```
**Resultado:**
```
Arange: [0 2 4 6 8]
Linspace: [0.   0.25 0.5  0.75 1.  ]
```
###Ejemplo 3: Generar números aleatorios
```python
aleatorios = np.random.rand(3, 2)
print(aleatorios)
```
**Resultado:**
```
[[0.93912605 0.69946397]
 [0.39729219 0.20085467]
 [0.60398808 0.71203604]]
```
###Ejemplo 4: Producto matricial y determinante
```python
A = np.array([[1, 2], [3, 4]])
B = np.array([[2, 0], [1, 2]])
producto = np.dot(A, B)
det_A = np.linalg.det(A)
print("Producto matricial:\n", producto)
print("Determinante de A:", det_A)
```
**Resultado:**
```
Producto matricial:
 [[ 4  4]
 [10  8]]
Determinante de A: -2.0000000000000004
```
<img width="1220" height="749" alt="Captura de pantalla 2025-08-23 185624" src="https://github.com/user-attachments/assets/0861ba7a-bd2f-41f3-907f-3c7f78e7a953" />

