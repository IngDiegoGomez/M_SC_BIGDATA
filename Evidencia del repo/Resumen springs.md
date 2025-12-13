# **Resumen de spring durante el semestre** 
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)
[![VSCode](https://img.shields.io/badge/VS%20Code-Editor-007ACC?logo=visual-studio-code)](https://code.visualstudio.com/)
[![Docker](https://img.shields.io/badge/Docker-Container-2496ED?logo=docker)](https://www.docker.com/)
[![pgAdmin](https://img.shields.io/badge/pgAdmin-4-336791?logo=postgresql)](https://www.pgadmin.org/)
[![AWS](https://img.shields.io/badge/AWS-Cloud-FCC624?logo=amazon-aws&logoColor=black)](https://aws.amazon.com/)
[![Terraform](https://img.shields.io/badge/Terraform-Infrastructure-844FBA?logo=terraform)](https://www.terraform.io/)
[![Git](https://img.shields.io/badge/Git-Version%20Control-F05032?logo=git)](https://git-scm.com/)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?logo=github)](https://github.com/)
[![Big Data](https://img.shields.io/badge/Big%20Data-blue?logo=databricks&logoColor=white)](https://es.wikipedia.org/wiki/Big_data)
[![Apache Hadoop](https://img.shields.io/badge/Hadoop-yellow?logo=apache-hadoop)](https://hadoop.apache.org/)
[![Apache Spark](https://img.shields.io/badge/Spark-orange?logo=apache-spark)](https://spark.apache.org/)
[![Streaming Data](https://img.shields.io/badge/Streaming-%23DD006C?logo=streamlit&logoColor=white)](https://es.wikipedia.org/wiki/Transmisi%C3%B3n_de_datos)

## Spring 1
**BookstoneData** es una start-up que lanzó su nuevo método de pago hace ocho meses. Inicialmente, la empresa tenía alrededor de **750 clientes** y, desde entonces, ha sumado aproximadamente **150,000 nuevos clientes cada mes**. Este año, la proyección es alcanzar un incremento promedio de **225,000 clientes mensuales**.

BookstoneData opera mediante sprints de dos semanas, utiliza **Git** para el control de versiones y **GitHub** como plataforma central de colaboración y gestión de código para todos sus departamentos. Todos sus servicios están desplegados en la nube, usando **Amazon Web Services (AWS)** como proveedor principal.

**Este escenario simula la velocidad de crecimiento y los retos tecnológicos a los que te enfrenarás como **Junior Data Engineer**. Requiere soluciones de adquisición, almacenamiento, procesamiento, modelado y visualización de datos escalables y eficientes, alineadas con metodologías ágiles y Lean.**

## Bitacora
Para este Sprint, tus tareas incluyen:

1. **Implementacion de software requerido** para la empresa *BookstoneData*:  
    a. Creacion de cuentas:  
    06/09/2025:
    	* i. **AWS**: Cuenta creada y habilitado la autenticacion de dos factores.  
    	* ii. **GitHub**: Cuenta creada y activada, se realizo una primera activacion del servicio de la cuenta institucional sin exito debido a que no estaba configurado el nombre completo del usuario, asi como el nombre discrepaba del documento oficial otorgado para dicha verificacion, en un segundo intento con el horario se acredito y se verifico, antes de aplicar deben tener el nombre completo en el perfil como aparece en el documento de la escuela, igual en la parte de billing necesita el nombre completo y habilitar la autentificacion por dos factores para que la verificacion se efectue.

    b. Instalaciones en el sistema (Mac OS Sequoia 15.6.1):
    06/09/2025:  
    * i. Python: v.3.13.0  
    * ii. VS Code: 1.103.2 (Universal) 
    08/09/2025
    * iii. Docker Desktop: 4.45.0
    * iv. pgAdmin4: v.9.8   
    * v. AWS CLI: 2.28.25  
    * vi. Terraform: 1.13.1

    c. Práctica en Python la [manipulación de ficheros](/Unidad_1/work/DiegoGomez/manipulación_ficheros.py)

## Spring 2
**Procesamiento por lotes - *Desarrollo Local***

## Escenario
Para esta unidad / 2do sprint, necesitas investigar la fuente de datos de *BookstoneData*, comprender la cantidad de datos del año anterior e identificar los campos disponibles y sus tipos de datos. Prepara un pipeline ETL local para extraer los datos hacia la capa bronce (zona raw), aplicar las transformaciones necesarias hacia la capa plata (zona staging) y cargar los datos en la capa oro (zona confiable) para su consumo en el proceso analítico. Se requiere que la capa oro contenga cuatro tablas: una tabla financiera para los cálculos de pagos, una tabla técnica para analizar problemas técnicos, una tabla sin PII (non-PII) para acceso de todos los usuarios con acceso restringido en la organización, y una tabla con PII para usuarios con altos niveles de acceso.

## Actividad

    a. Investigar la fuente de datos.  -> Archivo generado y almacenado en "DiegoGomez", archivo nombrado "batch_2025-09-20.csv"
    b. Extraer datos:
    * i. Generador de datos.
    * ii. Extracción de datos.

    c. Transformar datos: -> Base de datos creada y procesada con las capas mencionadas
    * i. Capa bronce.
    * ii. Capa plata.

    d. Cargar datos: -> Capa oro creada y verificada.
    * i. Datos financieros.
    * ii. Datos de soporte.
    * iii. Datos sin PII.
    * iv. Datos PII.

    f. Scrapping -> Se realizo por medio de jupyter para su mejor visualizacion y creacion de outputs.
    * i. Abre el portal catastral de España.
    * ii. Selecciona la pestaña "Coordenadas".
    * iii. Introduce una latitud y longitud.
    * iv. Extrae los datos.

[Scraping a web de españa](/Unidad_2/work/DiegoGomez/scrapping.ipynb)

## Spring 3
** Procesamiento por lotes - *Pipeline local*

## Escenario

Para el 3er. sprint, debes crear un pipeline orquestado que permita que todas las etapas se ejecuten de manera gestionada. El pipeline debe ejecutarse diariamente y poner los datos disponibles a las 08:00 AM. Debe extraer datos en la capa bronze (zona cruda) llamada *driven_raw*, aplicar las transformaciones necesarias en la capa silver (zona de staging) llamada *driven_staging*, y cargar los datos en la capa golden (zona confiable) llamada *driven_trusted* para su consumo en el proceso analítico. Se requiere que la capa golden contenga cuatro tablas: una tabla financiera para cálculos de pagos, una tabla técnica para el análisis de incidencias técnicas, una tabla sin PII para usuarios con acceso limitado en toda la organización, y una tabla PII para usuarios con altos niveles de acceso.

[Proyecto local](/Unidad_3/work/DiegoGomez/)

## Spring 4
**Procesamiento por lotes - Nube: Pipeline desde la consola**
Para este Sprint, tus tareas incluyen:

a. Amazon Web Services -> Se inicia sesion en modo Root para esta practica:

![Image 1](/Unidad_4/work/DiegoGomez/img/Captura de pantalla 2025-11-11 a la(s) 2.16.23 p.m..png)

b. Configuración de servicios:

    * i. S3.
    ![Image 2](/Unidad_4/work/DiegoGomez/img/CCaptura de pantalla 2025-11-01 a la(s) 8.58.41 a.m..png)

    * ii. VPC.
    ![Image 3](/Unidad_4/work/DiegoGomez/img/Captura de pantalla 2025-11-01 a la(s) 8.58.55 a.m..png)
    
    * iii. MWAA.
    ![Image 4](/Unidad_4/work/DiegoGomez/img/Captura de pantalla 2025-11-01 a la(s) 8.48.33 a.m..png)

    * iv. IAM.
    ![Image 5](//Unidad_4/work/DiegoGomezimg/Captura de pantalla 2025-11-08 a la(s) 10.04.52 a.m..png)


c. Creación de servicios:

    * i. Crear trabajos de Glue (Glue jobs).
    ![Image 6](/Unidad_4/work/DiegoGomez/img/Captura de pantalla 2025-11-08 a la(s) 10.03.48 a.m..png)
    
    * ii. Crear base de datos en Athena.
    * iii. Crear Crawlers.
        - Ambos servicios se crearon de manera satisfactorias.

d. Ejecutar DAG:

    * i. Crear el DAG.
    * ii. Ejecutar el pipeline a través del DAG.

    - En este paso hubo inconvenientes ya que el DAG estuvo presente todo el tiempo en el dag.
    ![Image 7](/Unidad_4/work/DiegoGomez/img/Captura de pantalla 2025-11-07 a la(s) 3.37.21 p.m..png)

    -Pero no fue visible para Airflow:
    ![Image 8](/Unidad_4/work/DiegoGomez/img/Captura de pantalla 2025-11-11 a la(s) 1.52.07 p.m..png)

    - Inclusive dando permisos necesario para la visibilidad:
    ![Image 9](/Unidad_4/work/DiegoGomez/img/Captura de pantalla 2025-11-08 a la(s) 10.40.53 a.m. (2).png)
    
    - Se intentaron varias opciones sin exito alguno y llegando al limite del budget:
    ![Image 9](/Unidad_4/work/DiegoGomez/img/Captura de pantalla 2025-11-11 a la(s) 1.57.11 p.m..png)


