### Regresión lineal 

#### bookmark_border
Tiempo estimado: 6 minutos
**Hace mucho tiempo se sabe que los grillos (una especie de insecto) cantan con más frecuencias en los días de más calor. Durante décadas, científicos profesionales y aficionados han catalogado datos sobre cantos por minuto y temperatura. Como regalo de cumpleaños, tu tía Ruth te da su base de datos de críquet y te pide que aprendas un modelo para predecir esta relación. Con estos datos, desea explorar esta relación.**

Primero, examina tus datos mediante un trazado:
![image](https://github.com/jwattspajaro/Machine_Learning/assets/18930760/abd90c7b-93bb-4f91-be90-0a275db2f4a0)

### Figura 1 Cantos por minuto contra temperatura en grados Celsius

Como era de esperar, la representación muestra que la cantidad de cantos aumenta. ¿Es lineal la relación entre los cantos y la temperatura? Sí, puedes dibujar una línea recta como la siguiente para aproximar esta relación:

![image](https://github.com/jwattspajaro/Machine_Learning/assets/18930760/e2ad4068-28ba-4fdb-a060-de159c530de0)

### Figura 2: Una relación lineal.

Si bien la línea no atraviesa todos los puntos, muestra la relación entre los cantos y la temperatura. Si usas la ecuación para una línea, puedes anotar esta relación de la siguiente manera:


<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mi>y</mi>
  <mo>=</mo>
  <mi>m</mi>
  <mi>x</mi>
  <mo>+</mo>
  <mi>b</mi>
</math>

 Donde:

* **y** es la temperatura en Celsius, el valor que intentamos predecir.
* **m** es la pendiente de la línea.
* **x** es la cantidad de cantos por minuto, el valor de nuestro atributo de entrada.
* **b** es la intersección en y.

Por convención en el aprendizaje automático, escribirás la ecuación de un modelo un poco diferente:

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <msup>
    <mi>y</mi>
    <mo>&#x2032;</mo>
  </msup>
  <mo>=</mo>
  <mi>b</mi>
  <mo>+</mo>
  <msub>
    <mi>w</mi>
    <mn>1</mn>
  </msub>
  <msub>
    <mi>x</mi>
    <mn>1</mn>
  </msub>
</math>

**Donde:**

 * **y'** es la **[etiqueta](https://developers.google.com/machine-learning/crash-course/framing/ml-terminology?hl=es-419#labels)** predicha (un resultado deseado).
 * **b** es el sesgo (la intersección en y), a veces denominado.
 * **w_1**es el peso del atributo 1. El peso es el mismo concepto que la pendiente 
* **m** en la ecuación tradicional de una línea.
* **X1** es un **[atributo](https://developers.google.com/machine-learning/crash-course/framing/ml-terminology?hl=es-419#features)** (una entrada conocida).
Para **inferir** (predecir) la temperatura **y'** para un nuevo valor de cantos por minuto **X1**, solo tienes que sustituir el valor **X1** en este modelo.

Aunque este modelo usa solo un atributo, un modelo más sofisticado podría basarse en varios atributos, cada uno con un peso diferente (
, 
, etc.). Por ejemplo, un modelo que se basa en tres atributos podría verse de la siguiente


<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <semantics>
    <mrow>
      <msup>
        <mi>y</mi>
        <mo>&#x2032;</mo>
      </msup>
      <mo>=</mo>
      <mi>b</mi>
      <mo>+</mo>
      <msub>
        <mi>w</mi>
        <mn>1</mn>
      </msub>
      <msub>
        <mi>x</mi>
        <mn>1</mn>
      </msub>
      <mo>+</mo>
      <msub>
        <mi>w</mi>
        <mn>2</mn>
      </msub>
      <msub>
        <mi>x</mi>
        <mn>2</mn>
      </msub>
      <mo>+</mo>
      <msub>
        <mi>w</mi>
        <mn>3</mn>
      </msub>
      <msub>
        <mi>x</mi>
        <mn>3</mn>
      </msub>
    </mrow>
    <annotation encoding="application/x-tex">y' = b + w_1x_1 + w_2x_2 + w_3x_3</annotation>
  </semantics>
</math>
