
# Big Data Architecture - Big Data Machine Learning Bootcamp

## Brainstorm


## Diseño del DAaaS

### Definicion de la estrategia del DAaaS
Catalogo de servicios
Crear un pagina web para buscar, predecir y mostrar graficas de precios de 200 productos de la canasta basica
Ademas quiero mostrar ofertas y publicidad de esos relojes

### Arquitectura DAaaS
Fuentes de datos
  Dataset
  Dataset
  Crawler de las siguientes paginas
    
  Crawler de las siguientes paginas
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










