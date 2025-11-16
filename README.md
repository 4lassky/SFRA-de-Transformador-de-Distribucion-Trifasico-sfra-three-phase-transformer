# SFRA-de-Transformador-de-Distribucion-Trifasico-sfra-three-phase-transformer
Este script de MATLAB está diseñado para el Análisis de Respuesta en Frecuencia de Barrido (SFRA) de un transformador de distribución trifásico. Compara una medición de referencia con múltiples mediciones de falla (archivos `.s2p`).

Proyecto académico realizado por **Galindo Barbosa Israel Aldahir** y **Herrera Godoy Hazael** para **ESIME ZACATENCO - IPN**.

## Características Principales
* **Carga de Datos:** Importa archivos `.s2p` de referencia y de fallas.
* **Modos de Prueba:** El código está preconfigurado con rangos de frecuencia para análisis de **Circuito Abierto** y **Circuito Corto**. El usuario debe comentar/descomentar la sección relevante.
* **Visualización 2D:** Genera gráficas SFRA (Referencia vs. Fallas) con las 4 zonas de frecuencia de la norma **IEEE C57.149-2012**.
* **Detección de Resonancias:** Identifica y extrae 3 resonancias principales basándose en los rangos de frecuencia definidos para la prueba (abierto o corto).
* **Análisis de Tendencia:** Grafica la dispersión de magnitud, frecuencia y ángulo de cada resonancia en función de la ubicación de la falla (disco).
* **Análisis Estadístico:** Calcula el coeficiente de correlación de **Pearson** para cada resonancia.
* **Visualización 3D:** Crea una superficie 3D que muestra la evolución de la traza SFRA.
* **Exportación:** Guarda las figuras en formato `.png` y crea un `.gif` animado de la gráfica 3D.

## Uso
1.  **Importante:** Antes de ejecutar, abra el script y navegue a la sección `%% === ANÁLISIS SFRA y detección de resonancias ===`.
2.  Asegúrese de que los rangos de frecuencia (`rangosRef` y `rangosFalla`) correctos estén **descomentados** (ya sea para "circuito abierto" o "circuito corto") y los otros estén comentados.
3.  Ejecute el script.
4.  Seleccione el archivo `.s2p` de **Referencia**.
5.  Seleccione los archivos `.s2p` de **Falla**.
6.  Asegúrese de que la variable `discosSeleccionados` esté correctamente definida.
7.  El script generará los resultados y preguntará si desea guardar las figuras.
