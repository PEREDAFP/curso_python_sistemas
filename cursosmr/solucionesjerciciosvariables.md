# **Soluciones Detalladas a los 50 Ejercicios de Python**

## **Ejercicios Básicos (1-10)**

### **1. Declara una variable `nombre` con tu nombre y imprímela.**

```python
nombre = "Carlos"
print(nombre)
```

**Explicación**:

- Creamos una variable `nombre` que almacena un string.
- `print()` muestra el valor de la variable.

---

### **2. Crea dos variables `a` y `b`, asígnales valores y muestra su suma.**

```python
a = 5
b = 3
suma = a + b
print(suma)  # Salida: 8
```

**Explicación**:

- Operación aritmética básica con variables.

---

### **3. Concatena dos cadenas `cadena1 = "Hola"` y `cadena2 = "Python"`.**

```python
cadena1 = "Hola"
cadena2 = "Python"
resultado = cadena1 + " " + cadena2
print(resultado)  # Salida: Hola Python
```

**Explicación**:

- El operador `+` concatena strings.

---

### **4. Convierte un número entero a flotante.**

```python
entero = 7
flotante = float(entero)
print(flotante)  # Salida: 7.0
```

**Explicación**:

- `float()` convierte un entero a flotante.

---

### **5. Usa `type()` para verificar el tipo de una variable.**

```python
x = 10.5
print(type(x))  # Salida: <class 'float'>
```

**Explicación**:

- `type()` devuelve el tipo de dato de la variable.

---

### **6. Declara una lista con tres elementos e imprímela.**

```python
lista = [10, "Python", True]
print(lista)  # Salida: [10, 'Python', True]
```

**Explicación**:

- Las listas pueden contener diferentes tipos de datos.

---

### **7. Añade un elemento a una lista existente.**

```python
lista = [1, 2, 3]
lista.append(4)
print(lista)  # Salida: [1, 2, 3, 4]
```

**Explicación**:

- `append()` añade un elemento al final de la lista.

---

### **8. Crea una tupla con tres elementos.**

```python
tupla = (1, "A", 3.5)
print(tupla)  # Salida: (1, 'A', 3.5)
```

**Explicación**:

- Las tuplas son inmutables y se definen con paréntesis.

---

### **9. Accede al segundo elemento de una lista.**

```python
lista = [10, 20, 30]
print(lista[1])  # Salida: 20
```

**Explicación**:

- Los índices en Python comienzan en 0.

---

### **10. Declara un diccionario con dos pares clave-valor.**

```python
diccionario = {"nombre": "Ana", "edad": 25}
print(diccionario)  # Salida: {'nombre': 'Ana', 'edad': 25}
```

**Explicación**:

- Los diccionarios almacenan datos en pares `clave: valor`.

---

## **Ejercicios Intermedios (11-30)**

### **11. Calcula el promedio de una lista de números.**

```python
numeros = [5, 10, 15]
promedio = sum(numeros) / len(numeros)
print(promedio)  # Salida: 10.0
```

**Explicación**:

- `sum()` suma los elementos, `len()` cuenta los elementos.

---

### **12. Suma todos los elementos de una lista.**

```python
lista = [1, 2, 3, 4]
total = sum(lista)
print(total)  # Salida: 10
```

---

### **13. Multiplica todos los elementos de una lista por 2.**

```python
lista = [1, 2, 3]
resultado = [x * 2 for x in lista]
print(resultado)  # Salida: [2, 4, 6]
```

**Explicación**:

- Comprensión de listas para operaciones en cada elemento.

---

### **14. Filtra los números pares de una lista.**

```python
numeros = [1, 2, 3, 4, 5]
pares = [x for x in numeros if x % 2 == 0]
print(pares)  # Salida: [2, 4]
```

---

### **15. Combina dos listas en una sola.**

```python
lista1 = [1, 2]
lista2 = [3, 4]
combinada = lista1 + lista2
print(combinada)  # Salida: [1, 2, 3, 4]
```

---

### **16. Invierte el orden de una lista.**

```python
lista = [1, 2, 3]
lista.reverse()
print(lista)  # Salida: [3, 2, 1]
```

---

### **17. Cuenta las veces que aparece un elemento en una lista.**

```python
lista = [1, 2, 2, 3]
print(lista.count(2))  # Salida: 2
```

---

### **18. Ordena una lista de números.**

```python
numeros = [3, 1, 4, 2]
numeros.sort()
print(numeros)  # Salida: [1, 2, 3, 4]
```

---

### **19. Convierte una lista en una tupla.**

```python
lista = [1, 2, 3]
tupla = tuple(lista)
print(tupla)  # Salida: (1, 2, 3)
```

---

### **20. Convierte una tupla en una lista.**

```python
tupla = (1, 2, 3)
lista = list(tupla)
print(lista)  # Salida: [1, 2, 3]
```

---

### **21. Extrae las claves de un diccionario**

```python
diccionario = {"a": 1, "b": 2}
claves = diccionario.keys()
print(list(claves))  # Salida: ['a', 'b']
```

**Explicación**:

- `.keys()` devuelve un objeto de vista con las claves del diccionario. Convertimos a lista para mejor visualización.

