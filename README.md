
# Big Data Architecture - Big Data Machine Learning Bootcamp

## Brainstorm


## Diseño del DAaaS

### Definicion de la estrategia del DAaaS
Crear un aplicacion web spa que mejore el acceso de los consumidores a la información, favorecer el funcionamiento de los mercados minoristas, estimulando la competencia y optimizando el proceso de difusión de precios.
La aplicación permitira buscar y predecir los precios de más de 200 productos en más de 500 establecimientos.

Los dataset se distribuyen bajo la [Licencia de DAG de Uruguay]([https://choosealicense.com/licenses/mit/](https://www.gub.uy/agencia-gobierno-electronico-sociedad-informacion-conocimiento/sites/agencia-gobierno-electronico-sociedad-informacion-conocimiento/files/documentos/publicaciones/licencia_de_datos_abiertos_0.pdf))
### Arquitectura DAaaS
Fuentes de datos
  Dataset de gobierno con los precios historicos desde 
  Dataset
  Crawler de las siguientes paginas
    
  Crawler de las siguientes paginas para obtener la informació diaria 
    - https://www.elclon.com.uy/
    - https://tiendainglesa.com.uy/
    - https://www.tata.com.uy/
    - https://www.eldorado.com.uy/
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
  Tareas por unica vez
    Crear y configurar un Google Cloud Project "El_Mejor_Precio_UY"
    Crear una Cloud function que permita descargar los Dataset historicos y subir a Google Storage para automatizar la tarea
    Crear usuarios para ejecutar los Cloud functions
    Configurar Cloud Scheduler
      - 
  Procesar los dataset históricos y subirlos a SQL Cloud
  Configurar la ejecucion de las tareas programadas con Google Cloud Scheduler :
    Crawler de recopilacion de datos mensual
    Crawler de 
    Resultado de ejecucion se sube a Cloud Storage
  Crear un SQL que inserte los precios

### Desarrollo de la plataforma DAaaS (Descripcipon del desarrollo)
  Crear una Cloud function en Python denominada "CF_DescargarHistoricos.py" que permita descargar los Dataset historicos y subir a Google Storage para automatizar la tarea









