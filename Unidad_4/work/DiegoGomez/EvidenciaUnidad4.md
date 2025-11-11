

# Bitacora de la unidad 4
**Procesamiento por lotes - Nube: Pipeline desde la consola**

>**NOTA:** Esta Unidad 4 implica trabajar con servicios en la nube que son cobrados por el proveedor de nube. Consulta el [Calculador de precios de AWS](https://calculator.aws/#/) para estimar el costo de los servicios utilizados en esta unidad. Si decides continuar, utiliza tus credenciales de estudiante, de no ser así lo haces bajo tu propia responsabilidad; el autor no se hace responsable de los costos resultantes.

## Escenario

Para el 4to. sprint, necesitas consolidar el pipeline desarrollado en tu máquina local, optimizar los procesos del pipeline, crear la arquitectura en la nube para asegurar que el producto sea robusto y escalable, implementar la arquitectura propuesta a través de la consola de AWS, y validar el pipeline *BookstoneDriven* en la nube.

## Actividad

Para este Sprint, tus tareas incluyen:

a. Amazon Web Services -> Se inicia sesion en modo Root para esta practica:

![Image 1](/img/Captura de pantalla 2025-11-11 a la(s) 2.16.23 p.m..png)

b. Configuración de servicios:

    * i. S3.
    ![Image 2](/img/CCaptura de pantalla 2025-11-01 a la(s) 8.58.41 a.m..png)

    * ii. VPC.
    ![Image 3](/img/Captura de pantalla 2025-11-01 a la(s) 8.58.55 a.m..png)
    
    * iii. MWAA.
    ![Image 4](/img/Captura de pantalla 2025-11-01 a la(s) 8.48.33 a.m..png)

    * iv. IAM.
    ![Image 5](/img/Captura de pantalla 2025-11-08 a la(s) 10.04.52 a.m..png)


c. Creación de servicios:

    * i. Crear trabajos de Glue (Glue jobs).
    ![Image 6](/img/Captura de pantalla 2025-11-08 a la(s) 10.03.48 a.m..png)
    
    * ii. Crear base de datos en Athena.
    * iii. Crear Crawlers.
        - Ambos servicios se crearon de manera satisfactorias.

d. Ejecutar DAG:

    * i. Crear el DAG.
    * ii. Ejecutar el pipeline a través del DAG.

    - En este paso hubo inconvenientes ya que el DAG estuvo presente todo el tiempo en el dag.
    ![Image 7](/img/Captura de pantalla 2025-11-07 a la(s) 3.37.21 p.m..png)

    -Pero no fue visible para Airflow:
    ![Image 8](/img/Captura de pantalla 2025-11-11 a la(s) 1.52.07 p.m..png)

    - Inclusive dando permisos necesario para la visibilidad:
    ![Image 9](/img/Captura de pantalla 2025-11-08 a la(s) 10.40.53 a.m. (2).png)
    
    - Se intentaron varias opciones sin exito alguno y llegando al limite del budget:
    ![Image 9](/img/Captura de pantalla 2025-11-11 a la(s) 1.57.11 p.m..png)



