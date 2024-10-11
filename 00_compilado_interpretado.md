**interpretado**.

### Ejemplo de código en C (Compilado)

Este es un código básico en C que imprime "Hola, mundo":

```c
#include <stdio.h>

int main() {
    printf("Hola, mundo\n");
    return 0;
}
```

### Ejemplo de código en Python (Interpretado)

Este sería el equivalente en Python:

```python
print("Hola, mundo")
```

### Diferencias clave entre **compilado** e **interpretado**

#### 1. **Compilado** (C)

Cuando trabajamos con un lenguaje compilado como C, el código fuente pasa por un **proceso de compilación** antes de ejecutarse:

1. **Escribimos el código** (archivo `.c`).
2. **Compilamos el código** usando un compilador, por ejemplo, en Linux podríamos usar `gcc`:
   
   ```bash
   gcc hola.c -o hola
   ```

   Esto genera un archivo ejecutable (`hola` en este caso).
   
3. **Ejecutamos el programa** directamente a través del ejecutable:

   ```bash
   ./hola
   ```

   Aquí, el compilador tradujo todo el código C a código máquina, que la CPU puede ejecutar directamente.

- **Ventajas del compilado**: Una vez compilado, el programa suele ejecutarse más rápido, ya que ya está en formato nativo para la máquina.
- **Desventajas del compilado**: El proceso de compilación toma tiempo y el binario generado es específico para la plataforma en la que fue compilado (por ejemplo, un ejecutable compilado en Linux no funcionará en Windows sin recompilarlo).

#### 2. **Interpretado** (Python)

En un lenguaje interpretado como Python, el código no se compila en un archivo ejecutable antes de ejecutarse. En lugar de eso, se ejecuta directamente línea por línea por un **intérprete**:

1. **Escribimos el código** (archivo `.py`).
2. **Ejecutamos el código directamente**:

   ```bash
   python hola.py
   ```

   Aquí, el intérprete de Python lee el código fuente, lo traduce y lo ejecuta en el momento.

- **Ventajas del interpretado**: No es necesario un paso de compilación, lo que hace más rápido el desarrollo (menos tiempo entre escribir el código y ejecutarlo). Además, el código es más portátil, ya que el mismo archivo Python puede ejecutarse en diferentes sistemas operativos, siempre que haya un intérprete de Python disponible.
- **Desventajas del interpretado**: Generalmente, los lenguajes interpretados son más lentos que los compilados, ya que el intérprete debe traducir el código fuente a código máquina cada vez que se ejecuta.

### Resumen de las diferencias

| Característica           | Lenguaje Compilado (C)                        | Lenguaje Interpretado (Python)                  |
|--------------------------|-----------------------------------------------|------------------------------------------------|
| **Ejecución**             | El código se compila y luego se ejecuta       | El código se interpreta y ejecuta línea por línea |
| **Velocidad de ejecución**| Generalmente más rápida                      | Generalmente más lenta                         |
| **Portabilidad**          | Depende del sistema donde se compile          | Alta, con tal de que haya un intérprete disponible |
| **Proceso de desarrollo** | Requiere compilar antes de ejecutar           | No necesita compilación, se ejecuta directamente |
| **Errores**               | Detectados en el proceso de compilación       | Detectados al momento de ejecución             |

### Conclusión

Los lenguajes compilados, como C, suelen ser más rápidos en tiempo de ejecución, pero requieren un paso adicional de compilación. Los lenguajes interpretados, como Python, son más flexibles y fáciles de probar rápidamente, pero suelen ser un poco más lentos debido al proceso de interpretación. ¡Cada uno tiene sus ventajas y desventajas según el tipo de proyecto!

