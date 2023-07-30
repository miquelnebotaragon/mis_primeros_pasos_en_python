# Lesson plan
  
  ** this file should contain teacher lesson plan details ** 

  __ students will never see this __

  ## Objetivos de aprendizaje en este módulo
  1. Conocer los tipos de datos básicos que podemos encontrar en Python.
  2. Trabajar con las secuencias de datos de tipo lista, _list_.
  3. Familiarizarse con los métodos básicos de las listas (añadir, extender, insertar, contar, longitud, índice, extraer, eliminar, ordenar...).


  Más información en la página de contacto del autor 👉 [Miquel Nebot](https://miquelnebot.es).

### Solución actividad MD06 Actividad 01
````Python
# Variables
l1 = [1,2,3,33,44,55]
l2 = ['María','Antonio','Alba','Sara']
l3 = [37,'acordeón',2.5]

# Ejecución
print(type(l1[0]))
print(type(l2[0]))
print(type(l3[2]))
````
### Solución actividad MD06 Actividad 02
````Python
# Variable
loteria = [[17456,30007],23569,90869,20013,99521]

# Ejecución
print(loteria[0])
````

### Solución actividad MD06 Actividad 03
````Python
# Variable
loteria = [[17456,30007],23569,90869,20013,99521]
numero_navidad = loteria[0]
# Ejecución
print(loteria[0][1]) # Esta instrucción hará que muestre el segundo valor del primer elemento de la enumeración. Recuerda que siempre se empieza a contar desde el valor "0".
print(loteria[0][-1]) # Esta opción es igualmente válida. Nos muestra el último valor de la cadena establecida. Lo verán en el siguiente ejemplo propuesto.
````

### Solución actividad MD06 Actividad 04
````Python
# Variable
grupo_trabajo = ['Ana','Pablo','Sonia','Abel']

# Ejecución

for componentes in grupo_trabajo:
  print(componentes)
````

### Solución actividad MD06 Actividad 05
````Python
# Variable
grupo_trabajo = ['Ana','Pablo','Sonia','Abel']
grupo_trabajo.append('Mónica')

# Ejecución
for componentes in grupo_trabajo:
    print(componentes)
````

### Solución actividad MD06 Actividad 06
````Python
grupo_trabajo = ['Ana','Pablo','Sonia','Abel']
grupo_trabajo.append('Mónica')

# Ejecución
print(sorted(grupo_trabajo))
````
