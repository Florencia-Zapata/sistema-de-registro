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

- Para verificar los cambios realizados:

  Utiliza el comando `git status`, sirve para listar todos los archivos que han sido modificados.

2 - Para agregar los cambios al repositorio local:

Para agregar los cambios realizados de una sola vez, es necesario usar `git add . `(git add y un punto) y, para agregar los cambios en algún archivo específico, usamos a `git add nombre-del-archivo-modificado`.

3 - Para guardar los cambios:

Utiliza el comando `git commit -m "Comentario que quiero"`, que sirve para capturar y guardar el estado actual del repositorio.

4 - Para enviar las modificaciones al repositorio remoto:

Utiliza el comando `git push`, que sirve para enviar las modificaciones guardadas en el directorio local para el repositorio remoto.

5 - Para bajar al repositorio local cambios realizados en el repositorio que esta en github:

Utiliza el comando `git pull`, que sirve para bajar a nuestro directorio local cualquier modificación realizada en el repositorio remoto. Siempre chequear con `git status` para saber que estoy bien parada.

6 - Para restaurar archivos y el proyecto, volviendo a un estado anterior a través de `git restore`.

```

```

Ejercicio práctico:

Estás haciendo un curso en Alura y te gustaría dividir el código del proyecto por aulas, para organizarse mejor, no perder el código antíguo después de una refactorización y conseguir revisar tu evolución. ¿Cómo puedes hacer eso?

Camino 1: crear una branch para cada clase del curso con el comando:

git checkout -b git branch nombre-de-la-branch
COPIA EL CÓDIGO
Con este comando, crearás una nueva branch y cambiarás automáticamente a ella para dar inicio al proceso de desarrollo.

Camino 2: crear una branch para cada clase del curso con el comando:

git branch nombre-de-la-branch
COPIA EL CÓDIGO
Esta es otra forma de crear una branch. En este caso, ella es creada, pero no hay cambio automático a esta nueva ramificación. Para eso, puedes usar el comando git switch nombre-de-la-branch.
