# simulacion-modelos-cambio-de-opinion
Proyecto para la materia "Simulación de eventos discretos", UBA

## Descripción 
En este proyecto se creó un modelo matemático para describir los cambios de opinión, en una sociedad de personas que interactúan entre si y con medios de comunicación masivos. Se hicieron distintos experimentos cómo por ejemplo, se vio qué pasa cuando a una sociedad de opiniones polarizadas está bajo influencia de medios polarizados, o qué pasa cuando hay un único medio de comunicación monopólico, etc. 

A este sistema se lo pensó como un sistema de eventos discretos y se lo formalizó y modularizó usando DEVS (Discrete Event System Specification). 
Para realizar la simulación se usó el simulador CD++ provisto por los docentes de la materia. 
Los modelos se escribieron en C++.

## Contenido
- [Instalación_simulador.ipynb](./Instalación_simulador.ipynb): este es un notebook de Jupyter-lab donde está el paso a paso y todos los códigos necesarios para poder instalar el simulador CD++ necesario para poder correr las simulaciones del proyecto.
- [notebook.ipynb](./notebook.ipynb): en este notebook se encuentra la descripción detallada del proyecto realizado y además todos los códigos necesarios para poder correr las simulaciones. También se presentan los resultados obtenidos y sus respectivas conclusiones. Observación: para que los resultados sean claros fue necesario hacer simulaciones de 2400 días. Hacer simulaciones que abarquen tanto tiempo, puede demorar un rato bastante largo. Por esto es que en el notebook ya están expuestos los resultados obtenidos con sus respectivos gráficos. Si aún así se quiere correr las simulaciones, se recomienda correrlas desde consola para demorar un poco menos de tiempo. 
- `\model`: aquí están todos los archivos .ma que se debieron generar para poder hacer las simulaciones de los distintos experimentos. Cada uno de estos archivos .ma contiene los modelos que componen al top-model y sus respectivos puertos de entrada y salida. Estos archivos fueron generados automáticamente con una función llamada generarMA presente en `notebook.ipynb`.
- `\out`: aquí están todos los archivos .out que se obtuvieron al hacer las simulaciones. Estos archivos contienen la información generada en las simulaciones, información la cual usamos para hacer los gráficos correspondientes de cada experimento.
- `\src`: acá están los códigos de C++ utilizados para programar los modelos implicados en este trabajo (Medio y Persona) con sus correspondientes headers.
- `\tests`: en esta carpeta están los archivos implicados en el testeo del proyecto. Aparecen archivos .ev donde se pusieron eventos discretos manualmente para testear a los modelos persona y medio, y también están los archivos .out obtenidos en las simulaciones. 
