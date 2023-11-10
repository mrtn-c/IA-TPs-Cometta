### Juego Nim con Inteligencia Artificial mediante Q-learning
##Descripción
Este proyecto implementa un juego simple de Nim junto con un jugador de inteligencia artificial que utiliza Q-learning para la toma de decisiones. Nim es un juego matemático en el que los jugadores se turnan para quitar objetos de montones o pilas distintas. El jugador que quita el último objeto gana.

#Archivos en el Repositorio
nim.py: Implementación del juego Nim y del jugador de inteligencia artificial.
play.py: Script para entrenar la inteligencia artificial y jugar partidas.
README.md: Este archivo.
nim.py - Implementación del Juego Nim

##Clase Nim
Representa el tablero de juego Nim. Realiza un seguimiento de los montones, el jugador actual y el ganador. Maneja los movimientos de los jugadores y las actualizaciones del estado del juego.

##Clase NimAI
Implementa un jugador de inteligencia artificial para Nim utilizando Q-learning. Utiliza un diccionario de Q-learning para almacenar los valores Q de los pares estado-acción. Maneja la actualización de los valores Q en función de las recompensas y las estimaciones futuras. Elige acciones de manera avara o mediante una estrategia épsilon-greedy.

##play.py - Entrenamiento y Juego
Función train(n)
Entrena el NimAI jugando n partidas contra sí mismo. Actualiza los valores Q en función de los resultados de cada partida.

Función play(ai, human_player=None)
Permite que un jugador humano juegue contra el NimAI entrenado. Muestra el estado actual de los montones y guía al jugador en su turno. Determina al ganador e imprime el resultado al final del juego.

##Cómo Usar
Ejecuta train(10000) en play.py para entrenar a la IA jugando 10,000 partidas.
Ejecuta play(ai) para jugar una partida contra la IA entrenada.

##Requisitos
Python 3.x

#Nota:
Asegúrate de que los módulos time y random estén disponibles en tu entorno de Python. Siéntete libre de personalizar y mejorar el código según sea necesario para tu comprensión y exploración adicional.
