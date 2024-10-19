# Proyecto de Análisis de YouTube con Ingeniería de Datos  

## Descripción General  

Este proyecto tiene como objetivo gestionar de manera segura, optimizar y analizar datos estructurados y semiestructurados de videos de YouTube, basándose en las categorías de video y las métricas de tendencias.

---

## Objetivos del Proyecto  

1. **Ingesta de Datos**  
   - Construir un mecanismo para ingerir datos desde diferentes fuentes.

2. **Sistema ETL**  
   - Recibir datos en formato bruto y transformarlos en un formato adecuado para su análisis.

3. **Lago de Datos**  
   - Al recopilar datos de múltiples fuentes, necesitamos un repositorio centralizado para almacenarlos.

4. **Escalabilidad**  
   - Asegurar que el sistema pueda escalar a medida que aumente el volumen de datos.

5. **Uso de la Nube**  
   - Dado que el procesamiento de grandes volúmenes de datos no es posible en equipos locales, utilizaremos la nube (AWS en este caso).

6. **Informes y Visualización**  
   - Crear un dashboard para responder a las preguntas de análisis planteadas.

---

## Servicios Utilizados  

- **Amazon S3:**  
  Servicio de almacenamiento de objetos que ofrece escalabilidad, disponibilidad de datos, seguridad y alto rendimiento.  
- **AWS IAM:**  
  Administración de identidades y accesos para gestionar de forma segura el acceso a servicios y recursos en AWS.  
- **Amazon QuickSight:**  
  Servicio de inteligencia empresarial (BI) escalable y sin servidor, con capacidades de machine learning, diseñado para la nube.  
- **AWS Glue:**  
  Servicio de integración de datos sin servidor que facilita la preparación y combinación de datos para análisis, aprendizaje automático y desarrollo de aplicaciones.  
- **AWS Lambda:**  
  Servicio de computación que permite ejecutar código sin necesidad de gestionar servidores.  
- **AWS Athena:**  
  Servicio de consultas interactivas para datos en S3, donde no es necesario cargar los datos, ya que permanecen en S3.

---

## Conjunto de Datos Utilizado  

Este conjunto de datos de **Kaggle** contiene estadísticas en formato CSV sobre los videos más populares de YouTube durante varios meses. Cada día se publican hasta 200 videos en tendencia por región, y los datos de cada una se encuentran en archivos separados.  

**Características del dataset:**  

- Título del video  
- Canal del video  
- Fecha de publicación  
- Etiquetas  
- Vistas, me gusta y no me gusta  
- Descripción  
- Cantidad de comentarios  
- `category_id`: Campo específico en formato JSON que varía según la región.

[Enlace al Dataset de Kaggle](https://www.kaggle.com/datasets/datasnaek/youtube-new)

---

## Diagrama de Arquitectura  

![alt text](architecture.jpeg)

---

Este proyecto busca demostrar cómo aplicar técnicas modernas de ingeniería de datos para gestionar y analizar grandes volúmenes de información utilizando servicios en la nube.

# YT_analysis-AWS-project
