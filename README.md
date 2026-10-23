# notebook-electiva-clase1

#Preguntas clase 1

1- Es necesario guardar los datos del CSV como una tabla permanente, por ejemplo, en formato Delta. Así, otros notebooks podrán consultarla sin tener que cargar nuevamente el archivo

2- Debemos revisar que las llaves utilizadas para unir las tablas no tengan valores duplicados. Si una llave aparece varias veces, puede multiplicar los registros y aumentar incorrectamente el importe total

3- No, Spark utiliza una evaluación diferida por lo que definir un filtro no ejecuta inmediatamente el cálculo. El procesamiento ocurre cuando se realiza una acción, como show() o count()

4- Además de SELECT, necesita permisos de USE CATALOG y USE SCHEMA para acceder al catálogo y al esquema donde se encuentra la tabla. Sin estos permisos, no podrá consultarla aunque tenga autorización de lectura

5- No, Aunque aparezca en el historial, es necesario comprobar que los archivos de esa versión todavía existan. Si fueron eliminados mediante VACUUM, puede que ya no sea posible recuperar los datos

6- Las ventas pueden quedar duplicadas porque append agrega nuevos registros sin reemplazar los existentes. Esto provocaría que los totales de ventas aumenten incorrectamente
