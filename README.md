
# Big Data Architecture - Big Data Machine Learning Bootcamp

## Brainstorm


## Diseño del DAaaS

### Definicion de la estrategia del DAaaS
Catalogo de servicios
Crear un aplicacion web spa que mejore el acceso de los consumidores a la información para favorecer el funcionamiento de los mercados minoristas y estimular la competencia, optimizando el proceso de difusión de los precios.
La aplicación permitira buscar, predecir de los precios y mostrar graficas de más de 200 y de más de 500 establecimientos.
La interfaz web debera ser responsive, contar con una interfaz amigable y de facil compresión.
### Arquitectura DAaaS
Fuentes de datos
  Dataset de gobierno con los precios historicos desde 
  Dataset
  Crawler de las siguientes paginas
    
  Crawler de las siguientes paginas para obtener la informació diaria 
    https://www.elclon.com.uy/
    https://tiendainglesa.com.uy/
    https://www.tata.com.uy/
    https://www.eldorado.com.uy/
Componentes
  Google Cloud Storage para ficheros de creawler, dataset, scrapper
  Hadoop para procesamiento de datos
  Servidor Web
    API de Python
    Cliente
    Base de datos Google Cloud SQL
  Cloud Functions para scrappers y crawlers
  Cloud Scheduler
  
### DAaas Operantin Model Design and Rollout
  Crear y configurar un Google Cloud Project
  Descargar Dataset y subir a Google Storage
  Configurar la ejecucion de las tareas programadas con Google Cloud Scheduler :
    Crawler de recopilacion de datos mensual
    Crawler de 
    Resultado de ejecucion se sube a Cloud Storage
  Crear un SQL que inserte los precios

### Desarrollo de la plataforma DAaaS (Descripcipon del desarrollo)










