# Diccionarios en Python: Teoría y Ejercicios

## Introducción a los Diccionarios

En Python, un diccionario es una estructura de datos que permite almacenar pares de clave-valor. Los diccionarios son:

- No ordenados (en versiones de Python anteriores a 3.7)
- Mutables: se pueden modificar después de su creación
- Indexados: se accede a los valores mediante claves en lugar de índices numéricos
- No permiten claves duplicadas

## Creación de Diccionarios

Puedes crear un diccionario usando llaves `{}` y separando los pares clave-valor con comas:

```python
mi_diccionario = {"nombre": "Juan", "edad": 30, "ciudad": "Madrid"}
```

## Operaciones Básicas con Diccionarios

1. Acceder a valores:
   ```python
   mi_diccionario["nombre"]  # Devuelve "Juan"
   ```

2. Modificar valores:
   ```python
   mi_diccionario["edad"] = 31
   ```

3. Añadir nuevos pares clave-valor:
   ```python
   mi_diccionario["profesion"] = "Ingeniero"
   ```

4. Eliminar pares clave-valor:
   ```python
   del mi_diccionario["ciudad"]
   ```

5. Verificar si una clave existe:
   ```python
   "nombre" in mi_diccionario  # Devuelve True
   ```

6. Obtener todas las claves y valores:
   ```python
   mi_diccionario.keys()
   mi_diccionario.values()
   mi_diccionario.items()
   ```

7. Métodos útiles:
   - `get()`: Obtiene un valor con una clave predeterminada si no existe
   - `update()`: Actualiza el diccionario con otro diccionario o pares clave-valor
   - `pop()`: Elimina y devuelve un valor para una clave específica
   - `clear()`: Elimina todos los elementos del diccionario

## Ejercicios

1. Crea un diccionario llamado `persona` con las claves "nombre", "edad" y "ciudad", y asígnales valores.

2. Accede e imprime el valor asociado con la clave "nombre" del diccionario `persona`.

3. Añade una nueva clave-valor al diccionario `persona` para representar la "profesion".

4. Modifica el valor de "edad" en el diccionario `persona`.

5. Elimina la clave "ciudad" del diccionario `persona`.

6. Verifica si la clave "apellido" existe en el diccionario `persona`.

7. Utiliza el método `get()` para obtener el valor de "edad", y si no existe, que devuelva 0.

8. Crea un diccionario llamado `calificaciones` con asignaturas como claves y notas como valores. Luego, calcula el promedio de las calificaciones.

9. Utiliza un bucle para imprimir todas las claves del diccionario `persona`.

10. Crea una función que reciba un diccionario y una clave, y devuelva el valor asociado a esa clave si existe, o None si no existe.

11. Combina dos diccionarios en uno solo utilizando el método `update()`.

12. Crea un diccionario a partir de dos listas, una de claves y otra de valores.

13. Cuenta cuántas veces aparece cada carácter en una cadena utilizando un diccionario.

14. Crea un diccionario donde las claves sean números del 1 al 5 y los valores sean sus cuadrados.

15. Invierte un diccionario, es decir, crea un nuevo diccionario donde las claves sean los valores del diccionario original y viceversa.

16. Crea un diccionario anidado para representar información de libros (título, autor, año) y accede a un valor específico.

17. Elimina todas las claves de un diccionario que tengan valores nulos (None).

18. Fusiona dos diccionarios y suma los valores de las claves que se repiten.

19. Crea una función que reciba un diccionario y devuelva una lista de tuplas (clave, valor) ordenadas por la longitud de la clave.

20. Implementa un pequeño sistema de gestión de inventario usando diccionarios, con funciones para añadir productos, actualizar cantidades y mostrar el inventario.

¡Intenta resolver estos ejercicios por tu cuenta! Las soluciones están disponibles en un documento separado para que puedas verificar tus respuestas después de intentar resolverlos.