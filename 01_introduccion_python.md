# Introducción a Python para Estudiantes de Sistemas

## ¿Qué es Python?

Python es un lenguaje de programación de alto nivel, interpretado y de propósito general. Fue creado por Guido van Rossum y lanzado por primera vez en 1991. Python se destaca por su sintaxis clara y legible, lo que lo hace ideal para principiantes y expertos por igual.

## ¿Para qué sirve Python?

Python tiene una amplia gama de aplicaciones:

1. Desarrollo web (con frameworks como Django y Flask)
2. Análisis de datos y ciencia de datos
3. Inteligencia artificial y aprendizaje automático
4. Automatización y scripting
5. Desarrollo de software
6. Internet de las cosas (IoT)
7. Aplicaciones de escritorio
8. Juegos

## Tu primer script en Python

Para escribir tu primer script en Python, sigue estos pasos:

1. Abre tu editor de texto favorito o un entorno de desarrollo integrado (IDE) para Python.
2. Escribe el siguiente código:

```python
print("¡Hola, mundo!")
```

3. Guarda el archivo con un nombre como `hola_mundo.py`.
4. Abre una terminal o línea de comandos.
5. Navega hasta el directorio donde guardaste el archivo.
6. Ejecuta el script escribiendo:

```
python hola_mundo.py
```

7. Verás el mensaje "¡Hola, mundo!" en la pantalla.

¡Felicidades! Has escrito y ejecutado tu primer script en Python.

## Ejercicios y Soluciones

Ahora, vamos a practicar con 20 ejercicios para reforzar los conceptos básicos de Python.

### Ejercicio 1: Variables y tipos de datos
Crea variables para almacenar tu nombre, edad y altura. Luego, imprímelas.

Solución:
```python
nombre = "Juan"
edad = 25
altura = 1.75

print(f"Me llamo {nombre}, tengo {edad} años y mido {altura} metros.")
```

### Ejercicio 2: Operaciones matemáticas
Calcula el área de un rectángulo con base 5 y altura 3.

Solución:
```python
base = 5
altura = 3
area = base * altura

print(f"El área del rectángulo es: {area}")
```

### Ejercicio 3: Strings
Crea una variable con tu nombre completo y muestra sus primeros 3 caracteres.

Solución:
```python
nombre_completo = "Juan Pérez García"
primeros_tres = nombre_completo[:3]

print(f"Los primeros tres caracteres son: {primeros_tres}")
```

### Ejercicio 4: Listas
Crea una lista de tus 3 frutas favoritas y agrega una cuarta al final.

Solución:
```python
frutas = ["manzana", "plátano", "fresa"]
frutas.append("naranja")

print(f"Mis frutas favoritas son: {frutas}")
```

### Ejercicio 5: Diccionarios
Crea un diccionario con información de una persona (nombre, edad, ciudad).

Solución:
```python
persona = {
    "nombre": "María",
    "edad": 30,
    "ciudad": "Barcelona"
}

print(f"Información de la persona: {persona}")
```

### Ejercicio 6: Condicionales
Escribe un programa que determine si un número es par o impar.

Solución:
```python
numero = 7

if numero % 2 == 0:
    print(f"{numero} es par")
else:
    print(f"{numero} es impar")
```

### Ejercicio 7: Bucles - For
Imprime los números del 1 al 10 usando un bucle for.

Solución:
```python
for i in range(1, 11):
    print(i)
```

### Ejercicio 8: Bucles - While
Cuenta regresiva desde 5 hasta 1 usando un bucle while.

Solución:
```python
contador = 5

while contador > 0:
    print(contador)
    contador -= 1

print("¡Despegue!")
```

### Ejercicio 9: Funciones
Crea una función que calcule el cuadrado de un número.

Solución:
```python
def cuadrado(numero):
    return numero ** 2

resultado = cuadrado(4)
print(f"El cuadrado de 4 es: {resultado}")
```

### Ejercicio 10: Listas por comprensión
Crea una lista con los cuadrados de los números del 1 al 5.

Solución:
```python
cuadrados = [x**2 for x in range(1, 6)]
print(f"Los cuadrados son: {cuadrados}")
```

### Ejercicio 11: Manejo de excepciones
Pide al usuario que ingrese un número y maneja la excepción si ingresa texto.

Solución:
```python
try:
    numero = int(input("Ingresa un número: "))
    print(f"Has ingresado: {numero}")
except ValueError:
    print("Error: Debes ingresar un número válido.")
```

### Ejercicio 12: Módulos
Importa el módulo `random` y genera un número aleatorio entre 1 y 10.

Solución:
```python
import random

numero_aleatorio = random.randint(1, 10)
print(f"Número aleatorio: {numero_aleatorio}")
```

### Ejercicio 13: Archivos
Escribe una frase en un archivo de texto y luego léela.

Solución:
```python
# Escribir en el archivo
with open("mi_archivo.txt", "w") as archivo:
    archivo.write("Python es genial")

# Leer del archivo
with open("mi_archivo.txt", "r") as archivo:
    contenido = archivo.read()
    print(f"Contenido del archivo: {contenido}")
```

### Ejercicio 14: Clases
Crea una clase `Rectangulo` con atributos de base y altura, y un método para calcular el área.

Solución:
```python
class Rectangulo:
    def __init__(self, base, altura):
        self.base = base
        self.altura = altura
    
    def calcular_area(self):
        return self.base * self.altura

mi_rectangulo = Rectangulo(5, 3)
print(f"El área del rectángulo es: {mi_rectangulo.calcular_area()}")
```

### Ejercicio 15: Herencia
Crea una clase `Vehiculo` y una subclase `Coche` que herede de ella.

Solución:
```python
class Vehiculo:
    def __init__(self, marca):
        self.marca = marca
    
    def arrancar(self):
        print(f"El vehículo {self.marca} ha arrancado")

class Coche(Vehiculo):
    def tocar_claxon(self):
        print("¡Beep, beep!")

mi_coche = Coche("Toyota")
mi_coche.arrancar()
mi_coche.tocar_claxon()
```

### Ejercicio 16: Manejo de cadenas
Crea una función que cuente cuántas veces aparece una letra en una frase.

Solución:
```python
def contar_letra(frase, letra):
    return frase.lower().count(letra.lower())

resultado = contar_letra("Python es un lenguaje de programación", "a")
print(f"La letra 'a' aparece {resultado} veces")
```

### Ejercicio 17: Tuplas
Crea una tupla con los meses del año y muestra el tercer mes.

Solución:
```python
meses = ("Enero", "Febrero", "Marzo", "Abril", "Mayo", "Junio", "Julio", "Agosto", "Septiembre", "Octubre", "Noviembre", "Diciembre")

print(f"El tercer mes es: {meses[2]}")
```

### Ejercicio 18: Sets
Crea dos sets con números y encuentra su intersección.

Solución:
```python
set1 = {1, 2, 3, 4, 5}
set2 = {4, 5, 6, 7, 8}

interseccion = set1.intersection(set2)
print(f"La intersección es: {interseccion}")
```

### Ejercicio 19: List comprehension con condicional
Crea una lista de números pares del 1 al 20 usando list comprehension.

Solución:
```python
pares = [x for x in range(1, 21) if x % 2 == 0]
print(f"Números pares: {pares}")
```

### Ejercicio 20: Funciones lambda
Usa una función lambda para ordenar una lista de tuplas por el segundo elemento.

Solución:
```python
frutas = [("manzana", 3), ("plátano", 1), ("naranja", 2)]
frutas_ordenadas = sorted(frutas, key=lambda x: x[1])
print(f"Frutas ordenadas por cantidad: {frutas_ordenadas}")
```

Practica y refuerza tus conocimientos básicos de Python. Recuerda experimentar y la resolver problemas.