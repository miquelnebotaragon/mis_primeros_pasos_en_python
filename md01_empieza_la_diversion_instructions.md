# Módulo 01. Aspectos básicos de Python

## 🤚🏻 Antes de empezar, ¿qué es replit.com?
  Replit.com es un espacio de trabajo colaborativo en línea que contiene un editor de código donde podemos programar en Python (además de en otros lenguajes) utilizando un __Idle__ (este es el nombre que recibe la consola o _shell_ de Python) completo y sin limitación.  

![image](md01_empieza_la_diversion_assets/logo.png)
 
  
  Fíjate como el punto de partida es siempre el símbolo mayor que ">" también llamado _prompt_. Dicho símbolo puede aparecer triplicado ">>>" en otros editores. 

![image](md01_empieza_la_diversion_assets/prompt_triple.png)

## ⛏ ¡Empezamos a picar!

Empecemos con algo tan sencillo como es utilizar la función precargada __print()__ la cual nos devolverá en pantalla aquello que tecleemos entre paréntesis y entrecomillado (las cadenas de texto o también llamadas _strings_ deben ir entre comillas). Recordad que para ejecutar el comando hay que pulsar "run" en la parte superior de esta consola.

```python
print('Mi primera línea de código en Python, ¡genial!')
```
Resultado:
> Mi primera línea de código en Python, ¡genial!
---
### 🔴 MD01 Actividad 01

Haz clic en el archivo __"main.py"__ que encontrarás en la parte superior de este módulo y escribe tu primera línea de código. <ins>Escribe una oración simple, la que tú quieras</ins>. Recuerda que aquello que escribas tiene que ir entre paréntesis y también entre comillas (pueden ser simples o dobles, da igual).  

Ejemplo:

```python
print('¡Me encanta esto de ser programador/a!')
```
Resultado:
> ¡Me encanta esto de ser programador/a!

---
## ➕ Ampliación de conocimientos

En Python, cada función debe ir en una línea diferente, por lo que __NO__ es nada recomendable anidar varias de ellas en la misma línea (la cual cosa podemos conseguir con el símbolo ";").  

Ejemplo:

```python
print ('Me llamo Miquel'); print ('y de apellido Nebot.')
```
Resultado:
> Me llamo Miquel\
> y de apellido Nebot.

Como podéis ver, aunque hemos juntado dos funciones en una misma línea (opción poco recomendable, ya que dificulta la lectura del código en caso de tener que analizarlo, reutilizarlo, depurarlo...), el resultado lo secciona en dos.

Si se diera el caso (poco probable) que necesitáramos utilizar diversas líneas para la misma instrucción, podemos forzar el salto de línea con el símbolo barra invertida __"\\\"__. 
 
Ejemplo:
 
 ```python
print ('Esto sería organizar funciones \
en diferentes líneas utilizando barra invertida, \
¿veis qué bien?')
```
Resultado:
>Esto sería organizar funciones en diferentes líneas utilizando barra invertida, ¿veis qué bien?

❗️ Al hilo de todo lo explicado en este apartado, comentar que existe una guía oficial de estilo denóminada __PEP 8__ _"Python Enhancement Proposal"_ donde encontramos 8 propuestas específicas para escribir código de manera clara, coherente i legible. El objetivo de esta guía es proporcionar unas directrices que ayuden a los desarrolladores a escribir código que sea fácil de leer, mantener y compartir con otros programadores/as.
### Principales recomendaciones de PEP 8:
__1. Identación:__ Utiliza 4 espacios para cada nivel de identación. Aunque lo veremos más adelante cuando tratemos las funciones, es importante no perder de vista esta primera recomendación. __NO__ se recomienda utilizar tabuladores.
```python
if a == 1:
    print('Correcto')
else:
    print('Incorrecto')
```
__2. Longitud de línea:__ Las líneas de código no deben tener más de 79 caracteres.
```python
# Esto sería un comentario de línea que, en ningún caso, supera los 79
# caracteres establecidos en la guía de estilo de PEP 8. En caso de necesitar
# comentarios largos utilizaremos almohadilla "#" al principio de cada una.
```

__3. Espacios en blanco:__ Deja espacios alrededor de los operadores (`=`, `+`, `-`...) y también después de las comas.
```python
a = 7
b = 30
c = 13
print(a + b + c)
```
Resultado:
>50

__4. Nombres de variables y funciones:__ Usa nombres descriptivos, en minúsculas y sin espacios. Si necesitas separar palabras utiliza guion bajo para hacerlo.
```python
nombre_chico = 'Andrés'
nombre_chica = 'Carla'
variable = int(input('Si eres chico pulsa 1, 2 si eres chica\n'))

if variable == 1:
    print('Tu compañero de trabajo será ' + nombre_chico + '.')
else:
    print('Tu compañera de trabajo será ' + nombre_chica + '.')
```
__5. Comentarios:__ Utiliza comentarios claros y concisos para explicar el código que puede no ser comprensible inmediatamente.
```python
# Mediante esta variable solicitamos al usuario que introduzca su edad.
# Quedará almacenada en la memoria en formato de número entero.

edad = int(input('¿Cuántos años tienes?\n'))

if edad >= 18:
    print('¡Enhorabuena! Ya eres mayor de edad.')

else:
    print('Eres joven, no tengas prisa. Aún no eres mayor de edad.')
```

