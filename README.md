# Vehicle-routing-problem-With-Stochastic-Demands
Vehicle Routing Problem With Stochastic Demands (VRPSD)
Este repositorio contiene los archivos y el informe del proyecto realizado para la Práctica Investigativa I, donde se estudia y optimiza el problema de enrutamiento de vehículos con demandas estocásticas (VRPSD). El trabajo fue realizado por Juan José Castrillón y Juan Carlos Rivera, y se presenta en un formato detallado con la siguiente estructura:

Contenido del Repositorio
Informe PDF:

Presentacion_PI1.pdf: Documento detallado con la introducción, definición del problema, metodología, resultados, y conclusiones.
Código Fuente:

vrpsd_grasp.py: Implementación del algoritmo GRASP (Greedy Randomized Adaptive Search Procedure).
split_s.py: Procedimiento Split-S para el problema de TSP.
gurobi_partition.py: Particionamiento de conjuntos utilizando Gurobi.
capacity_simulation.py: Simulación de restricciones de capacidad del vehículo.
Descripción del Proyecto
Introducción
El objetivo del proyecto es optimizar las rutas de vehículos bajo incertidumbre en las demandas de los clientes. Para ello, se implementó un algoritmo comprensivo en Python que integra varias técnicas avanzadas: GRASP, Split-S y un modelo de particionamiento con Gurobi.

Definición del Problema
Se aborda un grafo no dirigido completo 
𝐺
=
(
𝑉
,
𝐸
)
G=(V,E), donde 
𝑉
=
{
0
,
1
,
.
.
.
,
𝑛
}
V={0,1,...,n} representa los nodos y 
𝐸
E las aristas. Cada cliente 
𝑖
∈
𝑉
∖
{
0
}
i∈V∖{0} tiene una demanda estocástica 
𝜉
𝑖
ξ 
i
​
 , y los vehículos tienen una capacidad 
𝑄
Q. El objetivo es minimizar el costo total esperado, incluyendo costos de viaje y recargo, considerando acciones de recarga como volver al depósito o recibir asistencia de otro vehículo.

Metodología
La metodología se compone de las siguientes fases:

Algoritmo Heurístico GRASP: Construcción de una solución inicial y mejora mediante búsqueda local.
Procedimiento Split-S para TSP: División de la solución TSP en sub-rutas basadas en el número de vehículos disponibles.
Particionamiento de Conjuntos con Gurobi: Optimización de la combinación de rutas para minimizar la distancia total recorrida.
Simulación de Restricciones de Capacidad: Simulación de la demanda utilizando una distribución normal y evaluación de dos enfoques: retorno al depósito y asistencia de vehículos cercanos.
Resultados
Instancia 1: Comparación gráfica de las rutas y las distancias totales recorridas bajo diferentes simulaciones.
Tabla Resumen: Resumen de las distancias totales recorridas en tres instancias, mostrando la eficiencia de los enfoques implementados.
Conclusiones y Futuras Investigaciones
La simulación paralela mejora significativamente las soluciones.
La asistencia de vehículos cercanos reduce la distancia total recorrida.
Contribuciones importantes en la optimización de rutas bajo demandas estocásticas.
Propuestas para futuras investigaciones, incluyendo el impacto de diferentes distribuciones de demanda y la aplicación de técnicas de aprendizaje automático.
Referencias Bibliográficas
Magdalene Marinaki, Andromachi Taxidou, and Yannis Marinakis. “A hybrid Dragonfly algorithm for the vehicle routing problem with stochastic demands”. In: Intelligent Systems with Applications 18 (2023), p. 200225. doi: https://doi.org/10.1016/j.iswa.2023.200225.
Jorge E. Mendoza and Juan G. Villegas. “A multi-space sampling heuristic for the vehicle routing problem with stochastic demands”. In: Optimization Letters 7 (2013). doi: https://link.springer.com/article/10.1007/s11590-012-0555-8.
Majid Salavati-Khoshghalb et al. “A hybrid recourse policy for the vehicle routing problem with stochastic demands”. In: EURO Journal on Transportation and Logistics 8.3 (2019), pp. 269–298. doi: https://doi.org/10.1007/s13676-018-0126-y.
