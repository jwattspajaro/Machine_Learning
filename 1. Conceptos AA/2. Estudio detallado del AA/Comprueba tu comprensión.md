Error cuadrático medio
Considera las siguientes representaciones:
---
![image](https://github.com/jwattspajaro/Machine_Learning/assets/18930760/18701232-e59d-4788-8d48-e4de97f681dc) 
Un gráfico de 10 puntos. Una línea atraviesa 6 de los puntos. 2 puntos equivalen a 1 	<img "units"=" 1=" 2=" <="" above=" alt="Una representación de 10 puntos. Una línea atraviesa 8 de los puntos. 1 punto equivale a 2 ;

Explora las siguientes opciones.

    ¿Cuál de los dos conjuntos de datos que se muestran en las representaciones anteriores tiene el error cuadrático medio (ECM) más alto?
    
 El conjunto de datos a la derecha
Los ocho ejemplos de la línea incurren en una pérdida total de 0. Sin embargo, aunque solo dos puntos están fuera de la línea, ambos están dos veces más alejados de la línea que los puntos de valores atípicos de la figura de la izquierda. La pérdida al cuadrado amplifica esas diferencias, de manera que una compensación de dos incurre en una pérdida cuatro veces mayor que una compensación de uno.

---

MSE = $\frac{0^2 + 0^2 + 0^2 + 2^2 + 0^2 + 0^2 + 0^2 + 2^2 + 0^2 + 0^2}{10} = 0.8$


✅ Correcto

----

El conjunto de datos a la izquierda.
Los seis ejemplos de la línea incurren en una pérdida total de 0. Los cuatro ejemplos que no están en la línea no están muy lejos de la línea, por lo que incluso el cuadrado de su desplazamiento aún produce un valor bajo:


MSE = $\frac{0^2 + 0^2 + 0^2 + 1^2 + 0^2 + 0^2 + 0^2 + 1^2 + 0^2 + 0^2}{10} = 0.4$

<span style="color:red">Vuelve a intentarlo</span>

---


