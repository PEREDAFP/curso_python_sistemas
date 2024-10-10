# Soluciones: Ejercicios de Listas en Python

1. Crear una lista con los números del 1 al 5:
   ```python
   lista = [1, 2, 3, 4, 5]
   print(lista)
   ```

2. Añadir el número 6:
   ```python
   lista.append(6)
   print(lista)
   ```

3. Acceder al tercer elemento:
   ```python
   print(lista[2])
   ```

4. Modificar el segundo elemento:
   ```python
   lista[1] = 10
   print(lista)
   ```

5. Eliminar el último elemento:
   ```python
   lista.pop()
   print(lista)
   ```

6. Ordenar lista de colores:
   ```python
   colores = ["rojo", "azul", "verde"]
   colores.sort()
   print(colores)
   ```

7. Concatenar dos listas:
   ```python
   lista1 = [1, 2, 3]
   lista2 = [4, 5, 6]
   lista3 = lista1 + lista2
   print(lista3)
   ```

8. Encontrar índice:
   ```python
   lista = [1, 2, 3, 4, 3, 5]
   print(lista.index(3))
   ```

9. Contar ocurrencias:
   ```python
   lista = [1, 2, 3, 4, 3, 5]
   print(lista.count(3))
   ```

10. Invertir lista:
    ```python
    lista = [1, 2, 3, 4, 5]
    lista = lista[::-1]
    print(lista)
    ```

11. Slicing:
    ```python
    lista = [1, 2, 3, 4, 5]
    print(lista[1:4])
    ```

12. Copiar lista:
    ```python
    original = [1, 2, 3, 4, 5]
    copia = original[:]
    print(copia)
    ```

13. Eliminar todos los elementos:
    ```python
    lista = [1, 2, 3, 4, 5]
    del lista[:]
    print(lista)
    ```

14. Verificar si un elemento está en la lista:
    ```python
    lista = [1, 2, 3, 4, 6]
    print(5 in lista)
    ```

15. Comprensión de listas:
    ```python
    cuadrados = [x**2 for x in range(1, 6)]
    print(cuadrados)
    ```

16. Lista de números pares:
    ```python
    lista = [1, 2, 3, 4, 5, 6]
    pares = [x for x in lista if x % 2 == 0]
    print(pares)
    ```

17. Encontrar el número más grande:
    ```python
    lista = [1, 5, 3, 9, 2]
    maximo = lista[0]
    for num in lista:
        if num > maximo:
            maximo = num
    print(maximo)
    ```

18. Eliminar duplicados:
    ```python
    lista = [1, 2, 2, 3, 4, 3, 5]
    sin_duplicados = list(set(lista))
    print(sin_duplicados)
    ```

19. Crear matriz 3x3:
    ```python
    matriz = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
    print(matriz)
    ```

20. Aplanar matriz:
    ```python
    matriz = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
    aplanada = [num for fila in matriz for num in fila]
    print(aplanada)
    ```