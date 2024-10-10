# Listas en Python: Teoría y Ejercicios

## Introducción a las Listas

En Python, una lista es una estructura de datos que permite almacenar múltiples elementos en un solo contenedor. Las listas son:

- Ordenadas: Los elementos mantienen un orden específico.
- Mutables: Puedes modificar, añadir o eliminar elementos después de crear la lista.
- Capaces de contener elementos duplicados.
- Capaces de contener diferentes tipos de datos.

## Creación de Listas

Puedes crear una lista usando corchetes `[]` y separando los elementos con comas:

```python
mi_lista = [1, 2, 3, 4, 5]
lista_mixta = [1, "dos", 3.0, True]
```

## Operaciones Básicas con Listas

1. Acceder a elementos: Usa índices (empezando desde 0)
   ```python
   mi_lista[0]  # Primer elemento
   mi_lista[-1]  # Último elemento
   ```

2. Modificar elementos:
   ```python
   mi_lista[1] = 10
   ```

3. Añadir elementos:
   ```python
   mi_lista.append(6)  # Añade al final
   mi_lista.insert(0, 0)  # Inserta en una posición específica
   ```

4. Eliminar elementos:
   ```python
   mi_lista.remove(3)  # Elimina el primer 3 que encuentra
   del mi_lista[0]  # Elimina el elemento en el índice 0
   elemento = mi_lista.pop()  # Elimina y retorna el último elemento
   ```

5. Longitud de la lista:
   ```python
   len(mi_lista)
   ```

6. Slicing (rebanar):
   ```python
   mi_lista[1:4]  # Elementos del índice 1 al 3
   mi_lista[::-1]  # Lista invertida
   ```

7. Métodos útiles:
   - `sort()`: Ordena la lista
   - `reverse()`: Invierte el orden de la lista
   - `count()`: Cuenta las ocurrencias de un elemento
   - `index()`: Encuentra el índice de un elemento

## Ejercicios

1. Crea una lista con los números del 1 al 5 y imprime la lista.

2. Añade el número 6 a la lista anterior y vuelve a imprimirla.

3. Accede e imprime el tercer elemento de la lista.

4. Modifica el segundo elemento de la lista y asígnale el valor 10.

5. Elimina el último elemento de la lista usando el método pop().

6. Crea una lista con los nombres de tres colores y ordénala alfabéticamente.

7. Crea dos listas y concaténalas en una tercera lista.

8. Encuentra el índice del número 3 en la lista [1, 2, 3, 4, 3, 5].

9. Cuenta cuántas veces aparece el número 3 en la lista anterior.

10. Invierte el orden de la lista [1, 2, 3, 4, 5] sin usar el método reverse().

11. Crea una lista de números y usa slicing para obtener los elementos del segundo al cuarto.

12. Crea una copia de una lista usando slicing.

13. Elimina todos los elementos de una lista sin usar clear().

14. Verifica si el número 5 está en la lista [1, 2, 3, 4, 6].

15. Crea una lista de cuadrados de los números del 1 al 5 usando comprensión de listas.

16. Dada la lista [1, 2, 3, 4, 5, 6], crea una nueva lista con solo los números pares.

17. Encuentra el número más grande en una lista sin usar la función max().

18. Elimina los elementos duplicados de la lista [1, 2, 2, 3, 4, 3, 5].

19. Crea una lista de listas que represente una matriz 3x3.

20. Aplana la matriz del ejercicio anterior en una sola lista.

¡Intenta resolver estos ejercicios por tu cuenta! Las soluciones están disponibles en un documento separado para que puedas verificar tus respuestas después de intentar resolverlos.