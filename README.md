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

3. **q2_time**
   - All lines from the JSON file are read into memory at once
   - Reading the entire file into memory reduces disk access time compared to reading line by line.

4. **q2_memory**
   - JSON data is processed line by line without loading the entire file into memory at once
   - minimizes memory usage because it processes one line of JSON data at a time, which doesn't require storing the entire file content in memory

5. **q3_time**
   - Descripción: Identifica los 10 usuarios más influyentes históricamente basados en el número de menciones (@) que reciben en los tweets.
   - Archivo: `q3_time.py`
   - Firma de la Función: `def q3_time(file_path: str) -> List[Tuple[str, int]]`

6. **q3_memory**
   - Descripción: Implementación alternativa de q3_time optimizada para el uso de memoria.
   - Archivo: `q3_memory.py`
   - Firma de la Función: `def q3_memory(file_path: str) -> List[Tuple[str, int]]`

## Differences Between Optimizations for Time and Memory

**Optimization for Execution Time:**
   - Uses efficient data structures and algorithms to minimize execution time.
   - Processes data quickly at the expense of potentially higher memory usage.
   - More suitable for scenarios where processing speed is critical and memory constraints are less strict.

**Optimization for Memory Usage:**
   - Minimizes memory usage at the expense of potentially longer execution time.
   - Prioritizes efficient memory management and conservative data storage.
   - Ideal for scenarios where memory constraints are tight, and processing speed can be sacrificed for reduced memory footprint.
