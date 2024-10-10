# Soluciones: Ejercicios de Diccionarios en Python

1. Crear un diccionario `persona`:
   ```python
   persona = {"nombre": "Ana", "edad": 28, "ciudad": "Barcelona"}
   ```

2. Acceder al valor de "nombre":
   ```python
   print(persona["nombre"])
   ```

3. Añadir "profesion":
   ```python
   persona["profesion"] = "Ingeniera"
   ```

4. Modificar "edad":
   ```python
   persona["edad"] = 29
   ```

5. Eliminar "ciudad":
   ```python
   del persona["ciudad"]
   ```

6. Verificar si existe "apellido":
   ```python
   print("apellido" in persona)
   ```

7. Usar `get()` para "edad":
   ```python
   edad = persona.get("edad", 0)
   print(edad)
   ```

8. Calcular promedio de calificaciones:
   ```python
   calificaciones = {"Matemáticas": 85, "Historia": 92, "Ciencias": 78}
   promedio = sum(calificaciones.values()) / len(calificaciones)
   print(f"El promedio es: {promedio}")
   ```

9. Imprimir claves de `persona`:
   ```python
   for clave in persona.keys():
       print(clave)
   ```

10. Función para obtener valor de una clave:
    ```python
    def obtener_valor(diccionario, clave):
        return diccionario.get(clave)
    ```

11. Combinar dos diccionarios:
    ```python
    dict1 = {"a": 1, "b": 2}
    dict2 = {"c": 3, "d": 4}
    dict1.update(dict2)
    print(dict1)
    ```

12. Crear diccionario de dos listas:
    ```python
    claves = ["a", "b", "c"]
    valores = [1, 2, 3]
    nuevo_dict = dict(zip(claves, valores))
    print(nuevo_dict)
    ```

13. Contar caracteres en una cadena:
    ```python
    texto = "hola mundo"
    conteo = {}
    for char in texto:
        conteo[char] = conteo.get(char, 0) + 1
    print(conteo)
    ```

14. Diccionario de cuadrados:
    ```python
    cuadrados = {x: x**2 for x in range(1, 6)}
    print(cuadrados)
    ```

15. Invertir un diccionario:
    ```python
    original = {"a": 1, "b": 2, "c": 3}
    invertido = {v: k for k, v in original.items()}
    print(invertido)
    ```

16. Diccionario anidado de libros:
    ```python
    libros = {
        "1984": {"autor": "George Orwell", "año": 1949},
        "Cien años de soledad": {"autor": "Gabriel García Márquez", "año": 1967}
    }
    print(libros["1984"]["autor"])
    ```

17. Eliminar claves con valores nulos:
    ```python
    diccionario = {"a": 1, "b": None, "c": 3, "d": None}
    limpio = {k: v for k, v in diccionario.items() if v is not None}
    print(limpio)
    ```

18. Fusionar diccionarios sumando valores repetidos:
    ```python
    dict1 = {"a": 1, "b": 2, "c": 3}
    dict2 = {"b": 3, "c": 4, "d": 5}
    fusionado = {k: dict1.get(k, 0) + dict2.get(k, 0) for k in set(dict1) | set(dict2)}
    print(fusionado)
    ```

19. Ordenar por longitud de clave:
    ```python
    def ordenar_por_longitud_clave(diccionario):
        return sorted(diccionario.items(), key=lambda x: len(x[0]))

    mi_dict = {"a": 1, "abc": 2, "ab": 3}
    print(ordenar_por_longitud_clave(mi_dict))
    ```

20. Sistema de gestión de inventario:
    ```python
    inventario = {}

    def agregar_producto(nombre, cantidad):
        inventario[nombre] = inventario.get(nombre, 0) + cantidad

    def actualizar_cantidad(nombre, cantidad):
        if nombre in inventario:
            inventario[nombre] = cantidad
        else:
            print("Producto no encontrado")

    def mostrar_inventario():
        for producto, cantidad in inventario.items():
            print(f"{producto}: {cantidad}")

    # Uso del sistema
    agregar_producto("Manzanas", 50)
    agregar_producto("Peras", 30)
    actualizar_cantidad("Manzanas", 45)
    mostrar_inventario()
    ```