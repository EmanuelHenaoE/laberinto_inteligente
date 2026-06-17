#Laberinto Inteligente

## Descripción

Este proyecto implementa un solucionador de laberintos utilizando la técnica de **Backtracking**. El algoritmo explora diferentes caminos desde una posición inicial hasta encontrar la salida. Cuando llega a un callejón sin salida, retrocede automáticamente para probar rutas alternativas, simulando el comportamiento de exploración inteligente en videojuegos y sistemas de búsqueda.

## Objetivo

Encontrar un camino desde la entrada (`S`) hasta la salida (`G`) en un laberinto representado como una matriz.

## Representación del Laberinto

- `S`: posición inicial.
- `G`: salida.
- `#`: pared.
- `.`: camino libre.
- `*`: camino encontrado.
##Solución parcial

Las posiciones recorridas hasta el momento.

##Candidatos

Movimientos posibles desde la posición actual:

Arriba
Abajo
Izquierda
Derecha
Restricciones
No atravesar paredes (#)
No salir de los límites de la matriz
No visitar una celda más de una vez

##Solución completa

Se alcanza cuando la posición actual coincide con la salida (G).

##Retroceso

Si desde una posición no existen movimientos válidos, el algoritmo regresa a la posición anterior para probar otro camino.

##Poda

Se evita volver a visitar celdas ya exploradas para reducir búsquedas innecesarias.
