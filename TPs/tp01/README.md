# Degrees of Separation

Este proyecto implementa un algoritmo para calcular el grado de separación entre dos personas en la industria cinematográfica utilizando búsqueda en grafos.

## Contenido del Repositorio

### Estructura de Archivos
  `data/` Hace referencia al directorio donde se encuentran los .csv con la información necesaria. En este repo puede hacer referencia a `large/` o `small/`
- `data/people.csv`: Contiene información sobre personas como su ID, nombre y fecha de nacimiento.
- `data/movies.csv`: Contiene detalles de las películas, incluyendo su ID, título y año de lanzamiento.
- `data/stars.csv`: Relaciona las personas con las películas en las que han participado.

## Funcionalidades

- Cálculo del grado de separación entre dos personas en la industria cinematográfica.
- Interfaz de consola para ingresar los nombres de las personas de interés.
- Visualización de la ruta y películas que conectan a las dos personas.

## Archivo `util.py`

### Clase `Node`

La clase `Node` representa un nodo en el grafo. Cada nodo tiene un estado, un nodo padre y una acción que condujo a este nodo.

#### Funcionalidades:
- `__init__(self, state, parent, action)`: Inicializa un objeto `Node` con un estado, un nodo padre y una acción.

### Clase `StackFrontier` y `QueueFrontier`

Estas clases implementan la frontera para la búsqueda en grafos. `StackFrontier` utiliza una estructura de pila, mientras que `QueueFrontier` utiliza una cola.

#### Funcionalidades:
- `__init__(self)`: Inicializa la frontera.
- `add(self, node)`: Agrega un nodo a la frontera.
- `contains_state(self, state)`: Verifica si la frontera contiene un estado específico.
- `empty(self)`: Verifica si la frontera está vacía.
- `remove(self)`: Elimina y devuelve un nodo de la frontera.

### Requisitos
Python 3.x
Bibliotecas: No se requieren bibliotecas adicionales
### Instrucciones de Uso
Clona el repositorio: git clone https://github.com/mrtn-c/IA-TPs-Cometta.git
Navega al directorio del proyecto: cd tp01
Ejecuta el programa: python degrees.py
Sigue las instrucciones en consola para ingresar los nombres de las dos personas y visualizar el grado de separación.

