
# Temporizador-V2

Aplicación Every Minute On the Minute ( Versión WEB por componentes y manejo de usuarios.) 

Santiago Gómez Almeyda 20161020503

Jheisson Enrique Fortich Suarez 20172020049

Kevin Andres Malaver Cobos 20171020001


## Problemas en el modelo por Componentes:  
Fue difícil la implementación de este modelo ya que hubo confusiones respecto a como separar los modulos.  

1. El primer caso fue cuando simplemente apartamos el Javascript del temporizador pero el resultado fue incorrecto ya que para hacer uso de este en un proyecto futuro era necesario modificar el código fuente, lo que nos hizo percatar de un fuerte acoplamiento que corregismos posteriormente.

##Corrección al problema:
La solución que implementamos fue desacoplar el temporizador del resto del programa, y realzar un componente "temporizador" independiente (mediante el uso de clases) y luego crear otro archivo Javascript que utiliza este componente (lo extiende) y conecta el temporizador con la vista del framework en uso: Web2Py.
