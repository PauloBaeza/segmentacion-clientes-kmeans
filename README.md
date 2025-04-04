
# Segmentación de Clientes con K-Means de una cadena de supermercados

Este proyecto consiste en la aplicación de técnicas de **aprendizaje no supervisado** para segmentar clientes de una cadena de supermercados utilizando el algoritmo **K-Means**. El objetivo es identificar grupos de clientes con comportamientos similares para facilitar la personalización de estrategias de marketing y promociones.

---

# Estructura del Proyecto

- `dataclientes.xlsx`: Base principal con información transaccional de los clientes.
- `georef.csv`: Coordenadas geográficas de las ciudades, usadas para mapas.
- `segmentacion_clientes.ipynb`: Notebook principal con todo el análisis.
- `README.md`: Este archivo.

---

## 🔍 Descripción del Proyecto

Se trabajó con una base de datos de clientes, con variables como:

- `Customer_ID`: Identificador único del cliente.
- `Date`: Fecha de transacción.
- `Price`: Valor de la compra.
- `City`, `Store_Type`, `Season`, `Product`, etc.

Además, se creó una nueva variable llamada **`ticket_promedio`**, obtenida al dividir el gasto total entre la cantidad de transacciones por cliente.

El análisis incluyó:

1. **Análisis exploratorio de datos (EDA)**
2. **Creación de variables relevantes para el modelo**
3. **Normalización y escalamiento de datos**
4. **Aplicación del algoritmo K-Means**
5. **Validación con métricas (Silhouette Score y Calinski-Harabasz Index)**
6. **Visualización de los segmentos y análisis de perfiles**

---

# Resultados

Se definieron **5 segmentos de clientes**, con los siguientes perfiles:

| Segmento | Nombre                          | Descripción principal |
|----------|----------------------------------|------------------------|
| 0        | Cliente Leal y Frecuente        | Alta frecuencia de compra, ticket moderado |
| 1        | Cliente Premium Ocasional       | Pocas compras, ticket alto |
| 2        | Cliente VIP o Premium           | Alto gasto total y ticket elevado |
| 3        | Cliente Promedio                | Comportamiento intermedio |
| 4        | Cliente Dormido o de Bajo Impacto | Bajo en todas las variables |

---

# Visualización

Se incluyen gráficos:
- Barras por producto más vendido por estación
- Gráfico 3D con los clústeres
- Mapa georreferenciado por ciudad
- Tabla con productos más y menos comprados por ciudad

---

# Requisitos

Este proyecto requiere Python 3.10+ y las siguientes librerías:

```bash
pandas
numpy
matplotlib
seaborn
plotly
scikit-learn
```

Puedes instalar las dependencias con:

```bash
pip install -r requirements.txt
```

O manualmente:

```bash
pip install pandas numpy matplotlib seaborn plotly scikit-learn
```

---

# Conclusión

La segmentación realizada con K-Means permite identificar perfiles de clientes con comportamientos diferenciados. Gracias a las métricas de validación, se comprobó que los grupos obtenidos tienen una estructura razonable. Esta segmentación puede ser utilizada para diseñar promociones personalizadas, mejorar la retención y aumentar el valor de vida del cliente (CLV).

---

# Contacto

Para dudas o sugerencias: paulobaeza2@gmail.com

# Vista rápida

Si no tienes Jupyter, puedes ver una versión estática del notebook aquí:

👉 [Ver archivo HTML](segmentacion_clientes.html)
