# Analisis *in silico* de los circuitos de regulación de los linfocitos T CD4+ y su relación con la plasticidad durante la diferenciación celular 
## Introducción
La plasticidad fenotípica se define como el potencial de una célula ya diferenciada para alcanzar otros estados celulares o funcionales, como respuesta a alteraciones intrínsecas o extrínsecas (Martinez-Sanchez et al, 2015). Esta plasticidad es inherente al proceso de diferenciación de los linfocitos T CD4+ ante los cambios en el microambiente, por lo que son capaces de cambiar de tipo celular para tener una respuesta inmune adaptativa (Friedman et al, 2023) siendo  esenciales para responder contra diversos patógenos (Martinez-Sanchez et al, 2015). Estas células se originan como linfocitos vírgenes o Th0 y, ante un antígeno y un entorno de citocinas específico, se diferencian en diversos tipos celulares especializados, como Th1, Th2, Th17, iTreg y Tfh (Martinez-Sanchez et al, 2015). Anteriormente, esta determinación del tipo celular se consideraba como un proceso rígido; sin embargo, la evidencia actual demuestra una alta plasticidad lo que permite a las células cambiar de un tipo a otro, lo cual se ha identificado como un proceso importante para la adaptación dinámica del sistema inmune (Friedman et al, 2023). 

Los fenómenos biológicos no son estáticos, sino el resultado de redes complejas donde genes, proteínas y citocinas interactúan de forma no lineal, es decir, son altamente dinámicos (Martinez-Sanchez, 2018). Verlo de esta forma facilita el estudio de cómo estas interacciones moleculares dan origen a comportamientos a nivel celular. El estudio de estas redes de regulación permite integrar la información molecular para predecir fenotipos celulares y entender cómo las perturbaciones pueden afectar el destino de la célula (Martinez-Sanchez, 2018), además han sido ampliamente utilizadas para el estudio de diferentes casos a distintos niveles así como de regulación genética, redes neurobiológicas, redes ecológicas, entre otros (Milo et al, 2022).

Estas interacciones son representadas como una red, donde los nodos representan componentes (proteínas, citocinas, etc.) y las aristas representan las interacciones regulatorias (activación o inhibición) (Domínguez-Huttinger y Martínez-Sánchez, s.f.). Dentro de estas redes, existen circuitos funcionales clave como la autoactivación que suelen estar asociadas a la estabilidad, la inhibición mutua entre linajes celulares excluyentes y los bucles de retroalimentación (Feed-forward loops) siendo motivos de la red donde un factor de transcripción X regula a un segundo factor Y, y ambos regulan conjuntamente a un gen objetivo Z (Milo et al, 2022). Estos circuitos son esenciales para el procesamiento de información en los sistemas biológicos, ya que permiten a las células responder adecuadamente a su entorno. 

El modelo de redes booleanas permite estudiar la dinámica de este tipo de sistemas. En este modelo cada nodo tiene un valor de 1 (activo) o 0 (inactivo), las aristas tienen valores de 1(activación) y -1 (Inhibición), y su estado en el tiempo t+1 depende de una función lógica de sus reguladores en el tiempo t (Martinez-Sanchez, 2018). A través de la evaluación de las funciones de la red, es posible obtener los estados estables (puntos fijos o ciclos) a los que una red tiende a converger. Estos estados son denominados atractores. Los atractores pueden representar diferentes tipos celulares y otros procesos biológicos. La robustez de una red es definida por la plasticidad y estabilidad de los atractores. Un sistema se considera estable si, tras una perturbación transitoria, la red regresa al mismo atractor. Por el contrario, un sistema se considera plástico si la perturbación provoca la transición hacia un atractor diferente. 

Por medio de estas redes booleanas se pretende modelar los circuitos de regulación de los linfocitos T CD4+ con el propósito de explorar su relación con la plasticidad de los linfocitos T CD4+, realizando subredes que comparen las interacciones entre dos subtipos celulares. Estas serán analizadas de forma que se compare la plasticidad descrita de los linfocitos T CD4+ con las propiedades topológicas, los atractores y la robustez a perturbaciones de las subredes. 

##Metodología 

Se utilizaron redes booleanas para representar las distintas subredes entre los tipos de linfocitos de las T CD4+, por medio del software yEd. Las lineas rojas representan inhibición y las flechas negras indican activación.

Quedando de la siguiente manera:

1. Th1 (verde) vs Th2 (azul) <img width="568" height="495" alt="Th1vsTh2" src="https://github.com/user-attachments/assets/cdfae5c2-4462-4779-84e1-ad980b20c6a4" />
2. Th1 (verde) vs Th17 (rosa)  <img width="568" height="495" alt="Th1vsTh17" src="https://github.com/user-attachments/assets/72a6d99f-1b19-4805-a44a-19c921595b93" />
3. Th1 (verde) vs iTreg (morado) <img width="568" height="495" alt="Th1vsiTreg" src="https://github.com/user-attachments/assets/5010bad0-2a48-4c1f-8d93-d48ba14c78ed" /> 
4. Th2 (azul) vs Th17 (rosa) <img width="568" height="495" alt="Th2vsTh17" src="https://github.com/user-attachments/assets/13ab3ab8-c418-41e7-987f-433a05ab1f41" />
5. Th2 (azul) vs iTreg (morado) <img width="568" height="495" alt="Th2vsiTreg" src="https://github.com/user-attachments/assets/465bbad3-a2b3-4a7c-8e7d-f0ef14fed906" />
6. Th17 (rosa) vs iTreg (morado) <img width="568" height="495" alt="Captura de pantalla 2026-04-19 a la(s) 11 31 33 p m" src="https://github.com/user-attachments/assets/f4e7281e-a5d2-4a68-b644-3169b60ca1df" />

Estas subredes fueron exportadas en formato .graphml, sin embargo fue necesario agregar etiquetas a cada uno de los nodos y el valor de la interacción (1 o -1) a cada una de las flechas anterior a la exportación del archivo. De esta forma el programa yEd guarda esta información necesario para el analisis de las subredes. 

###Analisis de las subredes


   






