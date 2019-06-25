### Escenario 3 - Trabajando Remotamente


**Paso 1 - Git Remote**

Los repositorios remotos le permiten compartir cambios desde o hacia su repositorio. Las ubicaciones remotas son generalmente un servidor de compilación, una máquina de miembros del equipo o una tienda centralizada como Github.com. Los controles remotos se agregan utilizando el comando 
>git remote 

con un nombre descriptivo y la ubicación remota, generalmente una URL HTTPS o una conexión SSH, por ejemplo, https://github.com/OcelotUproar/ocelite.git o git@github.com: / OcelotUproar / ocelite.git.

El nombre descriptivo le permite referirse a la ubicación en otros comandos. Su repositorio local puede hacer referencia a varios repositorios remotos diferentes dependiendo de su escenario.

**Tarea**

Este entorno tiene una ubicación de repositorio remoto de / s / remote-project / 1. Usando 
>git remote, agregue esta ubicación remota con el origen de nombre.

**Protip**

Si utiliza 
>git clone 

que se analiza en un escenario futuro, entonces la ubicación desde la que está clonando se agregará automáticamente como un control remoto con el origen del nombre.


**Paso 2 - Git Push**

Cuando esté listo para compartir sus compromisos, debe enviarlos a un repositorio remoto a través de
> git push

Un flujo de trabajo típico de Git sería realizar múltiples confirmaciones pequeñas a medida que completa una tarea y lo empuja hacia un punto remoto en puntos relevantes, como cuando se completa la tarea, para garantizar la sincronización del código dentro del equipo.

**El comando git push es seguido por dos parámetros.** *El primer parámetro es el nombre descriptivo del repositorio remoto que definimos en el primer paso. El segundo parámetro es el nombre de la rama. Por defecto, todos los repositorios de git tienen una rama maestra donde se trabaja el código.*

**Paso 3 - Git Pull**

Donde **git push** *le permite enviar sus cambios a un repositorio remoto* 
**git pull** *funciona a la inversa.* 
>git pull 

le permite sincronizar los cambios de un repositorio remoto en su versión local.

Los cambios del repositorio remoto se fusionan automáticamente en la rama en la que está trabajando actualmente.

**Tarea**

Tire de los cambios desde el control remoto a su rama maestra.

En el siguiente paso exploraremos qué cambios se han hecho.
