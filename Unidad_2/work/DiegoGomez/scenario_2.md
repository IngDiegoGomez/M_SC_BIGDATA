

# **Evidencia del escenario 2** 
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

