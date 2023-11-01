# Lesson plan
  
  ** this file should contain teacher lesson plan details ** 

  __ students will never see this __

  ## Objetivos de aprendizaje en este módulo
  1. Repasar la declaración o definición de funciones en Python.
  2. Repasar el funcionamiento de variables. 
  3. Repasar el funcionamiento y uso de operaciones aritméticas básicas.
  6. Desarrollar funciones propias para su uso a lo largo de las diferentes propuestas.
  7. Uso de la librería _Tkinter_ para la creación de interfaces gráficas para nuestros programas.

  Más información en la página de contacto del autor 👉 [Miquel Nebot](https://miquelnebot.es).

### Solución actividad MD11 Actividad 01 (opcional)
```Python
# Importación de módulos y creación de alias
import tkinter as tk

# Diseño de nuestra interfaz gráfica
aplicacion = tk.Tk() 
aplicacion.title('Miquel\'s APP') 
aplicacion.geometry('400x400') 
aplicacion.configure(background='#ffffff')

etiqueta1 = tk.Label(text='Introduce tu nombre') # Etiqueta de texto
entrada1 = tk.Entry() # Cuadro de entrada de valores

etiqueta1.pack() # Empaquetado del primer elemento
entrada1.pack() # Empaquetado del segundo elemento

aplicacion.mainloop() 
```

### Ejemplo de posible solución actividad MD11 Actividad 02
```Python
# Importación de módulos y creación de alias
import tkinter as tk

# Función principal
def dividir():
    dividendo = int(entrada_dividendo.get())
    divisor = int(entrada_divisor.get())
    resultado = dividendo / divisor
    etiqueta_resultado.config(text='Resultado: ' + str(resultado))

# Creación de la interfaz gráfica
aplicacion = tk.Tk()
aplicacion.title('Calculadora')
aplicacion.geometry('400x200')

## Creación de los elementos o widgets que conformarán la aplicación
etiqueta_dividendo = tk.Label(text='Dividendo:')
entrada_dividendo = tk.Entry()

etiqueta_divisor = tk.Label(text='Divisor:')
entrada_divisor = tk.Entry()

etiqueta_resultado = tk.Label(text='--')

boton_sumar = tk.Button(text='Dividir', command=dividir)

## Empaquetado de todos los elementos para que sean visibles en pantalla
etiqueta_dividendo.pack()
entrada_dividendo.pack()
etiqueta_divisor.pack()
entrada_divisor.pack()
etiqueta_resultado.pack()
boton_sumar.pack()

aplicacion.mainloop()
```
