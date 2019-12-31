---
title: Control de versiones
date: 2019-09-19
draft: true
--- 
# Control de versiones
En esta lectura se habla de algunos conceptos básicos sobre las herramientas de control de versiones y el fucionamiento de Git en nuestro sistema. 
Es un sistema que registra los cambios realizados en un archivo para que posteriormente se puedan recuperar versiones específicas. Este sistema, además de `posibilitar la recuperación de versiones anteriores, permite ver quién lo ha modificado y cuándo,y permite diagnosticar los errores y verificar su origen.
1. Sistemas de Control de Versiones locales 
- Se trata de un mecanismo en el que se copian archivos a otro directorio.
- Es un mecanismo común pero propenso a errores. 

-	Una de las versiones más populares es el sistema RSC, que funciona guardando conjuntos de parches( las diferencias entre archivos) en un formato especial en disco. 
2. Sistemas de control de versiones centralizadas
- Se usa este sistema cuando las personas necesitan colaborar con desarrolladores de otros sistemas. 
- Estos sistemas tienen un único servidor que contiene todos los archivos versionados y varios clientes que descargan los documentos desde ese lugar central. 
- Ventajas frente a VCS: todos los miembros del equipo saben en qué están trabajando los demás. 
-  Desventajas: Si el servidor cae, ningún miembro del equipo podrá trabajar hasta que se recupere. 
3. Sistema de control de versiones distribuidos
- Este sistema ofrece mejoras y soluciones a los dos anteriores. 
- Los clientes no descargan la última copia, sino que se replica completamente en el repositorio. 
- Si un servidor deja de funcionar, cualquiera de los repositorios disponibles puede ser copiado al servidor. 
- Permite colaborar simultáneamente a diferentes equipos y personas dentro de un proyecto y establecer modelos de trabajo jerárquicos.

GIT
Creado en 2005, tras la caída de Bitkkeper, una herramienta parecida en el que se creaban cambios en el software a través de parches y archivos. Estos han sido los fundamentos de esta herramienta:  
1.	Copias instantáneas, no diferencias. La ventaja de Git es que la información que almacena se estructura como un conjunto de archivos y las modificaciones hechas en cada versión. 
2.	Casi todas las operaciones son locales, y por tanto, no depende de Internet. 
3.	Git tiene integridad. Se verifica y comprueba a través de una comprobación numérica que imposibilita la alteración de contenidos sin que el sistema lo sepa. 
4.	Git generalmente solo añade información y es muy difícil que el sistema pueda perder datos. 

### Los tres estados 
Git tiene tres estados principales: 
1.	Confirmado (committed): Cuando está confirmado significa que el cambio ya está almacenado de forma segura. 
2.	Modificado (modified): Cuando está modificado, significa que el cambio se ha realiado pero que todavía no se ha confirmado a la base de datos. 
3.	Preparado (staged): Cuando está preparado significa que se ha mercado un archivo para que vaya en la próxima confirmación. 

El funcionamiento de Git es el siguiente: 
1.	Se modifica un archivo en el directorio de trabajo. 
2.	Los cambios realizados pasan al área de preparación, en el que se almacena información acerca de la próxima confirmación. 
3.	Confirmas los cambios (commit) y pasan al directorio de Git. 
