# **Sesión de Clase: Introducción a Variables y Tipos de Datos en Python**

## **Objetivos de la Clase**

1. Comprender el concepto de variables en Python y su importancia en la legibilidad del código.
2. Conocer los tipos de datos básicos en Python: enteros (`int`), flotantes (`float`), cadenas (`str`), listas (`list`), tuplas (`tuple`) y diccionarios (`dict`).
3. Aprender a realizar operaciones básicas con variables y estructuras de datos.
4. Diferenciar entre mutabilidad e inmutabilidad en estructuras de datos.
5. Practicar el uso del intérprete interactivo de Python y scripts en archivos `.py`.

---

## **Contenido de la Sesión**

### **1. Introducción a las Variables**

- **Definición**: Una variable es un nombre que referencia un valor en memoria.
- **Sintaxis**: `nombre_variable = valor`
- **Reglas para nombrar variables**:
  - No pueden empezar con números.
  - Pueden contener letras, números y guiones bajos (`_`).
  - No se permiten espacios.
  - Es recomendable usar `snake_case` para nombres compuestos (ej: `total_amount`).

**Ejemplo:**

```python
gastado = 3
donado = 4
total_amount = gastado + donado
print(total_amount)  # Salida: 7
```

---

### **2. Tipos de Datos Básicos**

1. **Enteros (`int`)**: Números sin decimales.
   ```python
   edad = 25
   ```
2. **Flotantes (`float`)**: Números con decimales.
   ```python
   temperatura = 36.5
   ```
3. **Cadenas (`str`)**: Texto entre comillas simples o dobles.
   ```python
   nombre = "Ana"
   ```
4. **Listas (`list`)**: Colección ordenada y mutable de elementos.
   ```python
   numeros = [1, 2, 3]
   ```
5. **Tuplas (`tuple`)**: Colección ordenada e inmutable.
   ```python
   coordenadas = (4, 5)
   ```
6. **Diccionarios (`dict`)**: Pares clave-valor.
   ```python
   estudiante = {"nombre": "Juan", "edad": 20}
   ```

---

### **3. Operaciones con Variables**

- **Suma, resta, multiplicación y división**:
  ```python
  a = 10
  b = 2
  print(a + b)  # 12
  print(a * b)  # 20
  ```
- **Concatenación de cadenas**:
  ```python
  saludo = "Hola" + " " + "Mundo"  # "Hola Mundo"
  ```

---

### **4. Estructuras de Datos**

#### **Listas**

- **Creación**:
  ```python
  lista = [1, "dos", 3.0]
  ```
- **Operaciones**:
  ```python
  lista.append(4)      # Añade un elemento al final.
  lista.remove("dos")  # Elimina un elemento.
  ```

#### **Diccionarios**

- **Creación**:
  ```python
  datos = {"clave": "valor"}
  ```
- **Acceso a valores**:
  ```python
  print(datos["clave"])  # "valor"
  ```

---

### **5. Uso del Intérprete Interactivo vs. Scripts**

- **Intérprete interactivo**: Ideal para pruebas rápidas.
  ```python
  >>> x = 10
  >>> x + 5
  15
  ```
- **Scripts en archivos `.py`**: Para programas reutilizables.
  ```python
  # programa.py
  x = 10
  print(x + 5)
  ```

---

## **Ejercicios Propuestos (50 en total)**

### **Ejercicios Básicos (1-10)**

1. Declara una variable `nombre` con tu nombre y imprímela.
2. Crea dos variables `a` y `b`, asígnales valores y muestra su suma.
3. Concatena dos cadenas `cadena1 = "Hola"` y `cadena2 = "Python"`.
4. Convierte un número entero a flotante.
5. Usa `type()` para verificar el tipo de una variable.
6. Declara una lista con tres elementos e imprímela.
7. Añade un elemento a una lista existente.
8. Crea una tupla con tres elementos.
9. Accede al segundo elemento de una lista.
10. Declara un diccionario con dos pares clave-valor.

### **Ejercicios Intermedios (11-30)**

11. Calcula el promedio de una lista de números.
12. Suma todos los elementos de una lista.
13. Multiplica todos los elementos de una lista por 2.
14. Filtra los números pares de una lista.
15. Combina dos listas en una sola.
16. Invierte el orden de una lista.
17. Cuenta las veces que aparece un elemento en una lista.
18. Ordena una lista de números.
19. Convierte una lista en una tupla.
20. Convierte una tupla en una lista.
21. Extrae las claves de un diccionario.
22. Extrae los valores de un diccionario.
23. Comprueba si una clave existe en un diccionario.
24. Elimina un elemento de un diccionario.
25. Crea una lista de diccionarios (ej: lista de estudiantes).
26. Suma los valores de un diccionario.
27. Encuentra el valor máximo en una lista.
28. Encuentra el valor mínimo en una lista.
29. Crea una lista con números del 1 al 10 usando `range()`.
30. Genera una lista con números pares del 2 al 20.

### **Ejercicios Avanzados (31-50)**

31. Convierte una cadena en una lista de palabras.
32. Une una lista de palabras en una cadena.
33. Crea una lista de comprensión que eleve al cuadrado los números del 1 al 10.
34. Filtra los números mayores que 5 en una lista.
35. Crea un diccionario a partir de dos listas (claves y valores).
36. Combina dos diccionarios en uno solo.
37. Ordena un diccionario por sus valores.
38. Encuentra la intersección entre dos listas.
39. Elimina elementos duplicados de una lista.
40. Crea una matriz (lista de listas) y accede a un elemento.
41. Suma los elementos de una matriz.
42. Transpone una matriz (intercambia filas por columnas).
43. Convierte una cadena en mayúsculas.
44. Divide una cadena en una lista usando un delimitador.
45. Reemplaza una palabra en una cadena.
46. Comprueba si una cadena es un palíndromo.
47. Crea una función que calcule el factorial de un número.
48. Implementa una búsqueda lineal en una lista.
49. Implementa una búsqueda binaria en una lista ordenada.
50. Crea un programa que simule un diccionario de traducción (español-inglés).

---
