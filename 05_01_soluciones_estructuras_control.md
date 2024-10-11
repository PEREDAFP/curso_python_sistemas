# Soluciones: Ejercicios de Estructuras de Control en Python (1-25)

1. Determinar si un número es positivo, negativo o cero:
   ```python
   numero = float(input("Ingrese un número: "))
   if numero > 0:
       print("Positivo")
   elif numero < 0:
       print("Negativo")
   else:
       print("Cero")
   ```

2. Verificar si es mayor de edad:
   ```python
   edad = int(input("Ingrese su edad: "))
   if edad >= 18:
       print("Es mayor de edad")
   else:
       print("Es menor de edad")
   ```

3. Determinar si un año es bisiesto:
   ```python
   año = int(input("Ingrese un año: "))
   if (año % 4 == 0 and año % 100 != 0) or (año % 400 == 0):
       print("Es bisiesto")
   else:
       print("No es bisiesto")
   ```

4. Máximo de tres números:
   ```python
   a = float(input("Primer número: "))
   b = float(input("Segundo número: "))
   c = float(input("Tercer número: "))
   maximo = max(a, b, c)
   print(f"El máximo es: {maximo}")
   ```

5. Determinar si un número es par o impar:
   ```python
   numero = int(input("Ingrese un número: "))
   if numero % 2 == 0:
       print("Par")
   else:
       print("Impar")
   ```

6. Calificación en letra:
   ```python
   calificacion = float(input("Ingrese la calificación: "))
   if calificacion >= 90:
       print("A")
   elif calificacion >= 80:
       print("B")
   elif calificacion >= 70:
       print("C")
   elif calificacion >= 60:
       print("D")
   else:
       print("F")
   ```

7. Tipo de triángulo:
   ```python
   a = float(input("Lado 1: "))
   b = float(input("Lado 2: "))
   c = float(input("Lado 3: "))
   if a == b == c:
       print("Equilátero")
   elif a == b or b == c or a == c:
       print("Isósceles")
   else:
       print("Escaleno")
   ```

8. Calculadora simple:
   ```python
   a = float(input("Primer número: "))
   b = float(input("Segundo número: "))
   op = input("Operación (+,-,*,/): ")
   if op == '+':
       print(a + b)
   elif op == '-':
       print(a - b)
   elif op == '*':
       print(a * b)
   elif op == '/':
       if b != 0:
           print(a / b)
       else:
           print("Error: División por cero")
   else:
       print("Operación no válida")
   ```

9. Determinar si un número es primo:
   ```python
   num = int(input("Ingrese un número: "))
   es_primo = True
   for i in range(2, int(num**0.5) + 1):
       if num % i == 0:
           es_primo = False
           break
   print("Es primo" if es_primo and num > 1 else "No es primo")
   ```

10. Día de la semana:
    ```python
    dia = int(input("Ingrese un número del 1 al 7: "))
    dias = ["Lunes", "Martes", "Miércoles", "Jueves", "Viernes", "Sábado", "Domingo"]
    if 1 <= dia <= 7:
        print(dias[dia-1])
    else:
        print("Número no válido")
    ```

11. Factorial de un número:
    ```python
    n = int(input("Ingrese un número: "))
    factorial = 1
    for i in range(1, n+1):
        factorial *= i
    print(f"El factorial de {n} es {factorial}")
    ```

12. Secuencia de Fibonacci:
    ```python
    n = int(input("Ingrese el número de términos: "))
    a, b = 0, 1
    for _ in range(n):
        print(a, end=" ")
        a, b = b, a + b
    ```

13. Fizz Buzz:
    ```python
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

14. Triángulo de asteriscos:
    ```python
    n = int(input("Ingrese la altura del triángulo: "))
    for i in range(1, n+1):
        print('*' * i)
    ```

15. Suma de números pares del 1 al 100:
    ```python
    suma = sum(i for i in range(2, 101, 2))
    print(f"La suma es: {suma}")
    ```

16. Contar vocales en una frase:
    ```python
    frase = input("Ingrese una frase: ").lower()
    vocales = 'aeiou'
    conteo = {vocal: frase.count(vocal) for vocal in vocales}
    print(conteo)
    ```

17. Adivinar número aleatorio:
    ```python
    import random
    numero = random.randint(1, 100)
    while True:
        intento = int(input("Adivina el número (1-100): "))
        if intento < numero:
            print("Más alto")
        elif intento > numero:
            print("Más bajo")
        else:
            print("¡Correcto!")
            break
    ```

18. Cuadrado de asteriscos:
    ```python
    n = int(input("Ingrese el tamaño del cuadrado: "))
    for _ in range(n):
        print('*' * n)
    ```

19. MCD de dos números:
    ```python
    def mcd(a, b):
        while b:
            a, b = b, a % b
        return a

    num1 = int(input("Primer número: "))
    num2 = int(input("Segundo número: "))
    print(f"El MCD es: {mcd(num1, num2)}")
    ```

20. Simulación de lanzamiento de dado:
    ```python
    import random
    lanzamientos = [random.randint(1, 6) for _ in range(1000)]
    for i in range(1, 7):
        print(f"Número {i}: {lanzamientos.count(i)} veces")
    ```

21. Imprimir cadena al revés:
    ```python
    cadena = input("Ingrese una cadena: ")
    print(cadena[::-1])
    ```

22. Generar contraseña aleatoria:
    ```python
    import random
    import string
    caracteres = string.ascii_letters + string.digits + string.punctuation
    contraseña = ''.join(random.choice(caracteres) for _ in range(8))
    print(f"Contraseña generada: {contraseña}")
    ```
