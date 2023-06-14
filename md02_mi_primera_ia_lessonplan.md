# Lesson plan
  
  ** this file should contain teacher lesson plan details ** 

  __ students will never see this __

  ## Objetivos de aprendizaje en este módulo
  1. Aprender qué son las variables.
  2. Afianzar el trabajo con variables. Presentación y almacenaje.
  3. Trabajar de manera básica con las secuencias de escape en cadenas de texto.
     

Más información en la página de contacto del autor 👉 [Miquel Nebot](https://miquelnebot.es).

### Solución actividad MD02 Actividad 01
```python
# Variables
amigo1 = 'Juan'
amigo2 = 'Carla'
amigo3 = 'Alba'

# Ejecución de la instrucción
print(amigo1,amigo2,amigo3)
```
### Solución actividad MD02 Actividad 02
```python
# Variables
amigo1 = 'Juan'
amigo2 = 'Carla'
amigo3 = 'Alba'
mi_nombre = input('Introduce tu nombre: ')

# Ejecución de la instrucción
print('Mi nombre es',mi_nombre,'y los nombres de mis amigos son:',amigo1,amigo2,amigo3)
```
### Solución actividad MD02 Actividad 03 (opcional)
❗ De momento, como no hemos visto opciones de lista más avanzadas, les animaremos para que se esfuercen para conseguir una oración perfecta con los recursos vistos hasta el momento.  

```python
# Variables
amigo1 = 'Juan'
amigo2 = 'Carla'
amigo3 = 'Alba'
mi_nombre = input('Introduce tu nombre: ')
mi_nombre_con_espacio = mi_nombre+' ' # Con esta nueva variable conseguimos añadir un espacio al nombre introducido por el usuario/a.

# Ejecución de la instrucción
'''En esta instrucción hay que jugar de manera repetida con los espacios entre las variables para conseguir el resultado deseado.'''  

print('Mi nombre es ',mi_nombre_con_espacio,'y los nombres de mis amigos son: ',amigo1,', ',amigo2,' y ',amigo3,sep='',end='.') 
```
