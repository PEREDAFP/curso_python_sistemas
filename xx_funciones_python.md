### **Funciones en Python**

Las **funciones** en Python son bloques de código reutilizables que permiten dividir un programa en partes más pequeñas y manejables. Estas partes pueden ser llamadas tantas veces como sea necesario, lo que mejora la legibilidad, reduce la redundancia y facilita el mantenimiento del código.

### **1. Definición de Funciones**

En Python, una función se define con la palabra clave `def`, seguida del nombre de la función, los parámetros entre paréntesis (si los hay) y dos puntos `:`. El bloque de código que sigue es el cuerpo de la función, que debe estar indentado.

```python
def nombre_funcion(parametros):
    # Cuerpo de la función
    return valor
```

### **2. Elementos de una función**

- **Nombre de la función**: El identificador que damos a la función, por ejemplo `suma()`.
- **Parámetros (opcionales)**: Son los valores de entrada que recibe la función. Se pasan entre paréntesis tras el nombre de la función.
- **Cuerpo**: Es el conjunto de instrucciones que define lo que hace la función. Debe estar correctamente indentado.
- **Valor de retorno (opcional)**: Es el valor que devuelve la función al final, indicado con la palabra clave `return`.

#### Ejemplo básico:
```python
def suma(a, b):
    resultado = a + b
    return resultado
```

### **3. Llamada a una función**

Para usar una función después de definirla, se la debe **llamar** escribiendo su nombre seguido de los argumentos (si los hay).

```python
resultado = suma(3, 4)  # Llamada a la función
print(resultado)  # Imprime: 7
```

### **4. Tipos de funciones**

#### a) **Funciones sin parámetros y sin valor de retorno**
Son funciones que no reciben datos y no devuelven resultados.

```python
def saludo():
    print("Hola Mundo")
```

#### b) **Funciones con parámetros**
Son funciones que reciben datos, los procesan y pueden devolver un resultado.

```python
def multiplicar(x, y):
    return x * y
```

#### c) **Funciones con valor de retorno**
Devuelven un valor tras ejecutar las instrucciones.

```python
def cuadrado(num):
    return num * num
```

#### d) **Funciones con parámetros por defecto**
Se pueden definir valores predeterminados para los parámetros.

```python
def saludar(nombre="Usuario"):
    print(f"Hola, {nombre}")
```

### **5. Parámetros y Argumentos**

Los **parámetros** son los nombres de las variables dentro de la definición de la función, mientras que los **argumentos** son los valores reales que pasamos a la función cuando la llamamos.

#### Tipos de argumentos:

- **Argumentos posicionales**: Los valores se asignan según el orden en que se pasan.
  
    ```python
    def resta(a, b):
        return a - b

    print(resta(10, 5))  # 10 se asigna a a, 5 a b
    ```

- **Argumentos con nombre (keyword arguments)**: Se asignan explícitamente por nombre.
  
    ```python
    print(resta(b=5, a=10))  # a=10, b=5
    ```

- **Parámetros arbitrarios**: Se puede pasar un número indeterminado de argumentos.

    ```python
    def sumar_todo(*numeros):
        return sum(numeros)

    print(sumar_todo(1, 2, 3, 4))  # 10
    ```

### **6. Variables locales y globales**

- **Variables locales**: Son las variables definidas dentro de una función, accesibles solo desde esa función.
  
    ```python
    def funcion():
        x = 10  # Local
        print(x)
    ```

- **Variables globales**: Son variables definidas fuera de cualquier función, accesibles desde cualquier parte del programa.

    ```python
    x = 10  # Global

    def imprimir_x():
        print(x)  # Accede a la variable global
    ```

### **7. Funciones Lambda**

Las **funciones lambda** son funciones anónimas, pequeñas y rápidas de definir en una sola línea. Se usan principalmente para funciones simples que se pasan como argumento a otras funciones.

```python
doblar = lambda x: x * 2
print(doblar(5))  # Imprime: 10
```

---

## **Ejercicios sobre Funciones en Python**

### **Ejercicio 1: Saludar**
Escribe una función llamada `saludar` que reciba un nombre como parámetro e imprima `"Hola, <nombre>"`.

### **Ejercicio 2: Suma de dos números**
Escribe una función llamada `suma` que reciba dos números como parámetros y devuelva la suma de ambos.

### **Ejercicio 3: Calcular área de un triángulo**
Escribe una función `area_triangulo` que reciba la base y la altura de un triángulo y devuelva su área.

### **Ejercicio 4: Número par o impar**
Escribe una función `es_par` que reciba un número y devuelva `True` si es par o `False` si es impar.

### **Ejercicio 5: Conversión de temperatura**
Escribe una función que convierta grados Celsius a Fahrenheit.

### **Ejercicio 6: Factorial de un número**
Escribe una función que reciba un número y calcule su factorial.

### **Ejercicio 7: Invertir una cadena**
Escribe una función `invertir_cadena` que reciba una cadena y la devuelva invertida.

### **Ejercicio 8: Número mayor**
Escribe una función que reciba tres números y devuelva el mayor de ellos.

### **Ejercicio 9: Contar vocales**
Escribe una función que cuente cuántas vocales hay en una cadena de texto.

### **Ejercicio 10: Lista al cuadrado**
Escribe una función que reciba una lista de números y devuelva una nueva lista con cada número elevado al cuadrado.

### **Ejercicio 11: FizzBuzz**
Escribe una función que imprima los números del 1 al 100, pero para múltiplos de 3 imprima "Fizz", para múltiplos de 5 imprima "Buzz", y para múltiplos de ambos imprima "FizzBuzz".

