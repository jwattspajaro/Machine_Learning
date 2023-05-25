Reducción de la pérdida: Tasa de aprendizaje 

bookmark_border
Tiempo estimado: 5 minutos
Como se señaló, el vector de gradiente tiene una dirección y una magnitud. 
Los algoritmos de descenso de gradientes multiplican el gradiente por un escalar conocido como tasa de aprendizaje 
(a veces llamado tamaño del paso) para determinar el siguiente punto. Por ejemplo, 
si la magnitud de la gradiente es 2.5 y la tasa de aprendizaje es 0.01, el algoritmo de descenso de gradientes elegirá el siguiente punto a 0.025 del punto anterior.

Los hiperparámetros son los controles que los programadores ajustan en los algoritmos de aprendizaje automático. 
La mayoría de los programadores de aprendizaje automático pasan bastante tiempo ajustando la tasa de aprendizaje. 
Si eliges una tasa de aprendizaje muy pequeña, el aprendizaje tardará demasiado:
![image](https://github.com/jwattspajaro/Machine_Learning/assets/18930760/0d977e97-8745-46c7-b6a7-a936b98032a6)

Figura 6: La tasa de aprendizaje es demasiado baja.

Por el contrario, si especificas una tasa de aprendizaje demasiado grande, el siguiente punto rebotará perpetuamente en la parte inferior del pozo, 
como un experimento de mecánica cuántica que salió muy mal:
![image](https://github.com/jwattspajaro/Machine_Learning/assets/18930760/cccebcc3-c117-4a56-a710-7991d6d39ca9)

Figura 7: La tasa de aprendizaje es demasiado alta.

Hay una tasa de aprendizaje con valor dorado para cada problema de regresión. 
El valor dorado está relacionado con qué tan plana es la función de pérdida. 
Si sabes que el gradiente de la función de pérdida es pequeño, 
puedes probar de forma segura una tasa de aprendizaje mayor, 
que compensa el pequeño gradiente y da como resultado un tamaño de paso más grande.
![image](https://github.com/jwattspajaro/Machine_Learning/assets/18930760/71c8da2c-c90a-48d8-a1a3-092ef0e352af)

### Términos clave
-  **[hiperparámetro](https://developers.google.com/machine-learning/glossary?hl=es-419#hyperparameter)**
-  **[tasa de aprendizaje](https://developers.google.com/machine-learning/glossary?hl=es-419#step_size)**
-  **[tamaño del paso](https://developers.google.com/machine-learning/glossary?hl=es-419#learning_rate)**


