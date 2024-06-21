# Azure end to end
Proyecto end to end Microsoft Azure + SQL + Databricks + Spark + Power BI 

## 1. Configuración del Proyecto:

### Creación de una base de datos SQL Server:
Se comienza con la creación de una base de datos SQL Server y la población de la misma con datos de muestra. Esta base de datos local servirá como origen de los datos que se transferirán a Azure Blob Storage.

### Creación de una cuenta de Azure Storage: 
Una cuenta de Azure Storage se crea para almacenar los datos transferidos desde el servidor SQL Server. Esta cuenta de almacenamiento en la nube proporcionará un repositorio escalable y accesible para los datos procesados.

## 2. Transferencia de Datos con Azure Data Factory:

### Establecimiento de una canalización de Azure Data Factory: 
Se crea una canalización de Azure Data Factory para automatizar la transferencia de datos desde el servidor SQL Server a la cuenta de Azure Blob Storage. Esta canalización define el flujo de datos y los componentes necesarios para la transferencia.

### Configuración de un entorno de ejecución de integración:
Un entorno de ejecución de integración se configura para permitir que Azure Data Factory se conecte al servidor SQL Server local. Este entorno de ejecución facilita la comunicación segura entre las instalaciones locales y la nube de Azure.

## 3. Procesamiento de Datos con Databricks:

### Creación de un clúster de Databricks: 
Se crea un clúster de Databricks para proporcionar recursos de computación en la nube para el procesamiento de datos. Este clúster escalable alojará los trabajos de Spark que transformarán los datos.

### Montaje del contenedor de Azure Blob Storage en Databricks: 
El contenedor de Azure Blob Storage que contiene los datos transferidos se monta en Databricks. Esto permite que los trabajos de Spark accedan y procesen los datos almacenados en la nube.

### Utilización de Spark SQL para crear una tabla agregada: 
Spark SQL, un lenguaje de consulta basado en SQL para Apache Spark, se utiliza para crear una tabla agregada a partir de los datos sin procesar. Esta tabla agregada contendrá los datos transformados y preparados para la visualización.

## 4. Visualización con Power BI:

### Conexión de Power BI a la tabla agregada en Databricks: 
Power BI Desktop se conecta a la tabla agregada creada en Databricks. Esta conexión permite que Power BI recupere y visualice los datos procesados.

### Creación de visualizaciones: 
Se crean diversas visualizaciones, como gráficos y tablas, para representar los datos de manera significativa. Estas visualizaciones proporcionarán información útil sobre los datos.

### Implementación de segmentadores y filtros: 
Se implementan segmentadores y filtros para permitir la exploración interactiva de los datos. Los usuarios podrán interactuar con las visualizaciones para filtrar y analizar los datos según sus necesidades.

## 5. Finalización del Panel de Control:

### Combinación de visualizaciones en un panel completo: 
Las visualizaciones creadas se combinan en un panel de control completo que proporciona una vista general integral de los datos.

### Personalización del diseño y el formato del panel: 
El diseño y el formato del panel se personalizan para mejorar la presentación y la facilidad de uso. Esto incluye la elección de colores, fuentes y la organización de las visualizaciones.

### Publicación del panel para compartir y acceder: 
El panel se publica para que otros usuarios puedan acceder y compartirlo. Esto permite la colaboración y el intercambio de conocimientos entre las partes interesadas.
