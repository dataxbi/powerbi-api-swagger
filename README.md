# powerbi-api-swagger

Fichero OpenAPI con la REST API de Power BI. 

Copiado de https://github.com/Microsoft/PowerBI-CSharp/tree/master/sdk/swaggers.


Modificado para facilitar la creación de un conector personalizado para Power Automate y Power Apps
* Eliminado el punto al final de la propiedad "summary" de las acciones, para que no de error al guardar el flujo sino se se modifica el tíy¡tulo por defecto de la acción.
* Adicionado el tipo "object" en todas las referencias, para que se puedan utilizar los resultados de la acciones en Power Apps.
* Adicionando el parámetro "pbixFile" a las acciones Imports_PostImport e Imports_PostImportInGroup, para permitir adjuntar un archivo PBIX.

Se ha separado en otro archvo la API para ejecutar consultas DAX, para poder crear un conector personalizado que sólo tenga la acción DAX query.
