# SEPPViz
Se presenta SEPPViz, una herramienta desarrollada con el fin de agilizar y democratizar el uso de algoritmos basados en los procesos de punto auto-excitado. 

En esta documentación se justifica la necesidad de una herramienta de este tipo, describiendo los requisitos que debe cumplir y comparando dicha herramienta con otras soluciones similares actualmente disponibles, posteriormente, se explica el proceso de desarrollo de esta herramienta y, finalmente, se proporcionan diversas imágenes que ilustran su uso adecuado.


## Necesidad y requisitos
No existen gran cantidad de herramientas de visualización disponibles para usuarios no introducidos en el mundo de la programación. La mayoría de visualizaciones se desarrollan con librerías de Python, MATLAB y R y no son reproducibles por los miembros de seguridad del estado que no tengan conocimiento de estos lenguajes de programación.

Se quiso aportar como novedad una herramienta la cual bautizamos como SEPPViz, nombre procedente de ``SEPP Visualization''.

SEPPViz nace con el fin de que incluso usuarios no familiarizados con el algoritmo SEPP sean capaces de hacer predicciones de puntos calientes en los que los futuros eventos espacio-temporales pueden ocurrir con mayor probabilidad, independientemente del suceso que se trate de predecir o el lugar del mismo.

La principal premisa de esta herramienta es proporcionar a los profesionales de la seguridad una solución accesible y fácil de utilizar, sin requerir una amplia capacitación en informática. Asimismo, se busca ofrecer una experiencia de visualización que permita tomar decisiones fundamentadas a partir de los datos analizados y desarrollar actividades de monitorización diaria así como estrategias de mitigación a largo plazo.

Es por ello que los principales requisitos para esta herramienta son:
 - Uso intuitivo y sencillo incluso para usuarios sin experiencia en programación.
 - Flexibilidad para cambiar la localización de manera sencilla.
 - Capacidad de cambiar los hiperparámetros y recalcular los mapas de calor interactivamente.
 - Capacidad para cambiar los \emph{datasets} utilizados.

## Desarrollo
El desarrollo de SEPPViz se ha efectuado usando el lenguaje de programación Python, la elección de este lenguaje se ha basado en su gran versatilidad ya que permite simplificar el proceso de desarrollo gracias a la multitud de librerías y herramientas disponibles y ya que es fácilmente ejecutable en cualquier tipo de sistema operativo, estando masivamente generalizado su uso actualmente.

Las principales librerías utilizadas en el desarrollo de SEPPViz han sido PyQt5 para la implementación de la interfaz gráfica y folium para la incorporación tanto del mapa interactivo como de las capas que se superponen mostrando la información de los mapas de calor.

Trabajando bajo la suposición de que se trata de un software utilizado principalmente por los cuerpos de seguridad del estado, se ha decidido distribuirlo bajo licencias de software libre, para ser específicos bajo la licencia GNU GENERAL PUBLIC LICENSE v3 por lo todo el código esta disponible libremente a través de este repositorio.

## Uso
La herramienta implementa una barra lateral que permite la selección de la fuente de datos y la introducción de valores para las variables que influyen en el cálculo de las predicciones. Esta funcionalidad permite a los usuarios ajustar los parámetros y obtener visualizaciones personalizadas según sus requerimientos. La barra lateral se concibe como un panel de control intuitivo, que posibilita la interacción de manera sencilla y eficiente.

La parte principal de la interfaz está dedicada a la visualización del archivo HTML generado, el cual emplea un mapa de calor. Este recurso gráfico proporciona una representación visual de los datos analizados, facilitando la identificación de patrones y tendencias relevantes. La escala de colores y la intensidad del mapa de calor se ajustan en función de los valores de los datos, permitiendo una comprensión y evaluación visual rápida de la información presentada.