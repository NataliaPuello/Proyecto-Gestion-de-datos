# Proyecto-Gestion-de-datos

Integrantes:
- Eliana Romero Leon
- Ivan Trujillo Abella
- Natalia Puello Acosta

# Alcance y características del proyecto

El objetivo de este proyecto fue crear una API REST que permitiera generar 10 recomendaciones de canciones a partir de una canción ingresada por el usuario. Adicionalmente, se creó un dashboard que diera visual a las unidades de negocio del estado actual de la plataforma y comportamiendo de los indicadores de interés a la compañía.

# Pasos para ejecutar

# Extract
1. Descargar data sets de artistas y canciones https://drive.google.com/drive/folders/1toW8fa6ag4oNU00RuJHVUwhwEqmMsJaZ, puede encontrar una breve descripción de las variables aquí https://developer.spotify.com/documentation/web-api/reference/get-audio-features. 

# Transform  
2. Correr los scripts Artists y Tracks, estos hacen una limpieza inicial de los datos. La salida de estos son los csv artist_new, tracks_new, lastbase y remaster.
3. Correr script Intermedio Artists, este añade el género principal al data set artist_new y genera una nueva versión del mismo.

# Load
4. PostgreSQL: para hacer el cargue de los datos a esta herramienda se debe correr el script Load SQL.
5. BigQuery: en el script Load_Big_Query está el despliegue de los datos a Google Cloud Platform.
6. Autonomous Data Warehouse de Oracle : Crear el datawarehouse con 1 OCPU y 1 TB, adicionalmente se deben cargar las bases de datos de artists y tracks limpias.
7. Oracle Analytics Cloud : Desplegar el visualizador y crear la conexión con el Data Warehouse.


