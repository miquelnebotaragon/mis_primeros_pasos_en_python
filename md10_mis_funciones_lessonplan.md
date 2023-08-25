# Lesson plan
  
  ** this file should contain teacher lesson plan details ** 

  __ students will never see this __

  ## Objetivos de aprendizaje en este módulo
  1. Declarar o definir funciones en Python.
  2. Repasar el funcionamiento de condicionales en Python (_if()_, _else()_y _elif()_).  
  3. Repasar el funcionamiento y uso de bucles en Python (_for_, _while_...).
  6. Desarrollar funciones propias para su uso a lo largo de las diferentes propuestas.

  Más información en la página de contacto del autor 👉 [Miquel Nebot](https://miquelnebot.es).

### Solución actividad MD10 Actividad 01 (opcional)
```Python
def imprimir_materias():
    asignaturas = ['Mates', 'Lengua', 'Ciencias', 'Tecnología']
    seleccion = int(input('Del 0 al 3, di qué asignatura quieres ver: '))
    
    if 0 <= seleccion < len(asignaturas):
        print(asignaturas[seleccion])
    else:
        print('Opción incorrecta. ¡Introduce un número válido!')

imprimir_materias()
```

### Solución actividad MD10 Actividad 02
```Python
year_actual = int(input('Introduce el año actual: '))
year_nacimiento = int(input('Introduce tu año de nacimiento: '))

def calcular_edad (year_actual, year_nacimiento):
    edad = year_actual - year_nacimiento
    return (edad)
print('Tu edad es', calcular_edad (year_actual, year_nacimiento),'años.')
```
Una solución alternativa con las mismas características en cuanto a rendimiento pero una mejor legibilidad:

```Python
def calcular_edad(year_actual, year_nacimiento):
    edad = year_actual - year_nacimiento

year_actual = int(input('Introduce el año actual: '))
year_nacimiento = int(input('Introduce tu año de nacimiento: '))
edad = calcular_edad(year_actual, year_nacimiento)
print('Tu edad es', edad, 'años.')
```
### Solución actividad MD10 Actividad 03
```Python
def area_triangulo(base, altura):
    area = (base * altura)/2
    return area

base = float(input('Introduce la medida de la base del triángulo: '))
altura = float(input('Introduce la altura del triángulo: '))
area = area_triangulo(base, altura)

print(f'El área del triángulo es {area} (unidades al cuadrado, x\u00b2).')
```
