# MCOC-Proyecto-2-Entrega-4-

## Edición de Windows

- Windows 10 pro

## Especificaciones del computador 

- Procesador: Intel(R) Core(TM) i5-4200U @ 1.60GHz 
- Memoria Instalada (RAM): 6,00 GB
- Tipo de sistema: Sistema Operativo de 64 bits, procesador x64

## Tiempos de procesamiento dependiendo del número de partículas

Para calcular los tiempos de funcionamiento se midió 3 veces el tiempo que demoraba en correr el código para cada cantidad de partículas y se sacó un promedio. Los resultados se presentan a continuación junto con los gráficos para cada situación:


## Resultados
Los gráficos previamente presentados representan el recorrido de cada una de las partículas. El eje "x" representa la distancia que recorre horizontalmente la párticula y el eje "y" la distancia vertical.

Cuando las curvas se intersectan, no significa que se produjo un choque entre las partículas, ya que los gráficos muestran la trayectoria a través del tiempo por lo que cuando dos curvas (o más) se intersectan, significa que las partículas pasaron por ese punto pero en distintos instantes de tiempo.

Para poder notar si es que se produjo un choque entre partículas, se debe observar si hubo un cambio abrupto en la curva de alguna de las partículas, ya que esto significa que algo interrumpió su trayectoria, y según lo implementado en el código sólo podría ser otra partícula. 

Los resultados obtenidos no son semejantes a la realidad, ya que para la implementación sólo se consideraron las siguientes fuerzas:
- Fuerza de arrastre (drag).
- Fuerza de sustentación (lift).
- Fuerza de gravedad (peso).

En la realidad estas no son las únicas fuerzas que afectan el movimiento de las partículas en un fluido (también influyen la fuerza Basset, Magnus y la fuerza de masa virtual).
Otros factores que afectan al realismo de los resultados son:
- Asumir que todas las partículas son esféricas y de iguaol radio.
- Para el rebote contra el suelo se utilizó el k_penal (valor que fue inventado).
- Sólo se consideraron dos dimensiones para modelar el movimiento de las partículas.

Todos estos supuestos se hicieron para poder simplificar la implementación del código, algo que es muy común en el ámbito de la ingeniería ya que a veces simplificando un poco el problema se obtienen resultados que no estan tan alejados de la realidad.
