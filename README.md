# Análisis de ventas de videojuegos

Proyecto de análisis exploratorio de datos sobre videojuegos para la tienda online Ice. El objetivo es identificar patrones de ventas, plataformas, géneros, puntuaciones y mercados regionales que ayuden a detectar juegos con potencial comercial.

El análisis se plantea como si fuera diciembre de 2016, con el propósito de planificar una campaña para 2017. Por eso, las comparaciones y conclusiones se enfocan principalmente en los datos disponibles hasta 2016.

## Contenido

- `notebook_andres_samboni_final_modulo_1.ipynb`: notebook con la limpieza, exploración, visualizaciones y pruebas de hipótesis.
- `datasets/games.csv`: archivo de datos esperado por el notebook. Debe estar disponible localmente; no se incluye aquí necesariamente.

## Datos

El dataset contiene información histórica de videojuegos, entre ella plataforma, año de lanzamiento, género, reseñas de usuarios y crítica, clasificación ESRB y ventas por región. Las columnas de ventas regionales (`na_sales`, `eu_sales`, `jp_sales` y `other_sales`) están expresadas en millones de unidades vendidas; `total_sales` se calcula sumándolas.

## Análisis realizado

- Limpieza de nombres de columnas, tipos de datos y valores no numéricos como `tbd`.
- Exploración de lanzamientos y ventas por año, década y plataforma.
- Comparación de plataformas, géneros, puntuaciones y ventas regionales.
- Análisis de la relación entre puntuaciones y ventas.
- Pruebas de hipótesis sobre puntuaciones de usuarios entre plataformas y géneros.

## Requisitos

Python 3 y Jupyter Notebook o JupyterLab, además de estas bibliotecas:

```bash
pip install numpy pandas matplotlib scipy seaborn jupyter
```

## Cómo ejecutar

1. Coloca `games.csv` en la carpeta `datasets/`, junto al notebook.
2. Inicia Jupyter desde la carpeta del proyecto:

   ```bash
   jupyter notebook
   ```

3. Abre `notebook_andres_samboni_final_modulo_1.ipynb` y ejecuta las celdas en orden.

El notebook carga los datos con la ruta relativa `./datasets/games.csv`.
