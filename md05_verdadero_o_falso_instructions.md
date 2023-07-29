# Módulo 05. Tipos de datos. Booleanos

## ❓ ¿Qué tipos de datos podemos tratar en Python?
Los tipos de datos nos ayudarán a conocer algo mejor la información que queremos tratar en nuestros programas. Empecemos entonces con una simple clasificación:
  * De Texto
    * 1️⃣ Cadenas de texto 👉 _(str)_
  * Datos Numéricos
    * 2️⃣ Números enteros 👉 _(int)_
    * 3️⃣ Números reales (o de "coma flotante") 👉 _(float)_
    * 4️⃣ Números complejos 👉 _(complex)_
  * Datos Booleanos 
    * 5️⃣ Bool 👉 _(bool)_
  * Secuencias
    * 6️⃣ Listas 👉 _(list)_
    * 7️⃣ Tuplas 👉 _(tuple)_
    * 8️⃣ Diccionarios 👉 _(dict)_

### 5️⃣ Datos booleanos _(bool)_
Este tipo de datos representan valores de verdad, es decir, para indicar si son valores verdaderos o falsos. En Python se representan como _TRUE_ o _FALSE_. Veamos unos ejemplos prácticos:

Ejemplo 1: ¿Es 1 igual a 2?
````Python
print(1==2)
````
Resultado:
> False

Ejemplo 2: ¿Es 2/3 mayor que 1/6?
````Python
print(2/3>1/6)
````
Resultado:
> True

## ➕ Ampliación de conocimientos
Para poder seguir trabajando con datos en Python es esencial que comprendamos, a nivel muy básico, qué __operadores lógicos y de comparación__ existen en este lenguaje de programación.  

👉 Operador de comparación: IGUAL _(==)_.  
El doble igual se utiliza para saber si un valor es igual que otro. La respuesta que arrojará Python será _TRUE_ (verdadero) o _FALSE_ (falso).  

Ejemplo 1: compararemos dos números.
````Python
# Variables
n1 = 10
n2 = 10

# Ejecución
print(n1 == n2)
````
Resultado:
> True

Ejemplo 2: seguimos comparando dos números.
````Python
# Variables
n1 = 5000
n2 = 5002
comparacion = (n1 == n2)
# Ejecución
print(comparacion)
````
Resultado:
> False

Ejemplo 3: comparamos dos cadenas de texto _str_.
````Python
# Variables
palabra1 = 'Alfonso'
palabra2 = 'alfonso'

# Ejecución
print(palabra1 == palabra2)
````
Resultado:
> False

Ejemplo 4: vamos a rizar el rizo y conseguiremos que el ejemplo anterior sea verdadero.
````Python
# Variables
palabra1 = 'Alfonso'
palabra2 = 'alfonso'

# Ejecución
print(palabra1.lower() == palabra2.lower())
````
Resultado:
> True

👉 Operador de comparación: DISTINTO DE _(!=)_.    
El signo de admiración y el de igual se utiliza para saber si dos o más valores son diferentes entre sí. La respuesta que arrojará Python será _TRUE_ (verdadero) o _FALSE_ (falso).  

Ejemplo 1: compararemos dos números.
````Python
# Variables
n1 = 1004
n2 = 1004.5

# Ejecución
print(n1 != n2)
````
Resultado:
> True


👉 Operador de comparación: MAYOR QUE _(>)_, MENOR QUE _(<)_.  
El signo de mayor o menor se utilizan para saber si un valor es mayor o menor que otro dado. La respuesta que arrojará Python será _TRUE_ (verdadero) o _FALSE_ (falso).  

Ejemplo 1: verificaremos qué número es mayor.
````Python
# Variables
n1 = 1/8
n2 = 1/4

# Ejecución
print(n1 > n2)
````
Resultado:
> False

Ejemplo 2: verificaremos qué número es menor.
````Python
# Variables
n1 = 17
n2 = 27

# Ejecución
print(n1 < n2)
````
Resultado:
> True

👉 Operador de comparación: MAYOR O IGUAL QUE _(>=)_, MENOR O IGUAL QUE _(<=)_.  
El signo de mayor/menor acompañado de un igual se utiliza para saber si un valor es mayor/menor o igual que el que aparece a continuación a su derecha. La respuesta que arrojará Python será _TRUE_ (verdadero) o _FALSE_ (falso).  

Ejemplo 1: compararemos dos números.
````Python
# Variables
n1 = 50
n2 = 50

# Ejecución
print(n1 >= n2)
````
Resultado:
> True

