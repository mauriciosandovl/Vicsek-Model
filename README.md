# Modelo de Vicsek

## Descripción

El modelo de Vicsek permite simular la materia activa desde una perspectiva de modelación basada en agentes dando lugar
a un modelo muy sencillo y flexible que puede adaptarse muy bien a describir una gran variedad de
fenómenos de la naturaleza como el comportamiento colectivo de animales (e.g. parvadas de aves o colonias de hormigas).
El modelo se basa únicamente en definir la interacción de los
agentes en un área de alineamiento y no define áreas de atracción y repulsión. Para ver una descripción completa consultar
el archivo protocolo.pdf.

## Parámetros

Todos los archivos están escritos en el programa NetLogo. Cada uno de los modelos contiene un botón de `setup` y `go`, y los siguientes parámetros en forma de deslizadores: `density` entre 0 y 100, `noise` entre 0 y 5, `velocity` entre 0 y 1 y `radius` entre 0 y 5.

Todas las pruebas fueron realizadas en una cuadrícula de 100 por 100 con condiciones de frontera periodicas.

## Códigos
1. En 1_vicsek_simple.nlogo se hace una implementación del modelo tal y como es expuesto en la referencia principal.

2. En 2_vicsek_extrinsic.nlogo se añade un chooser con la variable `noise-type` que permite elegir entre los tipos de ruido: "intrinsic" y "extrinsic". Esta variable se mantiene en el resto de archivos siguientes.

3. En 3_vicsek_variable_velocity.nlogo se modifica la variable `velocity` por `velocity-threshold` que toma valores en el mismo rango. Esta variable no se mantiene en el resto de archivos.

4. En 4_vicsek_vision.nlogo se añade la variable `vision` a manera de slider que toma valores entre 0 y 360.

5. En 5_vicsek_obstacles.nlogo se reproducen las mismas variables que en 4_vicsek_vision.nlogo y se añade un chooser con la variable `obstacle-type` que permite elegir entre tres distintos tipos de obstáculos: "circulos", "corona circular" y "muros".
