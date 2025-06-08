# 📊 TelecomX Churn Analysis: Descubriendo Patrones de Evasión de Clientes

## Introducción

Este proyecto tiene como propósito principal realizar un análisis exploratorio de datos (EDA) exhaustivo sobre los datos de clientes de una empresa de telecomunicaciones ficticia, TelecomX, con el fin de **comprender y mitigar la evasión de clientes (churn)**. La alta tasa de churn representa un desafío significativo para las empresas de servicios, y este análisis busca identificar los factores clave que influyen en la decisión de un cliente de cancelar su servicio. A través de la limpieza, transformación y visualización de datos, proporcionamos insights accionables para el desarrollo de estrategias de retención.

## Estructura del Proyecto y Organización de los Archivos

El repositorio está organizado de la siguiente manera:

-   `TelecomX_LATAM.ipynb`: El cuaderno principal de Jupyter/Colab que contiene todo el código del proyecto, incluyendo:
    -   **Extracción de Datos:** Carga del dataset original en formato JSON.
    -   **Transformación y Limpieza de Datos:** Normalización de datos anidados, manejo de valores faltantes, conversión de tipos de datos, creación de nuevas características y estandarización de columnas.
    -   **Análisis Exploratorio de Datos (EDA):** Visualizaciones y análisis estadísticos para entender la distribución de las variables y su relación con la evasión.
    -   **Análisis de Correlación:** Exploración de relaciones entre variables numéricas y la variable objetivo 'Evasión'.
    -   **Informe Final:** Un resumen estructurado de todo el trabajo realizado, los hallazgos y las recomendaciones.
-   `TelecomX_Data.json`: El dataset original de los clientes de TelecomX en formato JSON.
-   `TelecomX_Processed_Data.json`: (Opcional, si lo exportaste) El dataset después de todas las fases de extracción, limpieza y transformación, listo para futuros análisis o modelado.
-   `README.md`: Este archivo, que describe el proyecto.
-   `images/` (Opcional): Una carpeta que podrías crear para almacenar capturas de pantalla de tus gráficos para incrustarlas en este README.

## Ejemplos de Gráficos e Insights Obtenidos

Durante el análisis exploratorio, se descubrieron patrones significativos relacionados con la evasión. A continuación, se presentan algunos ejemplos representativos de las visualizaciones y los insights derivados:

### 1. Distribución General de la Evasión

Se observó que un porcentaje considerable de clientes tiende a la evasión, lo que subraya la importancia de este análisis.

![Proporción de Clientes con y sin Evasión](https://via.placeholder.com/600x400?text=IMAGEN+DEL+GRÁFICO+DE+TORTA+DE+EVASIÓN+AQUÍ)
*Este gráfico de torta muestra la proporción de clientes que evaden (Sí) y los que no (No).*

### 2. Evasión por Tipo de Contrato

Los clientes con contratos **"Mes a Mes"** muestran una propensión mucho mayor a la evasión en comparación con aquellos con contratos a largo plazo (uno o dos años). Esto sugiere que la falta de compromiso a largo plazo es un factor de riesgo clave.

![Evasión por Tipo de Contrato](https://via.placeholder.com/800x500?text=IMAGEN+DEL+GRÁFICO+DE+BARRAS+DE+TIPO+DE+CONTRATO+VS+EVASIÓN+AQUÍ)
*Se observa claramente cómo los contratos mensuales tienen la mayor tasa de churn.*

### 3. Evasión por Antigüedad del Cliente (Tenure)

Los clientes con **baja antigüedad** (pocos meses) tienen una tasa de evasión notablemente alta. La probabilidad de evasión disminuye significativamente a medida que la antigüedad del cliente aumenta.

![Distribución de Antigüedad por Evasión](https://via.placeholder.com/800x500?text=IMAGEN+DEL+HISTOGRAMA+O+BOXPLOT+DE+ANTIGUEDAD+VS+EVASIÓN+AQUÍ)
*Este gráfico ilustra que la mayoría de los clientes que evaden lo hacen en sus primeros meses.*

### 4. Evasión por Cargos Mensuales

Existe una tendencia a que los clientes con **cargos mensuales más altos** sean más propensos a la evasión. Esto podría indicar una insatisfacción con la relación calidad-precio o la presencia de ofertas más competitivas en el mercado.

![Distribución de Cargos Mensuales por Evasión](https://via.placeholder.com/800x500?text=IMAGEN+DEL+HISTOGRAMA+O+BOXPLOT+DE+CARGOS+MENSUALES+VS+EVASIÓN+AQUÍ)
*Los clientes que evaden tienden a tener facturas mensuales más elevadas.*

## Instrucciones para Ejecutar el Notebook

Para ejecutar este análisis en tu propio entorno:

1.  **Clona este Repositorio:**
    ```bash
    git clone [https://github.com/TuUsuario/NombreDeTuRepositorio.git](https://github.com/TuUsuario/NombreDeTuRepositorio.git)
    cd NombreDeTuRepositorio
    ```
    (Reemplaza `TuUsuario` y `NombreDeTuRepositorio` por los tuyos.)

2.  **Abre el Notebook en Google Colab:**
    * Ve a [Google Colab](https://colab.research.google.com/).
    * Haz clic en `Archivo > Abrir cuaderno`.
    * En la pestaña `GitHub`, busca tu repositorio y selecciona `TelecomX_LATAM.ipynb`.

3.  **Sube el Dataset:**
    * Una vez que el notebook esté abierto en Colab, deberás subir el archivo `TelecomX_Data.json`.
    * Haz clic en el icono de la carpeta en el panel izquierdo (`Files`).
    * Haz clic en el icono de "Subir" (un documento con una flecha hacia arriba) y selecciona `TelecomX_Data.json` desde tu computadora. Asegúrate de que quede en la carpeta `/content/`.

4.  **Ejecuta las Celdas:**
    * Ejecuta todas las celdas del notebook en orden, desde la primera hasta la última. Puedes usar `Runtime > Run all` o ejecutar cada celda individualmente (`Shift + Enter`).

¡Con esto, podrás reproducir el análisis completo y generar todas las visualizaciones en tu propio entorno!

## Tecnologías Utilizadas

* **Python 3.x**
* **Pandas:** Para manipulación y análisis de datos.
* **NumPy:** Para operaciones numéricas.
* **Matplotlib:** Para la creación de gráficos estáticos.
* **Seaborn:** Para visualizaciones estadísticas atractivas.

---
