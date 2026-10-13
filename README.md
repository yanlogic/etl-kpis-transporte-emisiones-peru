# Proyecto de Análisis de Datos y Sistemas

Este repositorio se encuentra actualmente en **fase de desarrollo**.

Debido a esto, la documentación y el contenido disponible se mantendrán

de forma breve y se actualizarán conforme avance el cronograma del

proyecto.

## Estado del Proyecto

✅ **COMPLETADO**

## Implementación de los Datasets al proyecto Power BI

Dado a que Power BI trabaja con un directorio especifico y local para los DataSets, al abrir los archivos Dashboard_mvp.pbix y queries_integracion.pbix es posible que haya errores en la lectura de estos mismos.

Para ello se recomienda lo siguiente:

Una vez dentro de uno de los archivos

- Ingresar a Power Query (transformar datos)

- Seleccionar uno de los datasets

- Click derecho en el y entrar al "editor avanzado"

- dentro de las líneas escritas ahí, editar la linea a continuación y colocar la ruta de la carpeta que contiene los datasets de la carpeta [UAIN1008R_Proyecto/datos/processed]:

Origen = Csv.Document(File.Contents("C:\Users\Usuario\Downloads\datos-20260508T023005Z-3-001\datos\processed\Limpio - Información Trafico - Carga y Operaciones.CSV"))

En caso de tener la carpeta en el escritorio, un ejemplo sería:

Origen = Csv.Document(File.Contents("C:\Users\Usuario\Desktop\Carpeta\_Datasets\Dataset\_elegido.CSV"))

De igual manera, si llega a tener un problema similar con los archivos .ipynb , deberá seguir un proceso similar:

- Necesita descargar la carpeta "UAIN1008R_Proyecto" del repositorio del proyecto y pegarla directamente en su unidad "MyDrive" principal

Se recomienda usar GOOGLE COLAB para la visualizacion de los archivos .ipynb

Se ha decidido integrar este archivo en este directorio debido a que

Power BI ha servido como la herramienta principal para: \* **Diseño y

Prototipado de Dashboards:
** Visualización preliminar de KPIs y métricas clave. 
* **Modelado de Datos:** Facilitar la lógica de relación entre tablas mediante el uso de **JOINS**. 
* **Agregaciones:** Pruebas de lógica de negocio utilizando operaciones de **GROUP BY** para validar la integridad de la información antes de su implementación final en el motor de base de datos.

------------------------------------------------------------------------

*Última actualización: Mayo 2026*