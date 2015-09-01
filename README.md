# Matematica para todos

Repositorio de la nueva versión de Matemática para todos

# Valores a modificar según latencia de la red
Si se observa que en el listado de amigos, un usuario que no se desconecto, aparece y desaparece se deben subir
los valores nodo_timeout = 6000; y master_timeout = 8000; El valor del master_timeout siempre debe ser igual o mayor al valor del nodo_timeout. Se recomienda mantener estos valores lo más bajo posible.

Las pruebas realizadas en una red hogareña necesitan un valor de nodo_timeout=6000; para mantener la estabilidad. Se realizaron otras pruebas en redes con mayores accesos y se necesito un valor de nodo_timeout = 12000; para mantener la estabilidad.

Todas las pruebas se realizaron con una maquina virtual y dos netbooks.


# Modificaciones en cuanto a la versión inicial

- Se elimino todo lo relacionado a avahi y se implemento la libreria del discover de nodos
- Se modifico casi totalmente el server.js, solo se utilizaron los eventos relacionados al momento del juego
- Se modifico que ambos juegos se cierren si un oponente se desconectaba, actualmente vuelve al listado de amigos
- Se soluciono problema de que en el tiempo de timeout un jugador intenten conectarse con otro que ya esta jugando
- Se agrego focus en el input del formulario de inicio
- Se modifico el formulario de inicio para que funcione aprentando ENTER
- Se agrego el cursor POINTER a todos los enlaces



