# powerbi-api-swagger

Archivo OpenAPI con la REST API de Power BI. 

Copiado de https://github.com/Microsoft/PowerBI-CSharp/tree/master/sdk/swaggers.


Modificado para facilitar la creación de un conector personalizado para Microsoft Flow y Power Apps
* Eliminado el punto al final de la propiedad "summary" de las acciones, para que no de error al guardar el flujo sino se se modifica el tíy¡tulo por defecto de la acción.
* Adicionado el tipo "object" en todas las referencias, para que se puedan utilizar los resultados de la acciones en Power Apps.
* Adicionando el parámetro "pbixFile" a las acciones Imports_PostImport e Imports_PostImportInGroup, para permitir adjuntar un archivo PBIX.
