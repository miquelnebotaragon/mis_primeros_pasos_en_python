# Módulo 02. Las variables

## ✅ ¿Qué es una variable? ¿Para qué sirve?

El término __variable__, si no lo has escuchado todavía, no te preocupes que a partir de ya, en clase de Matemáticas será tu nuevo amigo 🙋‍♀️. Generalmente, se representan mediante letras del alfabeto latino (x, y, z, n...) y, dependiendo del tipo de ejercicio donde las veamos incorporadas, tienen un significado u otro.  
Por ejemplo, el caso más sencillo y con el que seguro que llevas trabajando mucho tiempo es en ejercicios de álgebra. Veamos el ejemplo siguiente:
  
> x + 5 = 7
  
Seguro que acabas de adivinar que el valor que se "oculta" tras la letra `x` es el 2. Pues algo parecido encontramos en los lenguajes de programación cuando hablamos de variables. Podríamos establecer un símil con una __celda o espacio en la memoria donde dejamos unos valores para que el programa, posteriormente los utilice para hacer cualquier función__.

![image](md02_mi_primera_ia_assets/programming-variable.png)  
Imagen: _CPT-programming-variable.svg_ · [Wikimedia Commons](https://creativecommons.org/publicdomain/zero/1.0/deed.en)

## ⛏ Empezamos a picar código

1️⃣ Para asignar un valor a una variable (almacenar un valor en memoria) debemos hacerlo usando letras o palabras completas seguidas del operador `=`. En programación no hace la misma función que en matemáticas y aquí es el encargado de "asignar" un valor (parte derecha) a la variable creada (parte izquierda).

```python
# Ejemplo de variable. Almacena la localidad de origen de un usuario
# `=`: Operador
# Parte izquierda antes del operador: Nombre de la variable
# Parte derecha después del operador: Valor asignado a la variable

localidad_origen = 'Son Servera'

print(localidad_origen)
```

Resultado:
>Son Servera

❓️ ¿Qué debemos tener en cuenta a la hora de definir variables?
  
* Para definir variables utilizaremos letras __[Aa - Zz], números [0 - 9] o la combinació de ambos__. No podemos utilizar símbolos ni caracteres especiales a excepción del guion bajo `_` cuya función explicaremos más adelante.
* Usaremos, en la medida de lo posible, __nombres concretos y descriptivos__ que faciliten la comprensión del código para aquellos que quieran usarlo en el futuro. En el caso que queramos definir variables usando solo letras, utilizaremos letras minúsculas, por ejemplo: a, n, x, nombre, valor, ciudad...  
❗️Atención: Es importante destacar que, en Python, los nombres que asignamos a las variables son _case-sensitive_ (diferenciación entre mayúsculas y minúsculas). Por ejemplo, codigo, Codigo y CODIGO, serían variables completamente diferentes. Aunque podemos utilizar mayúsculas debemos seguir las convenciones de escritura establecidas y hacerlo en minúscula siempre que sea posible.
  
* Si queremos utilizar variables con más de una palabra, __utilizaremos el guion bajo `-`__ para separarlas (en programación, este estilo de escritura es conocido como _snake_case_). Ej. nombre_completo, codigo_postal, nuevo_valor...
* Otra técnica menos utilizada pero también a nuestra disposición es la llamada _camelCase_ donde escribimos palabras juntas utilizando mayúscula cada vez que cambiamos de palabra. Ej. fechaNacimiento, ciudadOrigen, colorDePelo...
* Utilizaremos el operador de asignación `=` para dar el valor elegido a nuestra variable. __Antes y después del signo dejaremos un espacio en blanco__ (solo 1). Ej. edad = 77, nombre = 'Antonio'...
* Si queremos definir nuestra variable usando números, podemos hacerlo pero nunca a principio de palabra (no está permitido hacerlo). Ej. alumno7 = 'Pedro' (esto sí está permitido), ~~5a = 'Mi clase'~~ (esto no está permitido).
* Si tenemos un conjunto de variables y queremos escribirlas en una sola línea, lo haremos siguiendo la estructura siguiente: variable1, variable2, variable3 = 'Valor variable 1', 'Valor variable 2', 'Valor variable 3'.

```python
# Ejemplo de 3 variables en una misma línea
animal1, animal2, animal3 = 'Perro', 'Gato', 'Pájaro'

print(animal1)
print(animal2)
print(animal3)
print(animal1, animal2, animal3)
```

Resultado:
>Perro  
Gato  
Pájaro  
Perro Gato Pájaro

* Otra necesidad que puede aparecer es la de tener que dar a diversas variables el mismo valor. Podemos resolverlo de la siguiente manera: variable1 = variable2 = variable3 = 'valor deseado'
  
```python
# Asignación del mismo valor, un string en este caso, a 3 variables distintas
mi_presupuesto = tu_presupuesto = su_presupuesto = '3500 €'

print(mi_presupuesto)
print(tu_presupuesto)
print(su_presupuesto)
```

Resultado
>3500 €  
3500 €  
3500 €  

* Debemos recordar que el valor de una variable se puede modificar a lo largo del desarrollo del código. El sentido de lectura del lenguaje es descendente, es decir, cogerá el último valor que le hayamos asignado. Fíjate en el ejemplo siguiente:

```python
# Variable inicial
alumno_participante = 'Abel'

# Variable modificada
alumno_participante = 'Cristina'

print(alumno_participante)
```

Resultado
>Cristina

* En Python, al igual que en todos los lenguajes de programación, existen __palabras reservadas que NO podemos utilizar para nombrar variables__. Por ejemplo `print` o `break` no podrán ser nombres de variables ya que realizan otras funciones en la programación. Si quieres tener a mano la lista de palabras reservadas, ejecuta Python en tu equipo y escribe `help()` y, a continuación, `keywords` para ver en pantalla la lista completa de palabras a evitar en el momento de definir variables.  

![image](md02_mi_primera_ia_assets/keywords.png)  
Imagen: Intérprete de comandos en línea _python.org_ · [Python.org](https://www.python.org/shell)

* Si en lugar de definir una variable queremos disponer de __constantes__, lo haremos usando letras mayúsculas. Ej. MI_NOMBRE = 'Miquel'. Podemos definir una constante como un valor queremos mantener después de su asignación inicial. Por ejemplo, el nombre de un usuario o el valor de PI siempre serán los mismos y, por eso, podemos indicar (usando letras mayúsculas) que son valores que no deberíamos cambiar. En Python no hay un tipo de datos específico para las constantes pero, por convención, las podemos definir utilizando el nombre en mayúsculas al completo.
  
```python
# Ejemplo de constante
# Escribimos `PI`en letra mayúscula indicando así a los desarrolladores que
# es un valor que no debería ser modificado.

PI = 3,14159
```

Veamos una serie de ejemplos:  

Ejemplo 1: Almacenamos una variable.

```python
numero1 = 5
print(numero1)
```

Resultado:
> 5  

Ejemplo 2: Modificamos el valor de una variable.

```Python
valor1 = 5
valor1 = 100
print(valor1)
```

Resultado:
> 100

Ejemplo 3: Almacenamos dos variables y calculamos la suma de ambas.

```python
a = 5
b = 2
suma = a + b
print(suma)
```

Resultado:
> 7

Ejemplo 4: Anidamos variables en una única línea.

```python
valor1, valor2 = 135, 409
print(valor1)
print(valor2)
```

Resultado:
> 135  
> 409

Ejemplo 5: Almacenamos cadenas de texto en una variable. Recuerda, comillas simples o dobles (valen igual, eso sí, mantén coherencia en todo tu código usando unas o las otras).

```python
mi_nombre = 'Juan Pedro'
print(mi_nombre)
```

Resultado:
>Juan Pedro

Ejemplo 6: Almacenamos dos cadenas de texto y las mostramos a la vez en pantalla. Lo conseguiremos añadiendo como argumento de la función `print()` la variable 2, 3...

```python
alumna1 = 'Carla Domínguez'
alumno2 = 'Pedro Gomila'
print(alumna1, alumno2)
```

Resultado:
>Carla Domínguez Pedro Gomila

Ejemplo 7: Repetimos las cadenas de texto tantas veces como le indiquemos con `*veces`.

```python
alimento_favorito = 'Melón'
print(alimento_favorito * 3)
```

Resultado:
>MelónMelónMelón

Ejemplo 8: Modificamos el tipo de dato introducido.

```Python
# Establecemos una variable en formato de número entero
primer_numero = 27
print(primer_numero)
print(type(primer_numero)) # La función `type()` nos indicará de qué tipo de valor se trata.
```

Resultado:
> 27  
<class 'int'>

```Python
# Continuando con el ejemplo anterior 👆️, le decimos a Python que esta variable
# pasará a ser una cadena de texto

cambio_primer_numero = str(primer_numero) # str para cambiar a `string`.
print(cambio_primer_numero)
print(type(cambio_primer_numero))
```

Resultado:
>27  
<class 'str'>

```Python
# Intentamos sumarle 3 al 27 anterior y arrojará error porque ya NO es un número
print(cambio_primer_numero + 3)
```

Resultado:
>print(cambio_primer_numero + 3)  
          ~~~~~~~~~~~~~~~~~~~~~^~~
TypeError: can only concatenate str (not "int") to str

---

### 🔴 MD02 Actividad 01

Haz clic en el archivo __"main.py"__ que encontrarás en la parte superior de este módulo __escribe un total de tres variables que se muestren en pantalla a la vez__ con la función `print()`.  

Ejemplo:

```python
# Variables
amigo1 = 'Juan'
amigo2 = 'Carla'
amigo3 = 'Alba'

# Ejecución de la función
print(amigo1, amigo2, amigo3)
```

Resultado:
> Juan Carla Alba

---
2️⃣ Podemos conseguir que sea el usuario/a quien introduzca el valor a almacenar, lo haremos usando la función `input()`. Fíjate en el ejemplo:  

Ejemplo 1:

```Python
nombre = input('Escribe a continuación tu nombre: ')
print(nombre)
```

Esto devolverá en pantalla el nombre que hayamos introducido después de la pregunta que nos ha hecho el programa.  

Resultado:
> Escribe a continuación tu nombre: Miquel  
> Miquel

---

### 🔴 MD02 Actividad 02

Continuando con el ejemplo anterior, añade la función necesaria para que el programa te haga introducir tu nombre y muestre en pantalla los nombres de tus amigos. Puedes personalizar el texto tanto como quieras para que quede una oración lo más cuidada posible.

````Python
# Variables
amigo1 = 'Juan'
amigo2 = 'Carla'
amigo3 = 'Alba'
mi_nombre = input('Introduce tu nombre: ')

# Ejecución de la instrucción
print('Mi nombre es', mi_nombre, 'y los nombres de mis amigos son:', amigo1, amigo2, amigo3)
````

---

## ➕ Ampliación de conocimientos

Como te habrás dado cuenta, la oración anterior que genera tu nueva máquina de _inteligencia artificial_, tiene faltas de ortografía que no debemos pasar por alto y nos gustaría corregir.  

![image](md02_mi_primera_ia_assets/faltas.png)  

Como ya sabrás de tus clases de lengua, los elementos de una enumeración deben ir entre comas y, además, el último elemento precedido de "y". ¡Ah!, y no olvidar el punto antes de finalizar la oración.  
Veamos entonces una __serie de secuencias (llamadas de escape)__ que te permitirán generar textos perfectamente escritos.

### 👉 Salto de línea

Si deseamos saltar a una nueva línea, utilizaremos `\n` dentro de nuestra instrucción.  
Ejemplo:  

````Python
print('Hola:\n\nMi nombre es Alberto y esto aparecerá como si fuera la cabecera de una carta formal, es decir, en dos líneas separando el saludo del cuerpo del mensaje.')
````

Resultado:  
>Hola:
>
>Mi nombre es Miquel y esto aparecerá como si fuera la cabecera de una carta formal, es decir, en dos líneas separando el saludo del cuerpo del mensaje.

### 👉 Separadores

Como supongo que ya habrás notado, cada vez que en la función `print()` separamos con comas los elementos, la misma sintaxis introduce un espacio entre los elementos. Si queremos cambiar el tipo de separador lo haremos añadiendo `sep = 'cualquier_elemento'` a los argumentos de la función.  
Ejemplo:

````Python
print('cebollas','patatas','puerros','calabacín',sep = ',')
````

Resultado:  
>cebollas,patatas,puerros,calabacín

Si al elemento separador anterior le añadimos un espacio detrás de la coma `sep = ', '`, tendremos una enumeración prácticamente perfecta.

>cebollas, patatas, puerros, calabacín

### 👉 Finalizar

También podemos añadir punto al final añadiendo `end = '.'` a los argumentos de la función para indicarle a Python que será el punto el signo que acabará nuestra oración.  
Ejemplo:

````Python
print('Estoy practicando como mostrar texto en Python', end = '.')
````

Resultado:  
>Estoy practicando como mostrar texto en Python.

### 👉 Caracteres especiales

Se puede dar el caso que necesitemos escribir por ejemplo unas comillas `" "` o una barra invertida `\` y no vamos a ser capaces de hacerlo si no tenemos en cuenta que es la misma barra invertida la que hace de elemento de escape ("borra" la función habitual de dichos elementos).  

Ejemplo 1: si en la función `print()` utilizamos comillas dobles aún será algo más complicado. Veamos:

````Python
print("Quiero escribir unas comillas \"\"", end = '.')
````

Resultado:  
>Quiero escribir unas comillas "".

Ejemplo 2: veamos como escribir una barra inclinada.

````Python
print("Quiero escribir una barra inclinada \\", end = '.') # También podría ser `end = "."`
````

Resultado:  
>Quiero escribir una barra inclinada \.

---

### 👌 MD02 Actividad 03 (opcional)

Después de todo lo aprendido en esta última sección (__➕ Ampliación de conocimientos__) completa tus oraciones para conseguir el mejor resultado posible.

---

## 🤗 Resumen del Módulo 02

Hasta aquí la segunda lección con aspectos básicos sobre Python. Recuerda que deberías retener los siguientes conceptos:

1. Variable.
2. Asignación.
3. Palabras reservadas.
4. Secuencias de escape.
  
También que:

* En todos los lenguajes de programación existen variables que se almacenan de manera temporal en memoria.  
* Mediante sep = 'separador_deseado' y end = 'finalizador_deseado' podemos conseguir oraciones mejor construidas.
* Podemos utilizar "\n" para provocar un salto de línea.  
* Podemos utilizar la "\\" como secuencia de escape para escribir caracteres especiales.
