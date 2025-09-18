# Otras notas de git
git status

git fetch --all # Busca últimos cambios del remoto

git branch -a # Revisa las ramas locales y remotas

git log --oneline -5 master # Compara los últimos commits del master y el local

git pull origin main # Trae los cambios de origin main a la rama master local

git branch -r 
git branch -vv

git push origin master

## Que es un pull request?
En la web la rama principal se llama main (antes se llamaba master). Sobre la rama principal se pueden subir archivos pero no se pueden borrar. Lo mejor es crear una rama y trabajar en la misma tanto para subir como para bajar archivos. Cada vez que hagamos algo en esa rama se generará una pull request (solicitud de extracción) en la cual el github pide saber cuales son los cambios que hiciste para actualizar la rama main. 

## Que es un fork?

Para qué sirve un fork?

La razón principal para hacer un fork es poder modificar el código de un proyecto sin afectar el repositorio original. Esto es fundamental en el desarrollo de código abierto. Por ejemplo, si quieres:
  - Hacer cambios o correcciones: Si encuentras un error en un proyecto de código abierto, haces un fork del repositorio, arreglas el error en tu copia y luego le propones al creador original que incorpore tu cambio a su proyecto principal a través de un Pull Request (solicitud de extracción).
  - Añadir una nueva funcionalidad: Si quieres agregar una nueva característica, puedes hacerlo en tu fork sin tener que pedir permiso al creador del proyecto.
  - Usar el código para tu propio proyecto: Puedes tomar el código de un proyecto público, hacer un fork para tener una copia y usarlo como punto de partida para tu propio trabajo.

El fork crea un enlace permanente entre tu repositorio y el original. Esto te permite "traer" las últimas actualizaciones del proyecto original a tu copia (sync fork) y, si quieres, "enviar" tus cambios al original (pull request).

Cuando tu propuesta de modificación es aceptada, el creador del repositorio lo que hace es fusionar (o merge) tus cambios en su rama principal.
### El proceso de fusión
El proceso es el siguiente:
  - El creador recibe una notificación de tu pull request (solicitud de extracción).
  - Revisa los cambios que propusiste. Si está de acuerdo con ellos, aprueba el pull request.
  - Hace clic en el botón "Merge pull request" en la interfaz de GitHub.
  - GitHub toma el código de tu rama y lo integra automáticamente en la rama main del repositorio original.

Una vez que se fusionan tus cambios, tu propuesta se convierte en parte del proyecto original y tu pull request se cierra. Si tu pull request solo incluía esos cambios, puedes eliminar tu rama y, si no planeas hacer más contribuciones, incluso el fork que hiciste.

Puedes pensarlo como un plano maestro del proyecto . Tu pull request es una sugerencia de mejora para ese plano. Cuando el creador lo aprueba y fusiona, esa mejora se convierte en parte oficial del plano original.

Reocdar que git commit crea una versión local del estado del directorio (no hace nada en la nube) para ir a la nube hay que usar pull o push.



