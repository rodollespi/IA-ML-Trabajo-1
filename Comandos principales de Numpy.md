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
# Datasheet: NumPy y Pandas para Ciencia de Datos

## Sección C – Pandas: Creación y manipulación de DataFrames y Series

Esta sección cubre los comandos principales de Pandas para crear y manipular DataFrames y Series, mostrando ejemplos ejecutados en Google Colab con los resultados incluidos.

---

### 1. Creación de un DataFrame

```python
import pandas as pd

# Crear un DataFrame desde un diccionario
data = {'Nombre': ['Julia', 'Miguel', 'Andrea'],
        'Edad': [28, 34, 22],
        'Ciudad': ['Madrid', 'Buenos Aires', 'Montevideo']}

df = pd.DataFrame(data)
print(df)
```

**Resultado:**
```
   Nombre  Edad        Ciudad
0   Julia    28        Madrid
1  Miguel    34  Buenos Aires
2  Andrea    22    Montevideo
```

---

### 2. Creación de una Serie

```python
# Crear una Serie desde una lista
edades = pd.Series([28, 34, 22], name='Edad')
print(edades)
```

**Resultado:**
```
0    28
1    34
2    22
Name: Edad, dtype: int64
```

---

### 3. Carga de datos desde un archivo CSV

```python
# Supongamos que tenemos un archivo 'personas_actualizadas.csv' con datos
df_csv = pd.read_csv('personas_actualizadas.csv')
print(df_csv.head())
```

**Resultado:**
```
   Nombre  Edad        Ciudad
0   Julia    28        Madrid
1  Miguel    34  Buenos Aires
2  Andrea    22    Montevideo
3   Carla    30       Quito
4   Bruno    26      Caracas
```

---


### 4. Selección de columnas

```python
# Seleccionar la columna 'Nombre'
nombres = df['Nombre']
print(nombres)
```

**Resultado:**
```
0     Julia
1    Miguel
2    Andrea
Name: Nombre, dtype: object
```

---

### 5. Visualizar tipos de datos (dtypes) y primeras filas (head)

```python
print(df.dtypes)
print(df.head(2))
```

**Resultado:**
```
Nombre     object
Edad        int64
Ciudad     object
dtype: object
   Nombre  Edad      Ciudad
0   Julia    28      Madrid
1  Miguel    34  Buenos Aires
```

---

### 6. Selección condicional de filas

```python
# Filtrar personas mayores de 30 años
mayores_30 = df[df['Edad'] > 30]
print(mayores_30)
```

**Resultado:**
```
   Nombre  Edad        Ciudad
1  Miguel    34  Buenos Aires
```

---

**Referencias:**  
- [Documentación oficial de Pandas](https://pandas.pydata.org/docs/)
- Ejecuciones realizadas en [Google Colab](https://colab.research.google.com/)


----


<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/3039511b-f7c8-453a-a41c-16f4bb6a0b3b" />

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/a54bdd56-773e-4bcc-ae84-60abe32dda24" />

<img width="1920" height="1020" alt="image" src="https://github.com/user-attachments/assets/9362a1aa-d6f4-4185-aea8-ba959e7f342f" />



---




