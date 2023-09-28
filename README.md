# Git Diff Command

El comando `git diff` es una herramienta poderosa en Git que te permite ver las diferencias entre las versiones de tus archivos en un repositorio. Puedes usarlo para entender qué cambios se han realizado, qué líneas se han añadido o eliminado, y mucho más. A continuación, se describen las principales características de `git diff`.

## Uso Básico

El comando `git diff` se utiliza para mostrar las diferencias entre el área de trabajo y el área de preparación (staging) o entre dos commits. Aquí tienes ejemplos de uso básico:

- Para ver las diferencias entre el área de trabajo y el área de preparación:

  `git diff`

- Para ver las diferencias entre el área de preparación y el último commit:

  `git diff --staged`

- Para ver las diferencias entre dos commits específicos:

  `git diff commit1 commit2`

## Opciones Comunes

- `--color`: Resalta las diferencias con colores para una mejor visualización.
- `--stat`: Muestra un resumen estadístico de las diferencias.
- `--cached`: Muestra las diferencias entre el área de preparación y el último commit.
- `--word-diff`: Muestra las diferencias a nivel de palabras en lugar de líneas completas.
- `--ignore-space-change`: Ignora los cambios de espacios en blanco.
- `--ignore-all-space`: Ignora todos los cambios de espacios en blanco.
- `--name-only`: Muestra solo los nombres de los archivos modificados.
- `--name-status`: Muestra el nombre de los archivos y un indicador de estado (M para modificado, A para añadido, D para eliminado, etc.).

## Ejemplos Avanzados

- Para ver las diferencias entre la rama actual y otra rama:

  `git diff branch_name`

- Para ver las diferencias entre dos commits en un archivo específico:

  `git diff commit1 commit2 path/to/file`

- Para ver las diferencias en un rango de commits:

  `git diff commit1..commit2`
  
## Recursos Adicionales

Para obtener más información sobre el comando `git diff` y sus opciones, consulta la documentación oficial de Git usando el siguiente comando:

 `git help diff`

## A continuación un ejemplo con un video:


[![](http://img.youtube.com/vi/qsZgk0AbAAc/0.jpg)](https://www.youtube.com/watch?v=qsZgk0AbAAc "")






# Git Checkout Command

El comando `git checkout` es una herramienta fundamental en Git que te permite cambiar entre ramas, commits, y más. Se utiliza para moverte por el historial de tu repositorio Git y administrar tus ramas y archivos de trabajo. A continuación, se describen las principales características de `git checkout`.

## Cambiar de Rama

El uso más común de `git checkout` es cambiar entre ramas en tu repositorio. Puedes hacerlo de la siguiente manera:

`git checkout nombre_de_la_rama`

- Si la rama existe, te moverás a esa rama y tu directorio de trabajo se actualizará con los archivos de esa rama.

- Si la rama no existe, Git mostrará un error.

## Crear Nuevas Ramas
También puedes utilizar `git checkout` para crear y cambiar a una nueva rama en un solo paso:

 `git checkout -b nueva_rama`

Esto creará una nueva rama llamada `nueva_rama` y te cambiará automáticamente a ella.

## Cambiar a un Commit Específico
Puedes usar `git checkout` para moverte a un commit específico en la historia del proyecto. Esto crea un estado "desconectado" en el que no puedes hacer cambios, pero puedes revisar el estado de tu proyecto en ese commit:

`git checkout commit_hash`

- `commit_hash` es el identificador único del commit al que quieres moverte.

## Deshacer Cambios en un Archivo
Si has realizado cambios en un archivo y deseas deshacer esos cambios, puedes usar `git checkout` para volver al estado del archivo en el último commit:

 `git checkout -- nombre_del_archivo`

## Recuperar Archivos Eliminados
Si has eliminado un archivo y deseas recuperarlo, puedes usar `git checkout` para hacerlo:

 `git checkout nombre_del_archivo`

Esto restaurará el archivo eliminado en tu directorio de trabajo.

## Cambiar Ramas de Forma Forzada
Si necesitas cambiar de rama incluso si tienes cambios sin confirmar en tu directorio de trabajo, puedes usar la opción `-f` o `--force`:

 `git checkout -f nombre_de_la_rama`

## Recursos Adicionales
Para obtener más información sobre el comando git checkout y sus opciones, consulta la documentación oficial de Git utilizando el siguiente comando:

 `git help checkout`

 ## A continuación un ejemplo con un video:


[![](http://img.youtube.com/vi/XFsh-cXkH4s/0.jpg)](https://www.youtube.com/watch?v=XFsh-cXkH4s "")
 

 Este archivo README proporciona una introducción básica a `git checkout` y `git diff`, pero hay muchas más opciones y características disponibles. ¡Explora y experimenta para aprovechar al máximo estas poderosas herramientas de Git!







