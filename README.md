# FlotaRESTClient
Project from EI1021-Sistemas Distribuidos. Battleship client side REST WebService with JAX-RS

- ClienteFlotaWS.java: Clase que crea la interfaz gráfica, con referencia a GestorPartidas.java. Cada acción sobre la interfaz gráfia resultará en la invocación de algún método del gestor.

- GestorPartida.java: Clase que realiza las peticiones HTTP siguiendo la filosofía REST, consta de los siguientes métodos:
  - nuevaPartida: realiza una petición HTTP POST, como resultado el servidor nos devuelve la ruta donde guarda nuestra partida.
  - borraPartida: realiza una petición HTTP DELETE, como resultado el servidor nos devuelve el estado de la petición, si ha tenido exito o no.
  - pruebaCasilla: realiza una petición HTTP PUT, como resultado el servidor nos devuelve el resultado de disparar a la casilla.
  - getBarco: realiza una petición HTTP GET y consume text/plain, como resultado el servidor nos devuelve la String con las caracteristicas del barco.
  - getSolucion: realiza una petición HTTP GET y consume application/xml, como resultado el servidor nos devuelve las Strings que representan a todos los barcos.
