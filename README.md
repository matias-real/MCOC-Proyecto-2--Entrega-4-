# MCOC-Proyecto-2-Entrega-4-

## Edición de Windows

- Windows 10 pro

## Especificaciones del computador 

- Procesador: Intel(R) Core(TM) i5-4200U @ 1.60GHz 
- Memoria Instalada (RAM): 6,00 GB
- Tipo de sistema: Sistema Operativo de 64 bits, procesador x64

## Tiempos de funcionamiento del código (en el computador del alumno)

El funcionamiento del código fue probado para la simulación de:
- 2 partículas.
- 5 partículas.
- 10 partículas.
- 20 partículas.

Estas fueron las mismas cantidades que probó el profesor y esto se hizo con la finalidad de comparar el funcionamiento del código de los alumnos, en sus respectivos computadores, con el del profesor, en su propio computador. A continuación, se presentan los gráficos y tiempos de funcionamiento para cada uno de los casos:

### 2 partículas ------> 7,98 segundos.
#### Gráfico de recorrido para 2 partículas.
![Gráfico_2_Partículas](https://user-images.githubusercontent.com/53578787/66691266-7af45700-ec6b-11e9-9b94-f1d241e68aff.png)

### 5 partículas ------> 63, 59 segundos.
#### Gráfico de recorrido para 5 partículas.
![Gráfico_5_Partículas](https://user-images.githubusercontent.com/53578787/66691264-70d25880-ec6b-11e9-8c88-1722f808cd7d.png)

### 10 partículas ------> 681.0 segundos.
#### Gráfico de recorrido para 10 partículas.
![Gráfico_10_Partículas](https://user-images.githubusercontent.com/53578787/66691260-6b750e00-ec6b-11e9-940a-548f9b480400.png)

Cuando se realizó la simulación para el caso en que eran 20 partículas, se dejó corriendo el código por mas de una hora y media y no entregó resultados, por lo que no se presentan los resultados para esa simulación.

#### Gráfico de tiempos de funcionamiento (alumno)
![Gráfico tiempos de funcionamiento](https://user-images.githubusercontent.com/53578787/66692218-a3cc1a80-ec72-11e9-8011-f57d48d5dd70.PNG)


## Tiempos de funcionamiento del código del profesor (en su propio computador)

### 2 partículas ------> 44.1 segundos
#### Gráfico de recorrido para 2 partículas.
![particle_trajectories](https://user-images.githubusercontent.com/53578787/66691614-0a026e80-ec6e-11e9-9587-4582ceb9f1fa.png)

### 5 partículas ------> 115.1 segundos
#### Gráfico de recorrido para 5 partículas.
![particle_trajectories](https://user-images.githubusercontent.com/53578787/66691573-e2aba180-ec6d-11e9-8b9b-b07b578b02eb.png)

### 10 partículas ------> 251.5 segundos
#### Gráfico de recorrido para 10 partículas.
![particle_trajectories](https://user-images.githubusercontent.com/53578787/66691552-b728b700-ec6d-11e9-8c62-a6dfd32dcfd7.png)


### 20 partículas ------> 477.0 segundos
#### Gráfico de recorrido para 20 partículas.
![particle_trajectories](https://user-images.githubusercontent.com/53578787/66691641-2ef6e180-ec6e-11e9-979d-e9c80a51ac5b.png)

#### Gráfico de tiempos de funcionamiento (profesor)
![Gráfico de tiempos de funcionamiento (profesor)](https://user-images.githubusercontent.com/53578787/66692306-80559f80-ec73-11e9-9fbb-89e493fbd650.PNG)

## Interpretación de los Resultados
Los gráficos previamente presentados representan el recorrido de cada una de las partículas. El eje "x" representa la distancia que recorre horizontalmente la párticula y el eje "y" la distancia vertical. También se presenta el gráfico de la variación del tiempo de funcionamiento del código de acuerdo a la cantidad de partículas simuladas.

Cuando las curvas se intersectan, no significa que se produjo un choque entre las partículas, ya que los gráficos muestran la trayectoria a través del tiempo por lo que cuando dos curvas (o más) se intersectan, significa que las partículas pasaron por ese punto pero en distintos instantes de tiempo.

Para poder notar si es que se produjo un choque entre partículas, se debe observar si hubo un cambio abrupto en la curva de alguna de ellas, ya que esto significa que algo interrumpió su trayectoria, y según lo implementado en el código sólo podría ser otra partícula. 

Se puede apreciar que para las simulaciones con 2 y 5 partículas los resultados del alumno fueron obtenidos con mayor rapidez. No así el caso para las simulaciones con 10 partículas ya que se obtuvieron considerablemente más rapido los resultados del profesor. Con esto se podría decir que para grandes números de partículas el código del alumno no funciona de la mejor manera, de hecho para 20 partículas no se obtuvieron resultados en el caso del alumno.

Los resultados obtenidos no son semejantes a la realidad, ya que para la implementación sólo se consideraron las siguientes fuerzas:
- Fuerza de arrastre (drag).
- Fuerza de sustentación (lift).
- Fuerza de gravedad (peso).

En la realidad estas no son las únicas fuerzas que afectan el movimiento de las partículas en un fluido (también influyen la fuerza Basset, Magnus y la fuerza de masa virtual).
Otros factores que afectan al realismo de los resultados son:
- Asumir que todas las partículas son esféricas y de igual radio.
- Utilizar el k_penal (valor que fue inventado) para simular rebote contra el suelo.
- Asumir que el suelo es una cama de partículas equiespaciadas.
- Considerar sólo dos dimensiones para modelar el movimiento de las partículas.

Todos estos supuestos se hicieron para poder simplificar la implementación del código, algo que es muy común en el ámbito de la ingeniería ya que a veces simplificando el problema se obtienen resultados que no estan tan alejados de la realidad.
