# APUNTES-TERCER-CORTE-DINAMICA-DE-SISTEMAS-
# Función de transferencia:
La función de transferencia es una representación matemática utilizada en sistemas de control. Se obtiene a partir de la transformada de 
Laplace de una ecuación diferencial, considerando todas las condiciones iniciales en cero. Esta función es una herramienta 
fundamental en la teoría de control y en la dinámica de sistemas. Sirve para analizar y diseñar sistemas que procesan señales de entrada 
para producir una respuesta deseada en la salida.
## principales usos :
## 1. Modelado de sistemas:
   - Permite representar sistemas dinámicos lineales de tiempo invariante (LTI) en el dominio de la frecuencia.

   - Facilita el paso de las ecuaciones diferenciales del sistema al dominio de Laplace.
## 2. Análisis del Comportamiento del Sistema:

   - Respuesta transitoria: Describe cómo el sistema reacciona a cambios iniciales o perturbaciones.
   - Respuesta en estado estacionario: Muestra el comportamiento del sistema cuando alcanza una condición estable.
## 3. Diseño de Controladores:
   - Ayuda a diseñar controladores como PID (Proporcional, Integral y Derivativo) para mejorar la estabilidad, la precisión y la velocidad del sistema.

## clasificacion de las funciones de transferencia:

una funcion de transferencia se puede expresar como :
$$G(s) = \frac{Y(s)}{U(s)}$$
Donde:
   - Y(S):Salida en el dominio de laplace
   - U(S):Entrada en el dominio de laplace
## Clasificación:
   - Estrictamente propia: 𝑚>𝑛(grado del denominador mayor al numerador).
   - Bipropia: 𝑚=𝑛
   - Impropia: 𝑛>𝑚
## Polos y Zeros

   - Zeros: Valores de 𝑠 que anulan el numerador.
   - Polos: Valores de 𝑠 que anulan el denominador.

