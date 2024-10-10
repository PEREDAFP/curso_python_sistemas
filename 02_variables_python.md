# Variables en Python: Identificación, Creación y Asignación

## Introducción

En Python, las variables son contenedores para almacenar datos. Python es un lenguaje de tipado dinámico, lo que significa que no necesitas declarar el tipo de una variable antes de usarla. El tipo se determina automáticamente en tiempo de ejecución.

## Identificación de Variables

Python identifica las variables por su nombre. Hay algunas reglas y convenciones importantes a seguir:

1. Los nombres de variables pueden contener letras (a-z, A-Z), números (0-9) y guiones bajos (_).
2. Los nombres de variables deben comenzar con una letra o un guión bajo, nunca con un número.
3. Los nombres de variables son sensibles a mayúsculas y minúsculas (age, Age y AGE son tres variables diferentes).
4. Los nombres de variables no pueden ser palabras reservadas de Python (como `if`, `for`, `while`, etc.).

### Convenciones de Nombrado

- Usa nombres descriptivos (por ejemplo, `edad` en lugar de `e`).
- Para variables con múltiples palabras, usa guiones bajos (snake_case): `mi_variable`.
- Las constantes suelen escribirse en mayúsculas: `PI = 3.14159`.

## Creación y Asignación de Variables

En Python, las variables se crean en el momento en que les asignas un valor. No es necesario declararlas previamente.

### Sintaxis Básica

```python
nombre_variable = valor
```

### Ejemplos

```python
# Asignación de diferentes tipos de datos
edad = 25                  # Entero
altura = 1.75              # Flotante
nombre = "Ana"             # Cadena de texto
es_estudiante = True       # Booleano

# Asignación múltiple
x, y, z = 1, 2, 3

# Asignación del mismo valor a múltiples variables
a = b = c = 0
```

## Tipos de Datos en Python

Python determina automáticamente el tipo de dato de una variable según el valor asignado:

- `int`: Números enteros
- `float`: Números decimales
- `str`: Cadenas de texto
- `bool`: Valores booleanos (True o False)
- `list`: Listas
- `tuple`: Tuplas
- `dict`: Diccionarios
- `set`: Conjuntos

### Verificación de Tipos

Puedes usar la función `type()` para verificar el tipo de una variable:

```python
edad = 25
print(type(edad))  # Salida: <class 'int'>

nombre = "Ana"
print(type(nombre))  # Salida: <class 'str'>
```

## Reasignación de Variables

En Python, puedes cambiar el valor y el tipo de una variable en cualquier momento:

```python
x = 5
print(x)  # Salida: 5

x = "Hola"
print(x)  # Salida: Hola
```

## Variables y Memoria

Cuando asignas un valor a una variable, Python crea un objeto en memoria para almacenar ese valor y hace que la variable apunte a ese objeto.

```python
a = 5
b = a  # 'b' apunta al mismo objeto que 'a'

a = 10  # 'a' ahora apunta a un nuevo objeto
print(a)  # Salida: 10
print(b)  # Salida: 5 (b sigue apuntando al objeto original)
```

## Ejercicios Prácticos

1. Crea variables para almacenar tu nombre, edad y ciudad de residencia. Luego, imprime una frase usando estas variables.

```python
nombre = "Carlos"
edad = 30
ciudad = "Madrid"
print(f"Me llamo {nombre}, tengo {edad} años y vivo en {ciudad}.")
```

2. Asigna un valor a una variable y luego reasígnala con un tipo de dato diferente.

```python
variable = 10
print(type(variable))  # Salida: <class 'int'>

variable = "Ahora soy un string"
print(type(variable))  # Salida: <class 'str'>
```

3. Crea dos variables numéricas y realiza operaciones básicas (suma, resta, multiplicación, división).

```python
num1 = 15
num2 = 4

suma = num1 + num2
resta = num1 - num2
multiplicacion = num1 * num2
division = num1 / num2

print(f"Suma: {suma}, Resta: {resta}, Multiplicación: {multiplicacion}, División: {division}")
```

Estos ejercicios te ayudarán a practicar la creación y manipulación de variables en Python. Recuerda que la práctica constante es clave para dominar estos conceptos fundamentales.