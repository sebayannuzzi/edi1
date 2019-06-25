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

**Paso 4 - Registro Git**

Como se describe en el escenario anterior, puede usar el comando 
>git log 

para ver el historial del repositorio. 

El comando 
>git show 

le permitirá ver los cambios realizados en cada confirmación.

En este ejemplo, la salida del registro de git muestra una nueva confirmación por "DifferentUser@JoinScrapbook.com" con el mensaje "Corrección para el error # 1234". La salida de git show resalta las nuevas líneas agregadas al archivo en verde.

**Protip**

Use el comando 
>git log --grep = "# 1234" 

para encontrar todas las confirmaciones que contienen # 1234.

**Paso 5 - Git Fetch**

El comando git pull es una combinación de dos comandos diferentes, **git fetch y git merge.** 
>git fetch

Fetch descarga los cambios del repositorio remoto en una rama separada llamada remotes / <remote-name> / <remote-branch-name>. Se puede acceder a la sucursal usando git checkout.

Usar git fetch es una excelente manera de revisar los cambios sin afectar tu rama actual. El formato de nomenclatura de las sucursales es lo suficientemente flexible como para que pueda tener varios controles remotos y sucursales con el mismo nombre y cambiar fácilmente entre ellas.

El siguiente comando fusionará los cambios recuperados en el maestro.

>git merge remotes

<remote-name> / <remote-branch-name> master

Cubriremos la fusión con más detalle en un escenario futuro.

**Tarea**

Se han realizado cambios adicionales en el repositorio de origen. Use git fetch para descargar los cambios y luego verifique la rama para verlos.

**Protip**

Puede ver una lista de todas las ramas remotas usando el comando 

>git branch -r