![image](https://github.com/user-attachments/assets/a48ffa60-af40-4f41-a340-b4c8a9aad4c0)

## EJEMPLO:

![12776c7f-fcf4-4a77-a7c5-32e7e309bf69](https://github.com/user-attachments/assets/a0fc2373-c184-4985-8688-e927cc466c20)

![2015c0f4-bc22-4b06-9ceb-e055bc75aa34](https://github.com/user-attachments/assets/612f59af-9b8f-4a9d-b41d-d314d5452676)

# Álgebra de Bloques

El álgebra de bloques es una herramienta esencial en el análisis de sistemas de control, que permite modelar y simplificar 
sistemas complejos mediante diagramas de bloques. Estos diagramas representan visualmente cómo las diferentes partes de un 
sistema interactúan entre sí.

## Elementos clave de un diagrama de bloques
   - Bloque funcional: Representa operaciones matemáticas realizadas en la señal de entrada para obtener la salida.
     
     ![image](https://github.com/user-attachments/assets/baf5fc7e-29f5-4b5f-beb0-8583c0700c0c)

   - Flechas: Indican la dirección del flujo de señales, mostrando la relación de entrada y salida.

     ![image](https://github.com/user-attachments/assets/c9a11b9b-3939-4274-a98f-1ba292384a9f)

   - Punto de suma: Combina señales mediante suma o resta. Las unidades deben coincidir.
     
     ![image](https://github.com/user-attachments/assets/5f701348-984b-4004-b864-24398a253539)

   - Punto de ramificación: Permite que una señal se dirija simultáneamente a múltiples bloques.
     
     ![image](https://github.com/user-attachments/assets/2c5bb518-6af1-4303-94cc-3cecac318520)

## Aplicaciones del álgebra de bloques

   - Obtener la función de transferencia de sistemas complejos, simplificando conexiones en serie, paralelo y retroalimentación.
   - Analizar la estabilidad del sistema mediante la ubicación de polos y zeros.
   - Diseñar controladores ajustando la retroalimentación, usualmente negativa, para mejorar el rendimiento del sistema.

## Propiedades fundamentales 
   - Cascada: Si dos bloques estan conectados en serie, sus funciones de transferencia se multiplican 

$$G total(s)=G1(s)⋅G2(s)$$

   - Retroalimentación negativa: Permite reducir el efecto de perturbaciones y aumentar la estabilidad:

$$G total(s)= \frac{G(s)}{1+G(s)H(s)}$$
​

Desde mi perspectiva, el uso de diagramas de bloques no solo simplifica la representación de sistemas complejos, sino que también 
hace más intuitivo el análisis del comportamiento del sistema. Es fascinante cómo, a través de esta herramienta gráfica, se puede 
entender la dinámica interna sin necesidad de profundizar en cada ecuación diferencial involucrada.

Además, el álgebra de bloques resalta la importancia de la retroalimentación negativa en los sistemas de control, un principio clave 
que está presente en muchas aplicaciones industriales y tecnológicas. En mi experiencia, trabajar con estos diagramas hace que el diseño 
y la optimización de sistemas se convierta en una tarea más manejable y visualmente comprensible.

Finalmente, aunque puede parecer un tema abstracto al inicio, su aplicación práctica en la resolución de problemas reales, como el control 
de procesos industriales o la regulación automática en sistemas electrónicos, demuestra su relevancia.

## Ejemplo 1:

![544ccf89-8ea2-4bdf-9552-cafd58748a97](https://github.com/user-attachments/assets/1991b694-eed9-4b4a-9f1a-ea88101bc5ea)

## Ejemplo 2:

![acf802b5-a071-4465-89cf-dd9cebf84190](https://github.com/user-attachments/assets/8127b774-9522-432f-9a9f-1c864696ed33)
![0bd67088-cdc4-43fa-9e50-fc355a007bc3](https://github.com/user-attachments/assets/f92f1476-afc7-4f0c-b645-218a6f09e5ce)

# Diagramas de flujo de señales 
Los diagramas de flujo de señales son una herramienta gráfica utilizada en la dinámica de sistemas para representar las relaciones entre las 
variables de un sistema complejo. A diferencia de los diagramas de bloques, estos diagramas facilitan el cálculo de la función de transferencia 
total de un sistema, utilizando la fórmula de Mason.

Elementos clave de los diagramas de flujo de señales
Nodos: Representan las variables del sistema (entrada o salida) y se indican con un círculo etiquetado.
![image](https://github.com/user-attachments/assets/e223dfcf-a7e3-45eb-93f3-04abbc2fb09a)

Flechas: Indican la relación entre variables, incluyendo la función de transferencia asociada.
![image](https://github.com/user-attachments/assets/6701d779-d273-4312-b4d3-87e0b385b204)

## Lazos y Trayectorias:
Camino directo: Conecta un nodo de entrada con uno de salida sin cruzar nodos repetidos.
Lazo cerrado: Camino que regresa al nodo inicial sin repetir otros nodos.
Fórmula de Mason
La fórmula de Mason permite calcular la función de transferencia total 

T(s) de un sistema complejo:

$$𝑇(𝑠)= \frac{∑PkΔk}{Δ}$$
​
​
 
Donde:
 - Pk: Ganancia de cada camino directo.
 - Δ: Determinante general del sistema.
 - Δk: Determinante que excluye los lazos que afectan al camino directo Pk.


![download](https://github.com/user-attachments/assets/bce56f20-e084-48c0-b485-efec54efce01)

![image](https://github.com/user-attachments/assets/79c56fc0-f263-456b-b67c-62ab68b8176f)
## Ejemplo:
![f607b15a-269d-4d65-99a0-81627be93eaf](https://github.com/user-attachments/assets/093ebbf5-bb51-486b-8e4c-5468b0c3203e)

Desde mi perspectiva, los diagramas de flujo de señales son una mejora considerable frente a los diagramas de bloques 
en sistemas complejos. Su estructura ordenada y la sistematicidad de la fórmula de Mason reducen la probabilidad de errores 
al manejar sistemas con múltiples interacciones.

Lo que encuentro más interesante es cómo esta herramienta conecta conceptos visuales con cálculos formales. En mi experiencia,
resulta valiosa tanto para estudiantes como para profesionales que trabajan con modelos de control, permitiendo una comprensión 
más profunda y efectiva de los sistemas.

con el diagrama de flujo de señales es mas rapido llegar a la funcion de tranferencia unicamente se debe tenr en cuenta la 
identificacion de la trayectoria o trayectorias y aplicar bien la formula de mason












