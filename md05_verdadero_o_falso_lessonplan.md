# Lesson plan
  
  ** this file should contain teacher lesson plan details ** 

  __ students will never see this __

  ## Objetivos de aprendizaje en este módulo
  1. Conocer los tipos de datos básicos que podemos encontrar en Python.
  2. Trabajar con datos booleanos en Python: _TRUE_ o _FALSE_.
  3. Familiarizarse con los operadores de comparación (igual, diferente, mayor, menor, mayor que y menor que).
  4. Familiarizarse con los operadores lógicos (_and_, _or_ y _not_).


  Más información en la página de contacto del autor 👉 [Miquel Nebot](https://miquelnebot.es).

### Solución actividad MD05 Actividad 01
````Python
# Variables
n1 = float(input('Introduce el primer número: '))
n2 = float(input('Introduce ahora el segundo número: '))

# Ejecución
print('¿Son los dos números iguales?', n1 == n2)
print() # Este print() generará un espacio en blanco.
print('¿Son los dos números diferentes?', n1 != n2)
print()
print('¿Es el primer número mayor que el segundo?', n1 > n2)
print()
print('¿Es el segundo número mayor o igual que el primero?', n2 >= n1)
print()
print('Invierte el valor anterior:',not(n2 >= n1))
````
### Solución actividad MD05 Actividad 02
````Python
# Variable
numero = int(input('Introduce un número entero positivo: '))

# Ejecución
if numero % 2 != 0:
  print('¡El número', numero,'es impar!')
elif numero % 2 == 0 and numero >= 0 and numero <= 100:
  print('¡El número', numero,'es par y está entre 0 y 100!')
else:
  print('¡El número', numero,'es par, pero no está entre 0 y 100!')
````
