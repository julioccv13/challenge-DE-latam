# challenge-DE-latam
This repository contains Python functions for analyzing tweet data stored in JSON format. Each function is provided with an implementation

## Functions

1. **q1_time**
   - Parses the JSON file once and iterates over each line.
   - Uses separate dictionaries for storing tweet counts (tweet_count) and user tweet counts (user_tweets).
   - Combines loops for counting tweets and finding the user with the most tweets for each date.

2. **q1_memory**
   - Utilizes a defaultdict (date_user_count) to efficiently store tweet counts for each date and user.
   - Parses the JSON file once and updates the date_user_count dictionary directly.
   - Finds the top 10 dates with the most tweets and their corresponding users from the date_user_count dictionary.

2. **q2_time**
   - Descripción: Determina los 10 emojis más utilizados en el contenido de los tweets.
   - Archivo: `q2_time.py`
   - Firma de la Función: `def q2_time(file_path: str) -> List[Tuple[str, int]]`

3. **q3_time**
   - Descripción: Identifica los 10 usuarios más influyentes históricamente basados en el número de menciones (@) que reciben en los tweets.
   - Archivo: `q3_time.py`
   - Firma de la Función: `def q3_time(file_path: str) -> List[Tuple[str, int]]`



5. **q2_memory**
   - Descripción: Implementación alternativa de q2_time optimizada para el uso de memoria.
   - Archivo: `q2_memory.py`
   - Firma de la Función: `def q2_memory(file_path: str) -> List[Tuple[str, int]]`

6. **q3_memory**
   - Descripción: Implementación alternativa de q3_time optimizada para el uso de memoria.
   - Archivo: `q3_memory.py`
   - Firma de la Función: `def q3_memory(file_path: str) -> List[Tuple[str, int]]`

## Diferencias Entre Implementaciones Optimizadas para Tiempo y Memoria

- **Optimización para el Tiempo de Ejecución:**
  - Utiliza estructuras de datos y algoritmos eficientes para minimizar el tiempo de ejecución.
  - Procesa datos rápidamente a expensas de un uso potencialmente mayor de memoria.
  - Más adecuado para escenarios donde la velocidad de procesamiento es crítica y las restricciones de memoria son menos estrictas.

- **Optimización para el Uso de Memoria:**
  - Minimiza el uso de memoria a expensas de un tiempo de ejecución potencialmente más largo.
  - Prioriza una gestión eficiente de la memoria y un almacenamiento de datos conservador.
  - Ideal para escenarios donde las restricciones de memoria son ajustadas y la velocidad de procesamiento puede sacrificarse por una huella de memoria reducida.
