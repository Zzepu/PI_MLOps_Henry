# PI_ML_OPS_Henry
# <h1 align=center> **PROYECTO INDIVIDUAL Nº1** </h1>
# <h1 align=center>**`Machine Learning Operations (MLOps)`**</h1>

## **Introducción:**
Este proyecto se enfoca en desarrollar una API que utiliza un modelo de recomendación basado en Machine Learning para Steam, una plataforma global de videojuegos. El objetivo principal es establecer un sistema de recomendación de videojuegos personalizado para los usuarios. La API proporciona una interfaz fácil de usar que permite a los usuarios acceder a información relevante para el sistema de recomendación, así como datos relacionados con géneros y fechas específicas de lanzamiento.

## **Herramientas Utilizadas**
+ Pandas
+ Matplotlib
+ Numpy
+ Seaborn
+ Wordcloud
+ NLTK
+ Uvicorn
+ Render
+ FastAPI
+ Python
+ Scikit-Learn

## **Paso a paso:**
### 1. ETL
Llevamos a cabo un proceso de ETL (Extracción, Transformación y Carga), donde obtuvimos información de diversas fuentes, la modificamos según los requisitos del proyecto y la transferimos a un destino final para su análisis y posterior utilización. Las herramientas fundamentales que empleamos fueron Python, Pandas, Sklearn y FastApi.
### 2. Deployment de la API
Desde Python, construimos una API mediante el uso del módulo FastAPI, incorporando 5 funciones para su consulta:

1. **PlayTimeGenre(genero: str):** Retorna el año con mayor cantidad de horas jugadas para un género específico. Por ejemplo, con entrada "casual".

2. **UserForGenre(genero: str):** Ofrece el nombre del usuario que acumula más horas jugadas en el género proporcionado, junto con una lista de la acumulación de horas jugadas por año. Por ejemplo, con entrada "action".

3. **UsersRecommend(año: int):** Devuelve el top 3 de juegos más recomendados por usuarios para el año indicado, considerando revisiones con recomendaciones positivas o neutrales. Por ejemplo, con entrada "2012".

4. **UsersNotRecommend(año: int):** Muestra el top 3 de juegos menos recomendados por usuarios para el año dado, tomando en cuenta revisiones con recomendaciones negativas. Por ejemplo, con entrada "2009".

5. **sentiment_analysis(año: int):** Según el año de lanzamiento, proporciona una lista con la cantidad de registros de reseñas de usuarios categorizados con un análisis de sentimiento. Por ejemplo, con entrada "2014".

Posteriormente, implementamos el despliegue de esta API utilizando Render. Utilizamos herramientas como Uvicorn, Render y FastAPI.
### 3. EDA
Llevamos a cabo un análisis exploratorio de datos (EDA) en el que examinamos y estudiamos minuciosamente la información con el propósito de obtener percepciones valiosas, identificar patrones, tendencias y relaciones, con el fin de fundamentar nuestras decisiones en la información obtenida. Buscamos pistas que puedan ser útiles para la creación de nuestro modelo de machine learning.

En este proceso, use herramientas como Numpy, Pandas, Matplotlib, Seaborn, Wordcloud y NLTK.
### 4. Modelo de Machine Learning
Desarrolle un modelo de machine learning para generar recomendaciones de juegos, utilizando algoritmos y técnicas como la similitud del coseno y Scikit-Learn. El objetivo es proporcionar recomendaciones personalizadas y precisas basadas en los gustos y preferencias individuales de cada usuario.

Si se trata de un sistema de recomendación item-item, disponemos de una función llamada `recomendacion_juego(id_producto)`, donde al ingresar el ID de un producto, recibimos una lista con 5 juegos recomendados que son similares al producto ingresado. Por ejemplo, al utilizar el ID 76561198030567998.

En el caso de un sistema de recomendación user-item, contamos con la función `recomendacion_usuario(id_usuario)`, donde al ingresar el ID de un usuario, obtenemos una lista con 5 juegos recomendados específicamente para ese usuario. Por ejemplo, al utilizar el ID 70.

Para llevar a cabo estas recomendaciones, utilice Scikit-Learn junto con las bibliotecas TfidfVectorizer, linear_kernel y cosine_similarity. Además, estas funciones son accesibles a través de la API para su consulta.

## **Links:**
- [Deploy de la API en Render](https://pi-mlops-henry-sepulveda.onrender.com/)
- [Video de youtube explicando el proyecto](-)
## **Canales de contacto:**
+ Linkedin: [Jorge Tiago Nahuel Sepulveda](https://www.linkedin.com/in/tiago-sepulveda-047102243/)
+ Gmail : themindixhack@gmail.com
