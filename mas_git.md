# Otras notas de git
git status

git fetch --all # Busca últimos cambios del remoto

git branch -a # Revisa las ramas locales y remotas

git log --oneline -5 master # Compara los últimos commits del master y el local

git pull origin main # Trae los cambios de origin main a la rama master local

git branch -r 
git branch -vv

git push origin master


En la web la rama principal se llama main (antes se llamaba master). Sobre la rama principal se pueden subir archivos pero no se pueden borrar. Lo mejor es crear una rama y trabajar en la misma tanto para subir como para bajar archivos. Cada vez que hagamos algo en esa rama se generará una pull request (solicitud de extracción) en la cual el github pide saber cuales son los cambios que hiciste para actualizar la rama main. 