__6. Módulos e importaciones:__ Cuando sea necesario (lo veremos en módulos posteriores), importa los módulos en líneas separadas y mantenlos al principio del archivo.
```python
import time
import os
```
__7. Blancos y líneas en blanco:__ Utiliza 2 líneas en blanco para separar definiciones de clases y funciones. 1 sola para separar bloques de código dentro de una función si crees que mejorará la legibilidad del código.
```python
def suma(a, b):
    # Suma de dos números
    return a + b

# Línea en blanco entre funciones según la guía de estilo PEP 8
def resta(a, b):
    # Resta dos números
    return a - b

# Programa principal para probar las funciones
if __name__ == "__main__":
    numero1 = int(input('Introduce el primer número: '))
    numero2 = int(input('Introduce el segundo número: '))

    resultado_suma = suma(numero1, numero2)
    resultado_resta = resta(numero1, numero2)

    print('La suma de', numero1, '+', numero2, 'es', resultado_suma)
    print('La resta de', numero1, '-', numero2, 'es', resultado_resta)
```

__8. Cadenas de caracteres (strings):__ Usa las comillas simples o dobles para cadenas breves. Eso sí, sé consistente al usar unas u otras. Para cadenas largas que incluyen salto de línea puedes usar 3 comillas dobles o simples tanto de apertura como de cierre.
```python
# Cadena con comillas simples
nombre = 'Antón'

# Cadena con comillas dobles
saludo = "¿Cómo te encuentras hoy?"

# Cadenas multilínea con comillas triples
mensaje = """Esta es una cadena de texto
multilínea que ocupa más espacio pero funciona
como una variable típica."""
```

## 💡 Vale... ¿y si quiero explicar mi código?

Es una práctica muy recomendable documentar nuestro código, es decir, efectuar anotaciones y explicaciones para facilitar la lectura y entendimiento a las personas que intenten utilizar nuestra aplicación en el futuro.  

Lo ideal es hacerlo con el símbolo almohadilla __"#"__. De esta manera iremos comentando líneas en el _idle_ de Python al igual que se hace en otros lenguajes de programación. Dicho símbolo hace posible que podamos redactar anotaciones, explicaciones, aclaraciones... o simplemente que invalidemos una o varias líneas de código de manera temporal si estamos realizando pruebas. Todo lo que siga a __"#"__, el editor lo omitirá y no se tendrá en cuenta en el momento de ejecutar el programa.  

Si el comentario es muy extenso y ocupa varias líneas, podemos seguir utilizando la almohadilla al inicio de cada línea. Aunque en Python es posible utilizar 3 comillas simples o dobles al principio y al final de un bloque de texto, obteniendo el mismo resultado (omisión del texto al ejecutar el código), es importante entender que este texto no se considera técnicamente un comentario, sino un __string literal__. Este string no está asociado a ninguna variable, por lo que Python lo descarta, aunque sigue ocupando espacio en memoria. Por esta razón, no es la mejor práctica para realizar comentarios multilínea generales.

Ejemplo 1: utilizando las comillas simples.

```python
''' Esto técnicamente no sería un comentario multilínea y, por lo tanto,
no es la mejor manera de comentar nuestro código. Recuerda que la opción
recomendada es utilizar la almohadilla al principio de cada línea que
deseemos incluir en nuestro código. '''
```
Resultado:
>-

Ejemplo 2: utilizando las comillas dobles.

```python
""" Esto técnicamente no sería un comentario multilínea y, por lo tanto,
no es la mejor manera de comentar nuestro código. Recuerda que la opción
recomendada es utilizar la almohadilla al principio de cada línea que
deseemos incluir en nuestro código. """
```
Resultado:
>-


## 👍️ Buenas prácticas
La codificación (o en inglés _enconding_) no es más que una simple directriz que colocamos al inicio de nuestros programas para indicarle a Python qué conjunto de caracteres utilizaremos a lo largo del mismo. UTF-8 (_Unicode Transformation Format_) es un formato de codificación de caracteres [Unicode](https://home.unicode.org/) que garantizará que nuestro proyecto pueda ser mostrado en cualquier ordenador sin errores ni caracteres extraños.  

```Python
# -*- coding: utf-8 -*-
print('Funcionará perfectamente con tildes, ñ... lo que queramos.')
```

---
### 🔴 MD01 Actividad 02

Haz clic en el archivo __"main.py"__ y, antes de la oración de la Actividad 01, <ins>haz un comentario usando la tecla almohadilla "#"</ins>.  

Ejemplo:

```python
# -*- coding: utf-8 -*-
# Miquel Nebot · Mayo 2023

print('¡Me encanta esto de ser programador/a!')
```

---
# 🤗 Resumen del Módulo 01

Hasta aquí esta primera lección con los aspectos más básicos de Python. Recuerda que deberías retener los siguientes conceptos:
1. Idle de Python (Shell o consola).
2. Prompt (>) o (>>>).
3. Función.
4. print('Hola mundo').
5. Unicode.
  
También que:  
* En Python cada instrucción deberá aparecer en una línea individual.  
* Podemos utilizar ";" para unir instrucciones en una misma línea.  
* Podemos utilizar la "\\" para fragmentar instrucciones en diversas líneas.  
* Utilizamos "#" para comentar, explicar o impedir que se ejecute alguna instrucción de manera temporal.
* Para comentarios largos que ocupen diversas líneas podemos utilizar 3 comillas simples o dobles para abrir y cerrar.  
