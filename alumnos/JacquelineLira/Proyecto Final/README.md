## **Proyecto Final Análisis Aplicado**
- Jacqueline Lira Chávez - 167334

### Resúmen
En este proyecto se implementaron los algoritmos de optimización de Newton, Búsqueda Lineal, Búsqueda Lineal con Modificación a la Hessiana y BFGS en una clase de Python. Además de esto, se utilizó una base de datos que contiene información sobre la ubicación de los crímenes cometidos en la Ciudad de México para determinar cuál sería la mejor ubicación para unas cámaras que se van a instalar. Por cuestiones de tiempo, sólo se tomó en consideración una parte de la base de datos para hacer esta aproximación y asumimos que el número de cámaras a instalarse serían 8.

### Estructura
En la carpeta del proyecto final se encuentran tres archivos, el primero de ellos es la base de datos de los crímenes. El segundo archivo, llamado _Proyecto Final(clase)_ contiene la clase de Optimización, que incluye los métodos implementados, y contiene la optimización de las cámaras en la ciudad de México. Por último, el tercer archivo, _Proyecto Final_ incluye los métodos mencionados anteriormente pero estos no están en forma de clase. Sin embargo, este archivo contiene un poco más de información sobre los distintos métodos utilizados y es dónde se realizaron la mayoría de las pruebas para verificar la correctez de la implementación.

### Implementación
Para la implementación de los métodos de optimización se utilizó cómo base el método de búsqueda lineal con modificación a la hessiana que se realizó en la primera entrega para el proyecto para realizar los métodos de búsqueda lineal y de Newton. Para el método de BFGS, se siguió la implementación que se muestra en el libro de la materia.

Para la optimización de las cámaras se utilizó la fórmula de Haversine para medir la distancia entre dos puntos que están representados por su latitud y longitud. La función de costos se definió como la distancia entre cada cámara y cada crimen sumado a la inversa de la distancia entre todas las cámaras. Para terminar, para implementarse, se tuvieron que convertir las matrices de tamaño (n, 2) a matrices de (2*n, 1) para poder utilizar los métodos.

### Conclusiones
Este proyecto permitió que se pudiera ver la diferencia entre los métodos de optimización y su efectividad. En partícular podemos notar que el método de Newton y de Búsqueda Lineal causaron problemas al sólamente aceptar una hessiana positiva definida, algo que no fue problema para los otros dos. 
