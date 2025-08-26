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


