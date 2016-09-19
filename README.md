# ZoraidaMediavillaTFG
Este código corresponde sólo a la parte de control y recogida de datos del prototipo.

Los archivos test_ corresponden a los ficheros de prueba de cada componente. Con éstos se comprueba que cada elemento funciona por separado para saber si hay algún problema con alguno.

El fichero calibrate_motors.py sirve para igualar la potencia de los dos motores para que vaya lo más recto posible el robot. Con el valor x de ChangeDutyCycle(x) se ajusta la velocidad para el motor A y el B.

El archivo reduce_picture.py crea un fichero que transforma el original pero con la reducción de píxeles correspondiente. En la línea 8 se puede variar la dimensión de la matriz a reducir.

Los ficheros restantes corresponden a alojados en el servidor web y utilizados por el controlador. El index.html presenta una pantalla con los botones a utilizar para el manejo del robot y el controlador.py o el controlador_save_data.py implementan las funciones para que ese control se haga efectivo. La diferencia entre el controlador.py y el controlador_save_data.py es que el segundo incorpora un thread daemon que se encarga de guardar todos los datos recogidos en un fichero txt. También se crea un fichero de log por si ocurriera algún problema saber donde ocurrió.
