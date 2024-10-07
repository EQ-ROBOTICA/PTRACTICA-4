# PRACTICA-4

## Introducción
Esta práctica consiste en la implementación de la dinámica robótica mediante coordenadas para realizar una acción específica. El objetivo es utilizar el robot Epson C4 para tomar cuatro placas diferentes y apilarlas una sobre otra en una posición determinada, de manera continua y con precisión.

## Instrucciones
### Programación de coordenadas

Se utilizó el software Epson RC+ para definir las coordenadas esenciales para el movimiento del robot. Se establecieron tres puntos clave: "Primera", "Segunda" y "Caja". Registrar estos puntos fue crucial para asegurar un desplazamiento seguro y eficiente, evitando colisiones con el entorno.

### Programación final mediante código

A diferencia de prácticas anteriores, en esta ocasión se empleó el tipo de dato integer, que se usa para representar números enteros. Esto es útil en diversas situaciones, como contar iteraciones, manejar índices de arreglos o realizar operaciones aritméticas que no requieren precisión decimal. En esta práctica, integer se utilizó específicamente para llevar un registro de cuántas veces se ha ejecutado un bucle, permitiendo controlar cuántas veces se desea realizar una acción determinada.

El código que se implementó para ejecutar la tarea es el siguiente:

```
Function main
Home
On 2

Integer i
For i = 0 To 3
    Go Primera
    Go Segunda
    Off 2
    Go Primera
    Home
    Go Caja +Z(i * 12)
    On 2
    Home
Next
Fend
```

El proceso comienza en el punto "Home", donde se activa la garra. Se establece la variable i como un entero e inicializa un bucle For desde i=0 hasta 3, repitiendo el proceso de movimiento cuatro veces. En cada iteración, el robot se desplaza a los puntos "Primera" y "Segunda" para recoger una placa, vuelve a "Home" para asegurar el movimiento, y luego se dirige a "Caja", aumentando la altura en el eje Z en 12 mm por iteración. Este valor corresponde al grosor de la placa, permitiendo que el robot apile correctamente las placas una sobre otra.

## Conclusiones
- *Edgar Zahid Hernandez Garcia:*
La implementación de bucles en la programación de movimientos facilita significativamente el código para realizar acciones repetitivas, evitando la redundancia de órdenes y agilizando el proceso.

- *Gael Mateo Rangel Chavez:*

  
- *Alejandro Saldaña Garcia:*
  
## Referencias bibliográficas


