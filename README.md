# Proyecto: Sistema urinario

## Información de las estudiantes

Yoseline Lizeth Puentes Hernandez \[22212265]; l22212265@tectijuana.edu.mx

Nicole Zoe Camacho Quezada \[22211747]; l22211747@tectijuana.edu.mx

Modelado de Sistemas Fisiológicos

Ingeniería Biomédica

## Docente

Dr. Paul Antonio Valle Trujillo; paul.valle@tectijuana.edu.mx

Departamento de Ingeniería Eléctrica y Electrónica, Tecnológico Nacional de México/IT Tijuana, Blvd. Alberto Limón Padilla s/n, Tijuana, C.P. 22454, B.C., México.

## Descripción de la asignatura

El modelizado de sistemas fisiológicos es una herramienta importante en Ingeniería Biomédica, permite comprender el funcionamiento del cuerpo humano, así como diseñar y evaluar terapias y dispositivos médicos; se define como el proceso de formular modelos matemáticos o computacionales que representan el comportamiento y la interacción de los sistemas biológicos y fisiológicos. Esta asignatura pretende aportar al perfil del Ingeniero Biomédico la capacidad de realizar investigación científica en el área de Biología de Sistemas con la finalidad de dirigir y participar en equipos de trabajo interdisciplinarios en contextos nacionales e internacionales, así como de proporcionar soluciones informáticas para resolver problemas en el campo de la Ingeniería Biomédica con ética profesional; lo anterior al proporcionar al estudiante bases sólidas para modelizar sistemas y diseñar controladores para la solución de problemas en las áreas de atención médica y del sector industrial médico. La construcción de analogías entre circuitos eléctricos y sistemas fisiológicos para la formulación de modelos matemáticos y el diseño de controladores mediante la experimentación in silico brindan herramientas de gran aplicación en el quehacer profesional del Ingeniero Biomédico.

La asignatura de Modelado de Sistemas Fisiológicos forma parte del plan de estudios de la carrera en Ingeniería Biomédica con la siguiente competencia general del curso: Utiliza las propiedades de los circuitos RLC para describir la dinámica de sistemas fisiológicos, obtener modelos matemáticos y aplicar el control clásico, esto con el objetivo de integrar los principios de la Ingeniería de Control, la Electrónica Analógica y las Ciencias de la Computación con la Anatomía y Fisiología del cuerpo humano para proporcionar descripciones cuantitativas y cualitativas de sistemas fisiológicos complejos con el objetivo de modelizar, analizar, controlar, ilustrar y predecir su dinámica tanto en el corto como en el largo plazo.

## Objetivos

1. Construir el diagrama eléctrico.
2. Calcular la función de transferencia aplicando el principio de superposición.
3. Calcular el error en estado estacionario y la estabilidad en lazo abierto.
4. Emular y simular la respuesta del circuito en Simulink/Simscape a la señal impulso unitario.
5. Sintonizar las ganancias de un controlador PID para eliminar el error entre la entrada y la salida del sistema control-caso.
6. Obtener la respuesta en lazo abierto y en lazo cerrado con el controlador PID en MATLAB con la función de transferencia.

## Descripción detallada del sistema

El sistema urinario, específicamente el proceso de formación, conducción y almacenamiento de la orina desde los riñones hasta la vejiga, puede representarse mediante un modelo simplificado que captura la dinámica de presión y flujo del líquido urinario a lo largo de sus estructuras principales. Para describir este comportamiento mediante un circuito eléctrico equivalente de segundo orden, se consideran las siguientes suposiciones fisiológicas:
##Resistencia al flujo urinario
La dificultad que enfrenta la orina para desplazarse a través de los túbulos renales, los uréteres y los esfínteres se modela mediante un resistor R.
Esta resistencia representa: la oposición al avance del filtrado dentro de los túbulos renales,  fricción del líquido contra las paredes de los uréteres durante su conducción hacia la vejiga, resistencia generada por los esfínteres ureterales que regulan la salida del flujo.
En conjunto, la resistencia refleja la limitación fisiológica al flujo, que determina qué tan rápido o lento se desplaza la orina.

**Capacidad de almacenamiento de las vías urinarias**.

La distensibilidad de la vejiga se representa mediante un capacitor C. Este elemento modela la función principal de la vejiga como depósito de almacenamiento antes de la micción.
El capacitor refleja la habilidad del sistema urinario para almacenar volumen sin generar incrementos bruscos e inmediatos de presión, lo cual es fundamental para una función adecuada.

**Inercia del flujo urinario**.


La masa del líquido urinario en movimiento y la inercia hidráulica dentro de las estructuras tubulares se modelan mediante un inductor L representa la tendencia del flujo urinario a oponerse a cambios rápidos en su velocidad, la inercia del líquido en los túbulos renales y el comportamiento peristáltico de los uréteres que impulsa la orina en ondas, generando un flujo que no cambia instantáneamente al aumentar o disminuir la presión.
El inductor refleja cómo el sistema urinario responde con cierto retardo natural ante cambios súbitos en la presión o volumen generado por el riñón.

**Señal de entrada al sistema**.

La señal de entrada al circuito RLC se modela como un escalón unitario de presión, que representa un incremento rápido en la presión de filtración glomerular o en la producción momentánea de líquido urinario.
Este escalón simboliza el paso del sistema desde un estado basal hacia un estado donde se genera o conduce más volumen, permitiendo observar cómo el flujo urinario responde ante un estímulo súbito, los conductos se llenan de forma gradual según su capacitancia y la inercia del líquido suaviza los cambios bruscos del flujo.


Así, el modelo captura la dinámica esencial de la formación, tránsito y almacenamiento de la orina mediante un equivalente eléctrico de segundo orden RLC, permitiendo estudiar su comportamiento ante una entrada fisiológica básica.


Palabras clave: Circuito RLC; Controlador PID; Sistema urinario; Modelo matematico; Simulaciones numéricas.

## Lista de archivos incluidos en el repositorio

1. Cuaderno computacional de MATLAB \[.mlx].
2. Modelo de Simulink \[.slx].
3. Imagen con los parámetros del controlador.
4. Imágenes de las simulaciones \[.pdf y .png].
5. Evidencia del análisis matemático: función de transferencia, error en estado estacionario y estabilidad en lazo abierto.

## Referencias

\[1] P. A. Valle, Syllabus para Modelado de Sistemas Fisiológicos, Tecnológico Nacional de México / Instituto Tecnológico de Tijuana, Tijuana, B.C., México, 2025. Permalink: https://biomath.xyz/course/

\[2] M. C. Khoo, Physiological Control Systems Analysis Simulation, and Estimation, 2nd ed. Piscataway, New Jersey, USA: IEEE Press, 2018, Section 4, Page 93.
