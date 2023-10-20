
# Big Data Architecture - Big Data Machine Learning Bootcamp

## Brainstorm


## Diseño del DAaaS

### Definicion de la estrategia del DAaaS

Crear un aplicacion web spa que mejore el acceso de los consumidores a la información, favorecer el funcionamiento de los mercados minoristas, estimulando la competencia y optimizando el proceso de difusión de precios.
La aplicación permitirá buscar, visualizar y predecirá los precios de más de 200 productos en más de 500 establecimientos.
Adicionalmente notificará las ofertas por debabjo del percentil diariamente a los suscriptores del servicio.

### Arquitectura DAaaS

Fuentes de datos
- Dataset de gobierno con los precios historicos desde 2007, [Licencia de DAG de Uruguay](https://www.gub.uy/agencia-gobierno-electronico-sociedad-informacion-conocimiento/sites/agencia-gobierno-electronico-sociedad-informacion-conocimiento/files/documentos/publicaciones/licencia_de_datos_abiertos_0.pdf)
  
- Crawler y Scrapper de las cadenas de establecimientos mas importarntes
  - https://www.devoto.com.uy/
  - https://tiendainglesa.com.uy/
  - https://www.tata.com.uy/
  - https://www.eldorado.com.uy/
Componentes
- Hadoop para procesamiento de datos
- Google Cloud Storage para ficheros de creawler, scrapper, dataset 
- Aplicacion Web
 - Angular Single Page Application
- API REST en Python/Flask
    
- Load Balancer para la gestion de peticiones http
- Base de datos Google Cloud SQL
- Big Query para Datawarehousing
- Cloud Functions para scrappers y crawlers
- Cloud Scheduler para la ejecucion de tareas programadas
- Firebase Cloud
- 
  
### DAaas Operantion Model Design and Rollout
  Tareas por unica vez
    Crear y configurar un Google Cloud Project "El_Mejor_Precio_UY" con un bucket de Cloud Storage
    Descargar Datasets historicos y subirlos a Google Cloud Storage
    Procesar los dataset históricos y subirlos a SQL Cloud
    Subir los Cloud Functions para el procesamiento de dataset historicos a Google Cloud Storage
    
    Crear una Cloud function que permita descargar los Dataset historicos y subir a Google Storage para automatizar la tarea
    Crear usuarios para ejecutar los Cloud functions
    Configurar Cloud Scheduler para la ejecucion de las tareas programadas
      - Crawler de recopilacion de datos mensual (planificacion mensual dias 1,3,5,7,10 hora 11 PM)
      - Crawler de recopilacion de ofertas diario (planificacion diaria hora 9 AM)
    
  
  
  
  Resultado de ejecucion se sube a Cloud Storage
  Crear un SQL que inserte los precios

  









