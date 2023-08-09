# Lesson plan
  
  ** this file should contain teacher lesson plan details ** 

  __ students will never see this __

  ## Objetivos de aprendizaje en este módulo
  1. Conocer los tipos de datos básicos que podemos encontrar en Python.
  2. Trabajar con las secuencias de datos de tipo tupla, _tuple_.
  3. Verificar la inmutabilidad de las tuplas.
  4. Descubrir y practicar con _f-strings_.


  Más información en la página de contacto del autor 👉 [Miquel Nebot](https://miquelnebot.es).

### Solución actividad MD07 Actividad 01
````Python
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
````
### Solución actividad MD07 Actividad 02
```Python
# Variables
notas = ('Notable','Excelente','Notable','Notable','Bien','Excelente','Bien','Suficiente','Notable','Notable')

suficiente = notas[7]
suficientes = notas[7]+'s' # Añadiendo "s" conseguiremos mejorar la redacción si el valor es >1.

bien = notas[4]

notable = notas[0]
notables = notas[0]+'s'

excelente = notas[1]
excelentes = notas[1]+'s'


contar_suficiente = notas.count('Suficiente')
contar_bien = notas.count('Bien')
contar_notable = notas.count('Notable')
contar_excelente = notas.count('Excelente')

# Ejecución
if contar_suficiente > 1:
    print(f'Abelardo ha sacado {contar_suficiente} {suficientes} en Matemáticas este curso.')
else:
    print(f'Abelardo ha sacado {contar_suficiente} {suficiente} en Matemáticas este curso.')

print(f'Abelardo ha sacado {contar_bien} {bien} en Matemáticas este curso.')

if contar_notable > 1:
    print(f'Abelardo ha sacado {contar_notable} {notables} en Matemáticas este curso.')
else:
    print(f'Abelardo ha sacado {contar_notable} {notable} en Matemáticas este curso.')

if contar_excelente > 1:
    print(f'Abelardo ha sacado {contar_excelente} {excelentes} en Matemáticas este curso.')
else:
    print(f'Abelardo ha sacado {contar_excelente} {excelente} en Matemáticas este curso.')
```
