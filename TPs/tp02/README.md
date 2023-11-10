###Minesweeper AI
Este proyecto implementa el clásico juego de Buscaminas junto con un agente de inteligencia artificial (IA) que puede jugar automáticamente o asistir al jugador.

###Contenido del Repositorio
Estructura de Archivos
assets/fonts/OpenSans-Regular.ttf: Fuente utilizada para la interfaz gráfica.
assets/images/flag.png: Icono de bandera para marcar celdas como minas.
assets/images/mine.png: Icono de mina para mostrar cuando se revela una mina.
minesweeper.py: Implementación del juego Buscaminas y la lógica de la IA.
runner.py: Interfaz gráfica del juego que utiliza la implementación de Buscaminas e IA.
##Funcionalidades
Juego de Buscaminas: Interfaz gráfica que permite al jugador jugar al Buscaminas clásico.
IA para Buscaminas: Una IA que puede jugar automáticamente al Buscaminas o asistir al jugador tomando decisiones seguras.
Archivo minesweeper.py
Clase Minesweeper
La clase Minesweeper representa el juego Buscaminas.

#Funcionalidades:
__init__(self, height=8, width=8, mines=8): Inicializa el juego con una altura, ancho y número de minas predeterminados.
print(self): Muestra una representación en texto de la ubicación de las minas.
is_mine(self, cell): Devuelve True si la celda es una mina, False de lo contrario.
nearby_mines(self, cell): Devuelve el número de minas adyacentes a una celda.
won(self): Verifica si todas las minas han sido marcadas.

###Clase Sentence
La clase Sentence representa una declaración lógica sobre el juego Buscaminas.

##Funcionalidades:
__init__(self, cells, count): Inicializa una sentencia con un conjunto de celdas y un recuento de minas.
known_mines(self): Devuelve el conjunto de celdas conocidas como minas según la sentencia.
known_safes(self): Devuelve el conjunto de celdas conocidas como seguras según la sentencia.
mark_mine(self, cell): Actualiza la representación de conocimiento cuando se conoce que una celda es una mina.
mark_safe(self, cell): Actualiza la representación de conocimiento cuando se conoce que una celda es segura.

###Clase MinesweeperAI
La clase MinesweeperAI representa el jugador de Buscaminas automático.

##Funcionalidades:
__init__(self, height=8, width=8): Inicializa la IA con una altura y ancho predeterminados.
mark_mine(self, cell): Marca una celda como mina y actualiza el conocimiento.
mark_safe(self, cell): Marca una celda como segura y actualiza el conocimiento.
add_knowledge(self, cell, count): Agrega conocimiento basado en la celda y el recuento proporcionados.
make_safe_move(self): Realiza un movimiento seguro si es posible.
make_random_move(self): Realiza un movimiento aleatorio si es posible.
##Requisitos
Python 3.x
Bibliotecas: Se requiere la instalación de pygame. Puedes instalar las dependencias ejecutando pip install -r requirements.txt.
Instrucciones de Uso
Clona el repositorio: git clone https://github.com/mrtn-c/IA-TPs-Cometta.git
Navega al directorio del proyecto: cd tp02
Instala las dependencias: pip install -r requirements.txt
Ejecuta el juego: python runner.py
Sigue las instrucciones en la interfaz gráfica para jugar al Buscaminas. La IA también puede asistirte si decides utilizarla.

¡Diviértete jugando al Buscaminas!
