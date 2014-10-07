ckanext-intro-changes
=====================

Extiende la funcionalidad del plugin **intro** para que además de retornar la lista de datasets, retorne la lista de los datasets que fueron modificados recientemente.

Instalación y configuración
---------------------------
1. Activar el entorno virtual
    
 `$ . ~/ckan/lib/default/bin/activate`
    
2. Ingresar al directorio de extensiones
    
 `$ cd ~/ckan/lib/default/src/`

3. Clonar este proyecto

 `$ git clone https://github.com/ckanext-intro-changes.git`
    
4. Ingresar al directorio de la extensión e instalar el plugin

 `$ cd ckanext-intro-changes`
    
 `$ python setup.py develop`

4. Agregar el plugin en el archivo development.ini del CKAN, el nombre del plugin es **changes_plugin**


Uso
---

Ingresar a la dirección donde se encuentra levantado el CKAN y agregar **/changes**. Esto descargará un archivo **csv** con la información correspondiente a los últimos datasets modificados, las columnas son: 
* timestamp (la fecha de la última modificación), 
* package name (el nombre del dataset) , 
* package title (el título del dataset) y,
* activity type (tipo de operación que se realizó sobre el dataset).