---

### **22. Extrae los valores de un diccionario**

```python
diccionario = {"a": 1, "b": 2}
valores = diccionario.values()
print(list(valores))  # Salida: [1, 2]
```

---

### **23. Comprueba si una clave existe en un diccionario**

```python
diccionario = {"nombre": "Ana", "edad": 25}
print("nombre" in diccionario)  # Salida: True
```

---

### **24. Elimina un elemento de un diccionario**

```python
diccionario = {"a": 1, "b": 2}
del diccionario["a"]
print(diccionario)  # Salida: {'b': 2}
```

---

### **25. Lista de diccionarios (estudiantes)**

```python
estudiantes = [
    {"nombre": "Ana", "edad": 20},
    {"nombre": "Luis", "edad": 22}
]
print(estudiantes[1]["nombre"])  # Salida: Luis
```

---

### **26. Suma los valores de un diccionario**

```python
diccionario = {"a": 10, "b": 20}
suma = sum(diccionario.values())
print(suma)  # Salida: 30
```

---

### **27. Encuentra el valor máximo en una lista**

```python
lista = [5, 2, 8, 1]
maximo = max(lista)
print(maximo)  # Salida: 8
```

---

### **28. Encuentra el valor mínimo en una lista**

```python
lista = [5, 2, 8, 1]
minimo = min(lista)
print(minimo)  # Salida: 1
```

---

### **29. Lista con números del 1 al 10 usando `range()`**

```python
numeros = list(range(1, 11))
print(numeros)  # Salida: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```

---

### **30. Lista con números pares del 2 al 20**

```python
pares = list(range(2, 21, 2))
print(pares)  # Salida: [2, 4, 6, 8, 10, 12, 14, 16, 18, 20]
```

---

### **36. Combina dos diccionarios en uno**

```python
dic1 = {"a": 1}
dic2 = {"b": 2}
combinado = {**dic1, **dic2}
print(combinado)  # Salida: {'a': 1, 'b': 2}
```

---

### **37. Ordena un diccionario por sus valores**

```python
diccionario = {"a": 3, "b": 1, "c": 2}
ordenado = dict(sorted(diccionario.items(), key=lambda item: item[1]))
print(ordenado)  # Salida: {'b': 1, 'c': 2, 'a': 3}
```

---

### **38. Intersección entre dos listas**

```python
lista1 = [1, 2, 3]
lista2 = [2, 3, 4]
interseccion = list(set(lista1) & set(lista2))
print(interseccion)  # Salida: [2, 3]
```

---

### **39. Elimina elementos duplicados de una lista**

```python
lista = [1, 2, 2, 3]
sin_duplicados = list(set(lista))
print(sin_duplicados)  # Salida: [1, 2, 3]
```

---

### **40. Matriz (lista de listas) y acceso a un elemento**

```python
matriz = [[1, 2], [3, 4]]
print(matriz[1][0])  # Salida: 3 (fila 1, columna 0)
```

---

### **41. Suma los elementos de una matriz**

```python
matriz = [[1, 2], [3, 4]]
suma = sum(sum(fila) for fila in matriz)
print(suma)  # Salida: 10
```

---

### **42. Transpone una matriz (filas ↔ columnas)**

```python
matriz = [[1, 2], [3, 4]]
transpuesta = list(zip(*matriz))
print(transpuesta)  # Salida: [(1, 3), (2, 4)]
```

---

### **43. Convierte una cadena a mayúsculas**

```python
cadena = "hola"
print(cadena.upper())  # Salida: "HOLA"
```

---

### **44. Divide una cadena usando un delimitador**

```python
cadena = "a,b,c"
lista = cadena.split(",")
print(lista)  # Salida: ['a', 'b', 'c']
```

---

### **45. Reemplaza una palabra en una cadena**

```python
cadena = "Hola mundo"
nueva = cadena.replace("mundo", "Python")
print(nueva)  # Salida: "Hola Python"
```

---

### **46. Comprueba si una cadena es palíndromo**

```python
cadena = "reconocer"
es_palindromo = cadena == cadena[::-1]
print(es_palindromo)  # Salida: True
```

---

### **47. Función para calcular el factorial de un número**

```python
def factorial(n):
    return 1 if n == 0 else n * factorial(n-1)

print(factorial(5))  # Salida: 120
```

---

### **48. Búsqueda lineal en una lista**

```python
def busqueda_lineal(lista, objetivo):
    for i, item in enumerate(lista):
        if item == objetivo:
            return i
    return -1

lista = [5, 2, 8, 1]
print(busqueda_lineal(lista, 8))  # Salida: 2 (índice)
```

---

### **49. Búsqueda binaria en una lista ordenada**

```python
def busqueda_binaria(lista, objetivo):
    izquierda, derecha = 0, len(lista) - 1
    while izquierda <= derecha:
        medio = (izquierda + derecha) // 2
        if lista[medio] == objetivo:
            return medio
        elif lista[medio] < objetivo:
            izquierda = medio + 1
        else:
            derecha = medio - 1
    return -1

lista_ordenada = [1, 2, 3, 4, 5]
print(busqueda_binaria(lista_ordenada, 3))  # Salida: 2
```

---
