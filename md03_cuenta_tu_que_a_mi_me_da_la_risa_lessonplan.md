# Lesson plan
  
  ** this file should contain teacher lesson plan details ** 

  __ students will never see this __

  ## Objetivos de aprendizaje en este módulo
  1. Conocer los tipos de datos básicos que podemos encontrar en Python.
  2. Descubrir las secuencias o cadenas de texto (_strings_).
  3. Practicar con algunas de las funciones relacionadas con las cadenas de texto.

  Más información en la página de contacto del autor 👉 [Miquel Nebot](https://miquelnebot.es).

### Solución actividad MD03 Actividad 01 (opcional)
````Python
# Variables
texto = ('Nacido en 1564 en Pisa, Galileo Galilei fue un astrónomo y físico italiano cuyas contribuciones revolucionaron la ciencia. Su telescopio permitió observaciones que desafiaron las creencias establecidas, confirmando el modelo heliocéntrico de Copérnico. Sin embargo, sus descubrimientos le valieron conflictos con la Iglesia Católica, que lo consideró hereje. A pesar de su persecución, persistió en sus investigaciones y sentó las bases de la física moderna, dejando un legado duradero en el avance científico.')
# Ejecución
print(texto.find('Galileo'))
````

### Solución actividad MD03 Actividad 02
````Python
# Variables
historia = ('Hoy les contaré una emocionante historia sobre la antigua civilización de los egipcios. Fijaos bien, porque este relato está lleno de misterio y aventuras. Hace miles de años, en tierras lejanas del valle del Nilo, los egipcios construyeron grandes pirámides para honrar a sus faraones. Fijaos en esas enormes estructuras que desafiaban el tiempo, ¡eran impresionantes! En el antiguo Egipto, el río Nilo era fundamental para la vida de su pueblo. Fijaos cómo las aguas del Nilo inundaban las tierras y dejaban un fértil limo que permitía cultivar sus alimentos. Gracias a ello, los egipcios prosperaban. Una de las cosas más asombrosas de los egipcios era su escritura jeroglífica. Fijaos en esos símbolos que representaban objetos y sonidos. A través de ellos, los egipcios dejaron registrada su historia y conocimiento. Además, fijaos en las momias, que eran cuerpos preservados mediante un proceso especial. Los egipcios creían en la vida después de la muerte y preparaban a sus difuntos para esa nueva etapa. La vida en el antiguo Egipto también estaba llena de dioses y diosas. Fijaos en Ra, el poderoso dios del sol, y en Isis, la diosa protectora. Los egipcios les rendían culto y les pedían su protección. ¡Qué interesante es la historia de los egipcios! Fijaos en cómo su legado ha perdurado a lo largo de los siglos. Hoy podemos aprender sobre su cultura y admirar las maravillas que dejaron atrás. Espero que hayáis disfrutado de esta historia llena de misterios y curiosidades. Fijaos en los detalles y seguid explorando el fascinante mundo de la historia. ¡Hasta la próxima aventura!')
repeticion = ('fijaos')

# Ejecución
print('El término',repeticion,'se ha repetido ',historia.count('fijaos'),'veces.')
````
❗ Como vemos, el error es notable y gracias a él propondremos la corrección del código en la actividad siguiente 👇.  

### Solución actividad MD03 Actividad 03
```python
# Variables
historia = ('Hoy les contaré una emocionante historia sobre la antigua civilización de los egipcios. Fijaos bien, porque este relato está lleno de misterio y aventuras. Hace miles de años, en tierras lejanas del valle del Nilo, los egipcios construyeron grandes pirámides para honrar a sus faraones. Fijaos en esas enormes estructuras que desafiaban el tiempo, ¡eran impresionantes! En el antiguo Egipto, el río Nilo era fundamental para la vida de su pueblo. Fijaos cómo las aguas del Nilo inundaban las tierras y dejaban un fértil limo que permitía cultivar sus alimentos. Gracias a ello, los egipcios prosperaban. Una de las cosas más asombrosas de los egipcios era su escritura jeroglífica. Fijaos en esos símbolos que representaban objetos y sonidos. A través de ellos, los egipcios dejaron registrada su historia y conocimiento. Además, fijaos en las momias, que eran cuerpos preservados mediante un proceso especial. Los egipcios creían en la vida después de la muerte y preparaban a sus difuntos para esa nueva etapa. La vida en el antiguo Egipto también estaba llena de dioses y diosas. Fijaos en Ra, el poderoso dios del sol, y en Isis, la diosa protectora. Los egipcios les rendían culto y les pedían su protección. ¡Qué interesante es la historia de los egipcios! Fijaos en cómo su legado ha perdurado a lo largo de los siglos. Hoy podemos aprender sobre su cultura y admirar las maravillas que dejaron atrás. Espero que hayáis disfrutado de esta historia llena de misterios y curiosidades. Fijaos en los detalles y seguid explorando el fascinante mundo de la historia. ¡Hasta la próxima aventura!')
historia_lower = historia.lower()
repeticion = ('fijaos')
# Ejecución
print('La palabra',repeticion,'se ha repetido',historia_lower.count(repeticion),'veces.')
```
