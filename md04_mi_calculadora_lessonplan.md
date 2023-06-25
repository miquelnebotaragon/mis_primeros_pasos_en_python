# Lesson plan
  
  ** this file should contain teacher lesson plan details ** 

  __ students will never see this __

  ## Objetivos de aprendizaje en este módulo
  1. Conocer los tipos de datos básicos que podemos encontrar en Python.
  2. Trabajar con los tipos de números que podemos tratar en Python: enteros, de coma flotante y complejos.
  3. Practicar con algunos operadores aritméticos de las funciones relacionadas con los números.
  4. Descubrir las sentencias condicionales _if_, _elif_, _else_ y los bucles _while_.

  Más información en la página de contacto del autor 👉 [Miquel Nebot](https://miquelnebot.es).

### Solución actividad MD04 Actividad 01
````Python
# Variables
numero1 = int(input('Escribe el primer sumando: '))
numero2 = int(input('Ahora el segundo sumando: '))

# Ejecución
print('El resultado de la suma es:'numero1+numero2)
````  

### Solución actividad MD04 Actividad 02
````Python
# Variables
nombre1 = input('Escribe el primer nombre: ')
nombre2 = input('Ahora el segundo: ')

# Ejecución
if len(nombre1) > len(nombre2):
  print('El primer nombre es más largo.')
elif len(nombre1) < len(nombre2):
  print('El primer nombre es más corto.')
else:
  print('Los dos nombres son iguales.')
````
### Solución actividad MD04  Actividad 03 (opcional)
```Python
numero1 = float(input("Introduce ahora tu primer número: ") )
numero2 = float(input("Introduce a continuación tu segundo número: ") )

while True:
    print("""
    ¿Qué tipo de operación deseas realizar ahora?
    
    1) Sumar
    2) Restar
    3) Multiplicar
    4) Dividir
    5) Introducir nuevos valores
    6) Salir
    """)
    opcion = int(input("Elige una opción: ") )     

    if opcion == 1:
        print('')
        print('RESULTADO: La suma de',numero1,'+',numero2,'es',numero1+numero2)
    elif opcion == 2:
        print('')
        print('RESULTADO: La resta de',numero1,'-',numero2,'es',numero1-numero2)
    elif opcion == 3:
        print('')
        print('RESULTADO: El producto de',numero1,'x',numero2,'es',numero1*numero2)
    elif opcion == 4:
        print('')
        print('RESULTADO: El cociente entre',numero1,'/',numero2,'es',numero1/numero2)
    elif opcion == 5:
        numero1 = float(input('Introduce ahora tu primer número: ') )
        numero2 = float(input('Introduce ahora tu segundo número: ') )
    elif opcion == 6:
        break
    else:
        print("¡Opción incorrecta!")

``` 
