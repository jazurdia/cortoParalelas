# Proyecto: Simulación Fork-Join

Autor: Javier Alejandro Azurdia | 21242

## Instrucciones
Implementa una pequeña simulación en el lenguaje de tu preferencia (Python, C, C++, etc.) utilizando el patrón Fork-Join. La simulación debe calcular la suma de los elementos de una lista dividida en sublistas, donde cada sublista es procesada en paralelo, y luego los resultados parciales son combinados.

### Requisitos del proyecto:
- El código debe ejecutarse en paralelo utilizando al menos 4 hilos o procesadores.
- Documenta cómo lograste dividir las tareas y cómo manejas la combinación de los resultados.
- Entrega el código junto con un reporte en PDF que explique la arquitectura utilizada y los resultados obtenidos.

## Arquitectura Utilizada
La simulación utiliza el patrón Fork-Join para dividir una tarea en sub-tareas que se ejecutan en paralelo, mejorando así la eficiencia del cálculo. En este caso, se logró calcular la suma de una lista de 100000 elementos dividiéndola en 4 sublistas y procesándolas en paralelo con 4 hilos.

### División de Tareas
1. La lista original se divide en 4 sublistas, cada una de las cuales es procesada por un hilo separado.
2. Cada hilo calcula la suma parcial de su sublista y almacena el resultado en una lista compartida.

### Combinación de Resultados
1. Una vez que todos los hilos han completado su tarea, los resultados parciales se combinan sumándolos para obtener el resultado final.

## Resultados Obtenidos
La simulación se ejecutó varias veces y se encontró consistencia en los resultados, con una suma total de 4999950000 para una lista de 100000 elementos. Esto demuestra que la implementación fue exitosa.

## Conclusión
La simulación demuestra cómo se puede utilizar el patrón Fork-Join para dividir una tarea en sub-tareas que se ejecutan en paralelo, mejorando así la eficiencia del cálculo. En este caso, se logró calcular la suma de una lista de 100000 elementos dividiéndola en 4 sublistas y procesándolas en paralelo con 4 hilos. Se encontró que la suma tiene como resultado 4999950000. Se realizó varias veces la simulación, encontrando consistencia en ese resultado, por lo que se puede concluir que la implementación fue exitosa.