### **Ejercicio 12: Palíndromo**
Escribe una función que determine si una palabra es un palíndromo (se lee igual hacia adelante que hacia atrás).

### **Ejercicio 13: Suma de una lista**
Escribe una función que reciba una lista de números y devuelva la suma de todos los elementos.

### **Ejercicio 14: Números primos**
Escribe una función que determine si un número es primo.

### **Ejercicio 15: Números Fibonacci**
Escribe una función que devuelva una lista con los primeros `n` números de la secuencia de Fibonacci.

### **Ejercicio 16: Conversión de segundos a horas, minutos y segundos**
Escribe una función que convierta una cantidad de segundos en formato `horas:minutos:segundos`.

### **Ejercicio 17: Descomposición de factores primos**
Escribe una función que reciba un número entero y devuelva sus factores primos.

### **Ejercicio 18: Promedio de una lista**
Escribe una función que reciba una lista de números y devuelva el promedio.

### **Ejercicio 19: Convertir mayúsculas a minúsculas**
Escribe una función que reciba una cadena y la devuelva convertida en minúsculas.

### **Ejercicio 20: Longitud de una cadena**
Escribe una función que reciba una cadena y devuelva su longitud.

### **Ejercicio 21: Intercalar listas**
Escribe una función que reciba dos listas y devuelva una nueva lista con los elementos de ambas listas intercalados.

### **Ejercicio 22: Ordenar una lista**
Escribe una función que reciba una lista de números y la devuelva ordenada de menor a mayor.

### **Ejercicio 23: Calcular potencia**
Escribe una función que reciba dos números, base y exponente, y devuelva la base elevada al exponente.

### **Ejercicio 24: Eliminar duplicados**
Escribe una función que reciba una lista de números y devuelva una nueva lista sin duplicados.

### **Ejercicio 25: Palabras más largas**
Escribe una función que reciba una lista de palabras y devuelva la palabra más larga.

---

## **Soluciones de los ejercicios**

### **Solución 1: Saludar**
```python
def saludar(nombre):
    print(f"Hola, {nombre}")
```

### **Solución 2: Suma de dos números**
```python
def suma(a, b):
    return a + b
```

### **Solución 3: Calcular área de un triángulo**
```python
def area_triangulo(base, altura):
    return (base * altura) / 2
```

### **Solución 4: Número par o impar**
```python
def es_par(numero):
    return numero % 2 == 0
```

### **Solución 5: Conversión de temperatura**
```python
def celsius_a_fahrenheit(celsius):
    return (celsius * 9/5

) + 32
```

### **Solución 6: Factorial de un número**
```python
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n-1)
```

### **Solución 7: Invertir una cadena**
```python
def invertir_cadena(cadena):
    return cadena[::-1]
```

### **Solución 8: Número mayor**
```python
def mayor(a, b, c):
    return max(a, b, c)
```

### **Solución 9: Contar vocales**
```python
def contar_vocales(cadena):
    vocales = "aeiouAEIOU"
    return sum(1 for char in cadena if char in vocales)
```

### **Solución 10: Lista al cuadrado**
```python
def cuadrados(lista):
    return [x**2 for x in lista]
```

### **Solución 11: FizzBuzz**
```python
def fizzbuzz():
    for i in range(1, 101):
        if i % 3 == 0 and i % 5 == 0:
            print("FizzBuzz")
        elif i % 3 == 0:
            print("Fizz")
        elif i % 5 == 0:
            print("Buzz")
        else:
            print(i)
```

### **Solución 12: Palíndromo**
```python
def es_palindromo(palabra):
    return palabra == palabra[::-1]
```

### **Solución 13: Suma de una lista**
```python
def suma_lista(lista):
    return sum(lista)
```

### **Solución 14: Números primos**
```python
def es_primo(n):
    if n <= 1:
        return False
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            return False
    return True
```

### **Solución 15: Números Fibonacci**
```python
def fibonacci(n):
    fibo = [0, 1]
    for i in range(2, n):
        fibo.append(fibo[-1] + fibo[-2])
    return fibo[:n]
```

### **Solución 16: Conversión de segundos a horas, minutos y segundos**
```python
def convertir_segundos(segundos):
    horas = segundos // 3600
    segundos %= 3600
    minutos = segundos // 60
    segundos %= 60
    return f"{horas}:{minutos}:{segundos}"
```

### **Solución 17: Descomposición de factores primos**
```python
def factores_primos(n):
    factores = []
    divisor = 2
    while n > 1:
        while n % divisor == 0:
            factores.append(divisor)
            n //= divisor
        divisor += 1
    return factores
```

### **Solución 18: Promedio de una lista**
```python
def promedio(lista):
    return sum(lista) / len(lista)
```

### **Solución 19: Convertir mayúsculas a minúsculas**
```python
def convertir_minusculas(cadena):
    return cadena.lower()
```

### **Solución 20: Longitud de una cadena**
```python
def longitud_cadena(cadena):
    return len(cadena)
```

### **Solución 21: Intercalar listas**
```python
def intercalar_listas(lista1, lista2):
    return [elem for par in zip(lista1, lista2) for elem in par]
```

### **Solución 22: Ordenar una lista**
```python
def ordenar_lista(lista):
    return sorted(lista)
```

### **Solución 23: Calcular potencia**
```python
def potencia(base, exponente):
    return base ** exponente
```

### **Solución 24: Eliminar duplicados**
```python
def eliminar_duplicados(lista):
    return list(set(lista))
```

### **Solución 25: Palabras más largas**
```python
def palabra_mas_larga(lista_palabras):
    return max(lista_palabras, key=len)
```

---

