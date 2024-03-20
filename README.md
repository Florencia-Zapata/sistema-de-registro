<h1>Sistema de Registro</h1>

-Estado del proyecto en construcción.

Para ejecutar el sistema, debes poner:

`npm install react`

COMANDOS IMPORTANTES PARA SABER DE GITHUB

GIT CLONE:

El comando git clone crea una copia de un repositorio git existente, y este repositorio puede ser local o remoto. Además, esta copia es un repositorio git completo, con tu propio historial, gestionamiento de tus propios archivos y es un ambiente aislado como un todo del repositorio original.

SERIA: `git clone <repositorio> <mi-proyecto-clone>`

El repositorio localizado en repositorio es clonado para una carpeta llamada:

`mi-proyecto-clone`

También puedes configurar el git clone y clonar el repositorio desde una branch específica, diferente a la original, de esta manera:

`git clone -branch new_feature <repositorio>`

GIT LOG:

Si deseas verificar el historial de cambios, los mensajes de commit, el nombre de la persona autora del commit y otras informaciones sobre el proyecto, hay un comando de git que te puede ayudar. Este comando es git log.

Como ya sabemos, los commits poseen hashs que los identifican de una manera única, es decir, no existen dos commits con el mismo hash. Con git log podemos ver el hash y muchas otras informaciones del commit.

Podemos visualizar todos los commits, uno en cada línea con el comando:

`git log –oneline`

Si, en lugar de menos informaciones, queremos ver más, como las alteraciones del commit, podemos usar:

`git log -p`

También podemos buscar las informaciones de la persona autora del commit con el comando:

`git log --author="user_name"`

Y buscar informaciones por fecha:

`git log --since=1.month.ago --until=1.day.ago`

En el comando anterior, estamos buscando las informaciones del commit desde hace un mes hasta hace un día.

Tu también puedes formatear la visualización de las informaciones del commit con el comando:

`git log --pretty="format:%h %s"`

Para limpiar la terminal de git bash:

`clear`

```

```
