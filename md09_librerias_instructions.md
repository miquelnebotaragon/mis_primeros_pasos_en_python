# Módulo 09. Librerías

## ❓ ¿Qué son las librerías? ¿Para qué sirven? ¿Cuántas hay?
De manera muy simple, podríamos definir una __librería__ (también son conocidas como bibliotecas o módulos) como <ins>un conjunto de instrucciones que permiten extender las funcionalidades básicas del lenguaje</ins>, ayudándonos a ahorrar tiempo al no tener que picar todo el código desde cero.
A día de hoy se computan más de 130.000 librerías en Python que nos facilitarán enormemente nuestro trabajo a la hora de programar. Veamos algunos ejemplos:

### Time

Librería [time](https://docs.python.org/3/library/time.html). Gracias a esta librería podremos (entre otras muchas funciones) detener por ejemplo la ejecución de nuestro programa los segundos que le marquemos a esta función.

```Python
# Librerías
import time

# Ejecución
nombre = (input('¿Serías tan amable de decirme tu nombre? '))

time.sleep(1)
print(f'\nBienvenido/a {nombre}, ¿qué tal te encuentras hoy?')
time.sleep(2)

quiere = int(input('\n¿Quieres saber cuántas letras tiene tu nombre? 1 para sí, 2 para no. '))

if quiere == 1:
    print(len(nombre))
    time.sleep('¡Gracias por utilizar el servicio!')
else:
    print('Gracias y que pases muy buen día.')
```
Resultado:
> ¿Serías tan amable de decirme tu nombre? Anacleto  
>
> Bienvenido/a Anacleto, ¿qué tal te encuentras hoy?  
>
> ¿Quieres saber cuántas letras tiene tu nombre? 1 para sí, 2 para no. 2  
> Gracias y que pases muy buen día.    

### Random
Librería [_random_](https://docs.python.org/es/3.10/library/random.html). Este módulo implementa generadores de números pseudoaleatorios (no siguen ningún patrón aunque son generados por un algoritmo determinista).

```Python
# Librerías
import random

# Ejecución
for num in range(5):
    aleatorios = random.randint(0,100)
    print(aleatorios)
```
Resultado:
> 3  
34  
71  
92  
42  

### Pandas
Librería [_pandas_](https://pandas.pydata.org/). Es una de las librerías "estrella" que encontrarás en prácticamente todos los programas desarrollados en Python, donde se manejen y analicen estructuras de datos.

Ejemplo 1: En este primer ejemplo construiremos un diccionario con datos para realizar una tabla de temperaturas medias anuales de una localidad del Mediterráneo.

```Python
# Librerías
import pandas as pd

# Ejecución
datos = {'Meses':['Enero','Febrero','Marzo','Abril','Mayo','Junio','Julio','Agosto','Septiembre','Octubre','Noviembre','Diciembre'],\
         'Temperaturas':[16,14,23,25,27,30,31,30,29,24,20,18]}

climograma = pd.DataFrame(datos)
print(climograma)
```
Resultado:  
![image](md09_librerias_assets/libreria_pandas_ejemplo.png)

Ejemplo 2: Avanzamos algo más en este segundo ejemplo donde trataremos de que la librería lea los datos incluidos en un archivo CSV (archivo de texto plano con los valores separados por comas "," o punto y coma ";") con información de alumnos para finalmente generar un _dataframe_ (tabla) con dicha información.  

📝 [grupo1.csv](md09_librerias_assets/grupo1.csv)

```Python
# Librerías
import pandas as pd

# Ejecución
grupo1 = pd.read_csv('grupo1.csv', sep=';',index_col=0)

print(grupo1)
```
Resultado:  
![image](md09_librerias_assets/libreria_pandas_ejemplo_1.png)

---
### 🔴 MD09 Actividad 01
Después de analizar los ejemplos anteriores, <ins>crea un diccionario de ejemplo con gastos e ingresos</ins> de una supuesta venta de camisetas, bocadillos... que llevaríais a cabo para sufragar los gastos en un viaje de estudios. A continuación, mediante la librería _pandas_ muestra en pantalla el resultado obtenido.

---
### 👌 MD09 Actividad 02 (opcional)
Esta es una actividad guiada donde verás de primera mano cómo realizar un <ins>juego de prueba error utilizando la librería _random_</ins> en Python. Analiza, estudia y personaliza la programación a tu gusto para conseguir un programa lo más elaborado posible.
```Python
# Librerías
import random

# Variables
numero_aleatorio = random.randint(1, 100) # Generando un número aleatorio entre 1 y 100.
contador_usuario = 0

# Ejecución
while True: # El bucle estará en ejecución hasta que el usuario adivine el número aleatorio.
    numero_usuario = int(input('Introduce un número entre 1 y 100: '))
    if numero_usuario == numero_aleatorio:
        print(f'Has adivinado el número en {contador_usuario} intentos.')
        break
    elif numero_usuario < numero_aleatorio:
        print('El número que has elegido es bajo...')
    elif numero_usuario > numero_aleatorio:
        print('El número que has elegido es alto...')

    contador_usuario += 1 # Cada vez que el bucle se repita, se incrementará el contador de intentos.
  ```

---

# 🤗 Resumen del Módulo 9

Hasta aquí la novena lección con aspectos básicos sobre Python. Recuerda que deberías retener los siguientes conceptos:
1. Librerías.
2. Librerías _time_, _random_ y _pandas_.
3. _Dataframe_.
4. Archivo CSV.