Ejemplo 2: seguiremos comparando dos números.
````Python
# Variables
n1 = 1037
n2 = 1115

# Ejecución
print(n1 <= n2)
````
Resultado:
> True

👉 Operador lógico: Y _(and)_.  
Este operador lógico devuelve _TRUE_ cuando al comparar dos o más valores todos deben ser verdaderos. En caso contrario, devuelve _FALSE_.  

Ejemplo 1: veamos un ejemplo sencillo con números.
````Python
# Variables
n1 = 10
n2 = 20
n3 = 30

# Ejecución
print(n1 <= n2 and n2 <= n3)
````
Resultado:
> True

Ejemplo 2: vayamos ahora a por un ejemplo en formato de texto.
````Python
# Variables
juan_futbolista = True
juan_estudiante = True
juan_padre = True

# Ejecución
print(juan_futbolista and juan_estudiante and juan_padre)
````
Resultado:
> True

👉 Operador lógico: O _(or)_.  
Este operador lógico devuelve _TRUE_ cuando al comparar dos o más valores se cumple alguna condición. En caso contrario, devuelve _FALSE_.  

Ejemplo 1: veamos un ejemplo sencillo con números.
````Python
# Variables
n1 = 22
n2 = 20


# Ejecución
print(n1 < n2 or n1 == n2)
````
Resultado:
> False

Ejemplo 2: continuando con el ejemplo anterior...
````Python
# Variables
juan_futbolista = True
juan_estudiante = False
juan_padre = True

# Ejecución
print(juan_futbolista or juan_estudiante or juan_padre)
````
Resultado:
> True

👉 Operador lógico: NO _(not)_.  
Este operador lógico invierte el valor booleano de una variable. En caso de ser _TRUE_ pasará a ser _FALSE_.  

Ejemplo 1:
````Python
# Variables
n1 = 100
n2 = 104


# Ejecución
print(not(n1 < n2))
````
Resultado:
> False

Ejemplo 2:
````Python
# Variables
pedro_camionero = True

# Ejecución
print(not(pedro_camionero))
````
Resultado:
> False
  
![image](assets/logicos_comparacion.png)
Imagen: Operadores lógicos y de comparación en Python.
### 🔴 MD05 Actividad 01
Desarrolla un programa sencillo donde el usuario deberá introducir 2 números en total. El programa <ins>deberá analizar dichos números</ins> y decirnos sí:  
* Si los dos números son iguales (es suficiente que arroje _TRUE_ o _FALSE_).
* Si los dos números son diferentes.
* Si el primero es mayor que el segundo.
* Si el segundo es mayor o igual que el primero.
* Invertir el resultado anterior.

### 🔴 MD05 Actividad 02
Crea en esta segunda actividad una aplicación donde el usuario tenga que introducir un número al azar y <ins>el sistema detecte si es par y está entre 0 y 100</ins>.  
❗ Recuerda que para saber si un número es par, debes dividirlo entre 2 y el residuo de la división debe darte 0. En el módulo 04 vimos como existía un operador aritmético _(%)_ con el cual podíamos adivinar el residuo de una división.
Ejemplo:
````Python
# Variable
numero = int(input('Introduce un número entero positivo: '))

# Ejecución
if numero % 2 == 0:
  print('¡Este número es par!')
else:
  print('¡El número', numero,'es impar!')
````
Además de los elementos del ejemplo, recuerda que deberás utilizar el operador lógico _(and)_ para conseguir tu cometido.  

# 🤗 Resumen del Módulo 5

Hasta aquí la quinta lección con aspectos básicos sobre Python. Recuerda que deberías retener los siguientes conceptos:
1. Tipos de datos.
2. Datos booleanos.
3. _bool_.
4. _TRUE_, _FALSE_.
5. Operadores de comparación.
6. Operadores lógicos.
  
También que:  
* En Python los operadores lógicos y de comparación son los siguientes:
  * Comparación: 
    * Igual: _(==)_ 👉 print(n1 == n2) 
    * Diferente: _(!=)_ 👉 print(n1 != n2)
    * Mayor: _(>)_ 👉 print(n1 > n2)
    * Menor: _(<)_ 👉 print(n1 < n2)
    * Mayor o igual: _(>=)_ 👉 print(n1 >= n2)
    * Menor o igual: _(<=)_ 👉 print(n1 <= n2)
  * Lógicos:
    * Y: _(and)_ 👉 print(pedro_musico and pedro_saxofonista)
    * O: _(or)_ 👉 print(araceli_deportista or araceli_trabajadora)
    * No: _(not)_ 👉 print(not(juan_maestro))
  
