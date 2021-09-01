# FOCA
OCA es una herramienta que permite extraer los metadatos de un fichero y/o buscar ficheros en una determinada web para posteriormente extraer sus metadatos, bien los metadatos básicamente son un grupo de datos que describen otros datos, es información “oculta” que puede existir dentro de algún fichero o incluso en las llamadas telefónicas y que nos proporciona más información sobre este.  Hay muchas herramientas para ver/modificar/eliminar metadatos, incluso hay algunas online, es solo cuestión de buscar. A las que más uso se les da son ExifTool y de la que estamos hablando, FOCA, este ultima de ElevenPaths, en este articulo veremos cómo podemos ver los metadatos de varios archivos usando FOCA.
Bien, empecemos, descarga FOCA y descomprime el .zip (todo esto partiendo que descargaste la “antigua FOCA”), al descomprimir, en la carpeta que te aparecerá, habrá un ejecutable llamado “FOCA.exe”, ejecútalo:



 

Y esta es la interfaz gráfica que tenemos a simple vista:



 

Extracción de metadatos de ficheros locales.
Ahora arrastra un fichero dentro de la interfaz gráfica, y luego da click en “Metadata” (ignorar el nombre de la máquina virtual):



 

Da clic derecho sobre el fichero en cuestión y da click en “Extract All Metadata” para extraer todos los metadatos:



 

Y nos arrojará los metadatos encontrados:



 

Claro, es un archivo de texto plano sin más, no hay mucho de interés por aquí, pero probemos esto con una imagen, por ejemplo:



Vemos que nos da más información, como el modelo de la cámara, cuándo fue hecha la foto, por qué usuario fue hecha, etc.

 

Extracción de metadatos de archivos sacados de un sitio web de dominio.
En este caso, desde el menú de FOCA, en la parte superior derecha, da click a “Project” > “New Project”:



 

Luego, rellena los campos y en el campo que pone “Domain website” es donde vas a poner el sitio web del cual quieres sacar archivos para posteriormente analizar sus metadatos y una vez hecho da click en “Create”:



 

Y guarda el proyecto:



 

Luego, en la parte superior derecha te saldrán los motores de búsqueda que puedes seleccionar para que FOCA busque los archivos, puedes seleccionarlos todos al igual que seleccionar también, todas las extensiones de los archivos que quieres:



 

En este punto ¿qué hará FOCA?, pues buscará archivos con todas esas extensiones en el sitio web que le indicamos, estos archivos también podemos conseguirlos nosotros de forma manual usando técnicas de Google Hacking por ejemplo, pero claro, en dicho caso tendríamos que conseguirlos manualmente, luego descargarlos y luego extraer los metadatos, FOCA hace de esto algo más automatizado.

 

Solo queda darle a “Search All” y empezará la búsqueda de ficheros en Google, Bing y Exalead:



 

Y nos salen ficheros pdf que son públicos, probemos descargar los tres primeros, para ello click derecho y “Download”:


Cuando se descarguen saldrán con un icono en verde a su derecha:

Posteriormente daremos clic derecho y extraemos todos los metadatos y analizamos los mismos y ya con eso podemos obtener información:

Para concluir, en una auditoria esta herramienta puede darnos una ventaja para poder saber qué hay dentro de la empresa que vamos a auditar, por ejemplo, si desde su sitio web logramos descargar algunos pdf, y al extraer sus metadatos podemos ver que han sido creados con el software Microsoft Office for MAC, pues podemos ir haciéndonos una idea de que en la empresa hay al menos una MAC, esto igualmente hay que comprobarlo y verificarlo revisando la mayoría de metadatos en los archivos y haciendo más recolección de información, además de que si nos detecta algún nombre de usuario, nombre de un ordenador, servidores, etc, nos pueden servir para ataques de ingeniería social por ejemplo, recuerda que hablo desde el punto de vista de una auditoría, no de acciones de ciberdelincuente.
