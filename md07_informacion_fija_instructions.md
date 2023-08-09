# Módulo 07. Secuencias. Tuplas y diccionarios

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


### 7️⃣ Tuplas
Las tuplas son también secuencias de datos muy similares a las listas, pero con una salvedad importante, son inmutables, es decir, no se pueden cambiar. De esta manera, no podremos añadir o modificar elementos como acabamos de hacer en las listas. Los elementos de una tupla deberán ir entre paréntesis "( )".  

Veamos en un ejemplo práctico cómo podemos modificar fácilmente una lista y cómo recibimos error al intentar modificar los elementos de una tupla.
```Python
# Comprobando la variabilidad de una lista
# Variables
lista1 = ['melón','sandía','papaya'] # Intentaremos modificar esta lista de frutas.
lista1.append('paraguayo') # Opción 1: Añadiendo un elemento a la lista anterior.

lista2 = ['melón','sandía','papaya'] 
lista2[0] = 'paraguayo' # Opción 2: Sustituyendo el primer elemento de la lista.

# Ejecución
print(lista1)
print(lista2)
```
Resultado:
> ['melón', 'sandía', 'papaya', 'paraguayo']  
['paraguayo', 'sandía', 'papaya']  

```Python
# Comprobando la inmutabilidad de una tupla
# Variables
tupla1 = ('Ana','Raquel','Saúl') # Intentaremos modificar esta tupla.
tupla1.append('Álvaro') # Opción 1: Añadiendo un elemento a la tupla anterior.

tupla2 = ('Ana','Raquel','Saúl') 
tupla2[0] = 'Álvaro' # Opción 2: Sustituyendo el primer elemento de la tupla.

# Ejecución
print(tupla1)
print(tupla2)
```
Resultado:
> AttributeError: 'tuple' object has no attribute 'append'  
> TypeError: 'tuple' object does not support item assignment
 
❗ ¡Cuidado! Las tuplas de un único elemento se pueden confundir con una variable corriente. Para evitar confusión deberemos introducir una coma "," dentro del paréntesis. Fíjate en el ejemplo.

````Python
 ### Ejemplo 1
# Variables
variable = ('Madrid')

# Ejecución
print(type(variable))

### Ejemplo 2
# Variables
tupla = ('Madrid',)

# Ejecución
print(type(tupla))
````
Resultado:
> <class 'str'>  
> <class 'tuple'>

Ejemplos de tuplas:
* ('Nalón','Nervión','Bidasoa')
* (-1,-2,-3)
* ('Perro salchicha','Gran Danés')

Algunas de las funciones de las tuplas son:
* _len()_ 👉 Medir la longitud de la tupla.

````Python
mar_cantabrico = ('Nalón','Nervión','Bidasoa')
print(len(mar_cantabrico))
````
Resultado:
> 3

* count() 👉 Contar la cantidad de veces que se repite un elemento dentro de la tupla.
````Python
# Variables
tupla1 = (1,2,3,4,5,6,5,7,8,9)
contar = tupla1.count(5)

# Ejecución
print(contar)
````  
Resultado:
> 2

* index() 👉 Busca un valor en la tupla y nos indica su posición.
````Python
 # Variables
 tupla1 = ('Jamón','Queso','Mantequilla')
 indice = tupla1.index('Mantequilla')

 # Ejecución
 print(indice)
 ````
Resultado:
> 2

---
### 🔴 MD07 Actividad 01
Crea un conjunto de secuencias de datos y haz que tu programa sea capaz de identificar qué es una cadena de texto, una lista y una tupla.
Fíjate en el ejemplo:
```Python
# Variables
num = 1
num2 = 7.5
num3 = 2j+3
cad = 'El halcón peregrino'
list = [100,200,300]
list2 = ['A','B','C']
tuple = ('sobre','tras','durante','mediante')

# Ejecución
print(type(num))
print(type(num2))
print(type(num3))
print(type(cad))
print(type(list))
print(type(list2))
print(type(tuple))
```
Resultado:
> <class 'int'>  
<class 'float'>  
<class 'complex'>  
<class 'str'>  
<class 'list'>  
<class 'list'>  
<class 'tuple'>  
---

### 🔴 MD07 Actividad 02
Estas son las notas de Abelardo de la asignatura de Matemáticas de todo el curso:
Notable, Excelente, Notable, Notable, Bien, Excelente, Bien, Suficiente, Notable y Notable.
Introduce las notas de Abelardo en una tupla y cuenta cuántas veces se repite cada calificación. Finalmente, indica mediante mensajes de texto cuántas veces se ha repetido cada nota.
Fíjate en el ejemplo, ya que lo podemos complicar tanto como queramos:
```Python
# Variables
animales = ('cerdo','chimpancé','jirafa','cerdo')

animal1 = animales[0]
animal2 = animales[1]
animal3 = animales[2]

contar_animal1 = animales.count('cerdo')
contar_animal2 = animales.count('chimpancé')
contar_animal3 = animales.count('jirafa')

# Ejecución
print(f'La palabra {animal1} se ha repetido {contar_animal1} veces.')
print(f'La palabra {animal2} se ha repetido {contar_animal2} veces.')
print(f'La palabra {animal3} se ha repetido {contar_animal3} veces.')
```
Resultado:
> La palabra cerdo se ha repetido 2 veces.  
La palabra chimpancé se ha repetido 1 veces.  
La palabra jirafa se ha repetido 1 veces.  
---
## ➕ Ampliación de conocimientos
Seguro que hay algo del ejemplo anterior que no te acaba de encajar, puesto que no lo habíamos visto hasta el momento. Fíjate en la captura siguiente 👇️.
![image](assets/f_strings.png)
Imagen: _f-Strings_ en Python.  

Para poder dar formato a un texto hemos utilizado dentro de las composiciones de texto para unir elementos las comas "," o también el signo "+". A partir de la versión 3.6 de Python se introdujo un nuevo concepto llamado _f-strings_ (_formatted string literals_) que nos facilitará enormemente poder formatear rápidamente las cadenas de texto. Veamos un par de ejemplos:

#### <ins>Método utilizado hasta el momento</ins>
```Pyhton
# Variables
alumno1 = 'Beatriz'
alumno2 = 'Sarai'

# Ejecución
print('Mis dos mejores amigas en clase son',alumno1,'y',alumno2,end=('.\n'))
print('Mis dos mejores amigas en clase son '+alumno1+' y '+alumno2+'.')
```
Resultado:
> Mis dos mejores amigas en clase son Beatriz y Sarai.  
Mis dos mejores amigas en clase son Beatriz y Sarai.

#### <ins>Método utilizado _f-strings_</ins>
```Python
# Ejecución
print(f'Mis dos mejores amigas en clase son {alumno1} y {alumno2}.')
```
Resultado:
> Mis dos mejores amigas en clase son Beatriz y Sarai.

Como las f-strings se van evaluando al momento podemos utilizarlas para poder efectuar también, por ejemplo, operaciones aritméticas básicas. Fíjate en el ejemplo:
```Python
# Variables
entero1 = 100
entero2 = 15

# Ejecución
print(f'El resultado del producto entre {entero1} y {entero2} es {entero1 * entero2}.')
```
Resultado:
> El resultado del producto entre 100 y 15 es 1500.

# 🤗 Resumen del Módulo 7

Hasta aquí la séptima lección con aspectos básicos sobre Python. Recuerda que deberías retener los siguientes conceptos:
1. Tipos de datos.
2. Tipos de secuencias: tuplas.
3. _tuple_.
4. Datos inmutables.
5. f-strings 👉️ _f { }_.
