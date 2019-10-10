# MCOC-Proyecto-2-Entrega-4-

## Edición de Windows

- Windows 10 pro

## Especificaciones del computador 

- Procesador: Intel(R) Core(TM) i5-4200U @ 1.60GHz 
- Memoria Instalada (RAM): 6,00 GB
- Tipo de sistema: Sistema Operativo de 64 bits, procesador x64

## Tiempos de procesamiento dependiendo del número de partículas

Para calcular los tiempos de funcionamiento se midió 3 veces el tiempo que demoraba en correr el código para cada cantidad de partículas y se sacó un promedio. Los resultados se presentan a continuación junto con los gráficos para cada situación:

- ### 1 partícula: 1.3 segundos
#### Gráfico para 1 partícula
![Gráfico_1_partícula](https://user-images.githubusercontent.com/53578787/66603805-4f963d00-eb83-11e9-9b9f-c8b5acc223f6.png)

- ### 2 partículas: 1.5 segundos
#### Gráfico para 2 partículas
![Gráfico_2_partículas](https://user-images.githubusercontent.com/53578787/66604298-448fdc80-eb84-11e9-86b6-c6a4dc0908d6.png)

- ### 3 partículas: 2.1 segundos
#### Gráfico para 3 partículas
![Gráfico_3_partículas](https://user-images.githubusercontent.com/53578787/66605484-96d1fd00-eb86-11e9-9b26-403c63fb17b0.png)

- ### 4 partículas: 3.1 segundos
#### Gráfico para 4 partículas
![Gráfico_4_partículas](https://user-images.githubusercontent.com/53578787/66605760-0e079100-eb87-11e9-94fa-a999c8c13b87.png)

- ### 5 partículas: 5.9 segundos
#### Gráfico para 5 partículas
![Gráfico_5_partículas](https://user-images.githubusercontent.com/53578787/66605894-57f07700-eb87-11e9-952b-53b4fd9cb577.png)

- ### 8 partículas: 18.6 segundos
#### Gráfico para 8 partículas
![Gráfico_8_partículas](https://user-images.githubusercontent.com/53578787/66605999-88d0ac00-eb87-11e9-8ec0-1c3f4c3ce75b.png)

- ### 10 partículas: 85.9 segundos
#### Gráfico para 10 partículas
![Gráfico_10_partículas](https://user-images.githubusercontent.com/53578787/66606170-ee249d00-eb87-11e9-964c-035a73ec3b4f.png)

## Resultados
Los gráficos previamente presentados representan el recorrido de cada una de las partículas. El eje "x" representa la distancia que recorre horizontalmente la párticula y el eje "y" la distancia vertical.

Cuando las curvas se intersectan, no significa que se produjo un choque entre las partículas, ya que los gráficos muestran la trayectoria a través del tiempo por lo que cuando dos curvas (o más) se intersectan, significa que las partículas pasaron por ese punto pero en distintos instantes de tiempo.

Para poder notar si es que se produjo un choque entre partículas, se debe observar si hubo un cambio abrupto en la curva de alguna de las partículas, ya que esto significa que algo interrumpió su trayectoria, y según lo implementado en el código sólo podría ser otra partícula. 

Los resultados obtenidos no son semejantes a la realidad, ya que para la implementación sólo se consideraron las siguientes fuerzas:

