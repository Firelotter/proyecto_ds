# EV09 - Clasificacion de Variables y Seleccion de Graficas

**Evidencia:** GA1-240201064-04-AA1-EV09  
**Programa:** ADSO  
**Fecha:** 2026-04-05

## 1. Tabla de clasificacion de variables (dataset del proyecto)

| Variable | Tipo | Subtipo | Justificacion |
|---|---|---|---|
| Rank | Cualitativa | Ordinal | Representa orden de posicion (ranking), no magnitud de distancia. |
| Name | Cualitativa | Nominal | Etiqueta de texto sin orden natural. |
| Platform | Cualitativa | Nominal | Categoria de consola/plataforma sin jerarquia. |
| Year | Cuantitativa | Discreta | Valores enteros de tiempo (anos). |
| Genre | Cualitativa | Nominal | Categoria de genero sin orden. |
| Publisher | Cualitativa | Nominal | Nombre de empresa, categoria sin orden. |
| NA_Sales | Cuantitativa | Continua | Medida numerica con decimales en millones. |
| EU_Sales | Cuantitativa | Continua | Medida numerica con decimales en millones. |
| JP_Sales | Cuantitativa | Continua | Medida numerica con decimales en millones. |
| Other_Sales | Cuantitativa | Continua | Medida numerica con decimales en millones. |
| Global_Sales | Cuantitativa | Continua | Variable de medicion agregada en escala continua. |

## 2. Tabla de seleccion de graficas

| Variable | Tipo/Subtipo | Grafica recomendada | Por que usarla |
|---|---|---|---|
| Rank | Cualitativa ordinal | Histograma por rangos de ranking | Permite ver concentracion de juegos por tramos de posicion. |
| Name | Cualitativa nominal | Barras (Top N por frecuencia) | Solo en resumenes; nombres individuales son demasiados para grafica completa. |
| Platform | Cualitativa nominal | Barras | Comparacion directa de frecuencia o ventas por plataforma. |
| Year | Cuantitativa discreta | Linea (conteo/ventas por ano) | Muestra tendencia temporal. |
| Genre | Cualitativa nominal | Barras | Facilita comparar categorias de genero. |
| Publisher | Cualitativa nominal | Barras (Top N) | Hay muchas categorias, conviene resumir por principales. |
| NA_Sales | Cuantitativa continua | Histograma y boxplot | Muestran distribucion, dispersion y atipicos. |
| EU_Sales | Cuantitativa continua | Histograma y boxplot | Muestran distribucion, dispersion y atipicos. |
| JP_Sales | Cuantitativa continua | Histograma y boxplot | Muestran distribucion, dispersion y atipicos. |
| Other_Sales | Cuantitativa continua | Histograma y boxplot | Muestran distribucion, dispersion y atipicos. |
| Global_Sales | Cuantitativa continua | Histograma y boxplot | Permite evaluar sesgo, dispersion y extremos. |
| NA_Sales vs EU_Sales | Cuantitativa continua vs continua | Dispersion | Permite evaluar relacion entre ventas de dos regiones. |

## 3. Reflexion final

1. **Que variables fueron mas dificiles de clasificar y por que?**  
`Rank` fue la mas discutible porque usa numeros, pero describe posicion relativa; por eso se clasifica mejor como ordinal.

2. **Que riesgos puede generar escoger una grafica incorrecta?**  
Se pueden ocultar patrones o inducir conclusiones erradas. Un ejemplo comun es usar grafica de pastel con demasiadas categorias, lo que dificulta comparar proporciones.

3. **Como impacta la clasificacion de variables en la analitica de datos?**  
Impacta directamente la validez del analisis: una clasificacion correcta permite elegir tecnicas y visualizaciones coherentes, mejora la interpretacion y reduce errores de decision.

## Referencias

- pandas development team. (n.d.). *pandas documentation*. https://pandas.pydata.org/docs/
- Matplotlib Development Team. (n.d.). *Matplotlib documentation*. https://matplotlib.org/
- McKinney, W. (2022). *Python for Data Analysis* (3rd ed.). O'Reilly Media.
