#### Dog Breeds Data Analysis
### Descripción del proyecto

Este proyecto consiste en un análisis exploratorio de datos sobre razas de perros, utilizando información obtenida desde The Dog API.
El objetivo es identificar patrones relacionados con la esperanza de vida, el peso y el temperamento de las distintas razas, y comunicar los hallazgos mediante visualizaciones claras.

El proyecto fue desarrollado como parte de un portafolio de Data Analysis, con foco en buenas prácticas de obtención, limpieza, análisis y comunicación de datos.

### Objetivos

Responder las siguientes preguntas:

¿Cuál es la esperanza de vida más frecuente entre las razas de perros?

¿Cuál es el temperamento más común?

¿Existe alguna relación entre el tamaño/peso de una raza y su esperanza de vida?

### Fuente de datos

Los datos fueron obtenidos desde The Dog API, utilizando el endpoint:

/v1/breeds


La API requiere autenticación mediante API Key, la cual fue incluida en la solicitud a través de headers HTTP (x-api-key).

### Nota de seguridad:
La API Key no se incluye en este repositorio. Para ejecutar el proyecto localmente, es necesario definir la variable de entorno DOG_API_KEY.

### Tecnologías utilizadas

Python

Jupyter Notebook

Pandas

Requests

Matplotlib

Seaborn

### Metodología

El análisis siguió las siguientes etapas:

Obtención de datos desde una API pública autenticada.

Inspección inicial del dataset (shape, head, info, valores nulos).

Limpieza y transformación de datos, incluyendo:

Conversión de rangos de texto a valores numéricos promedio.

Creación de variables derivadas (peso promedio, esperanza de vida promedio).

Clasificación de razas por categoría de tamaño.

Análisis exploratorio de datos (EDA).

Visualización de resultados mediante gráficos exportados para documentación.

Interpretación y conclusiones.

El dataset final contiene información de 169 razas de perros.

### Visualizaciones principales
Distribución del peso promedio

Relación entre peso promedio y esperanza de vida

Esperanza de vida por categoría de tamaño

### Hallazgos principales

La mayoría de las razas de perros se concentra en rangos de peso bajo, especialmente por debajo de los 30 kg.

Se observa una relación inversa entre el peso promedio y la esperanza de vida: las razas más pequeñas tienden a vivir más años.

Las razas grandes presentan una menor esperanza de vida media y una mayor variabilidad en comparación con razas pequeñas y medianas.

El temperamento más frecuente entre las razas analizadas está asociado a características como sociabilidad y docilidad.

### Estructura del proyecto
dog-breeds-analysis/
│
├── data/
│   └── breeds_raw.csv
│
├── images/
│   ├── distribucion_peso.png
│   ├── peso_vs_vida.png
│   └── vida_por_tamano.png
│
├── notebooks/
│   └── dog_breeds_analysis.ipynb
│
├── README.md
└── requirements.txt

### Cómo ejecutar el proyecto

Clonar este repositorio.

Crear un entorno virtual (opcional).

Instalar dependencias:

pip install -r requirements.txt


Definir la variable de entorno DOG_API_KEY con tu API Key de The Dog API.

Ejecutar el notebook dog_breeds_analysis.ipynb.

Conclusiones

El análisis sugiere que el tamaño y el peso de las razas de perros están estrechamente relacionados con su esperanza de vida.
Las razas pequeñas no solo son más frecuentes en el dataset, sino que también presentan una mayor longevidad promedio, mientras que las razas grandes tienden a vivir menos años y muestran mayor dispersión en sus valores.

Este proyecto demuestra el uso de datos reales obtenidos desde una API, así como habilidades de limpieza, análisis exploratorio y comunicación de resultados.

Contacto

Si quieres saber más sobre este proyecto o mi perfil profesional, puedes encontrarme en LinkedIn o GitHub.