# Lesson plan
  
  ** this file should contain teacher lesson plan details ** 

  __ students will never see this __

  ## Objetivos de aprendizaje en este módulo
  1. Conocer los tipos de datos básicos que podemos encontrar en Python.
  2. Trabajar con las secuencias de datos de tipo diccionario, _dictionary_.
  3. Familiarizarse con los métodos básicos de los diccionarios (mostrar valores, añadir, eliminar, cambiar elementos, ordenar, longitud...).
  4. Desarrollar métodos para la presentación avanzada de datos en pantalla.

  Más información en la página de contacto del autor 👉 [Miquel Nebot](https://miquelnebot.es).

### Solución actividad MD08 Actividad 01
```Python
# Variables
datos_alumnado = {'AL1':[{'nombre':'Carlos','apellido1':'Alzamora','apellido2':'Garau','fecha':'28_02_2012'}],\
                  'AL2':[{'nombre':'Macarena','apellido1':'Arjona','apellido2':'Pérez','fecha':'04_06_2012'}],\
                    'AL3':[{'nombre':'Jordi','apellido1':'Ballester','apellido2':'Suau','fecha':'12_03_2012'}]}
```

### Solución actividad MD08 Actividad 02 (opcional)
```Python
# Variables
datos_alumnado = {'AL1':[{'nombre':'Carlos','apellido1':'Alzamora','apellido2':'Garau','fecha':'28_02_2012'}],\
                  'AL2':[{'nombre':'Macarena','apellido1':'Arjona','apellido2':'Pérez','fecha':'04_06_2012'}],\
                  'AL3':[{'nombre':'Jordi','apellido1':'Ballester','apellido2':'Suau','fecha':'12_03_2012'}]}

# Ejecución:
for alumno,datos in datos_alumnado.items():
  nombre = datos[0]['nombre']
  apellido1 = datos[0]['apellido1']
  apellido2 = datos[0]['apellido2']
  fecha = datos[0]['fecha']
  print(f'{alumno} > {nombre} {apellido1} {apellido2} - {fecha}')
```
Resultado:
> AL1 > Carlos Alzamora Garau - 28_02_2012  
AL2 > Macarena Arjona Pérez - 04_06_2012  
AL3 > Jordi Ballester Suau - 12_03_2012  
