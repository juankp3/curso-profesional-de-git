### Curso de profesional de Git

#### Resumen:
Git es un sistema de control de versiones que nos ayuda a ver la evolución de un proyecto de software de inicio a fin e incluso en proyecto existente; desde proyectos pequeños hasta muy grandes, con velocidad y eficiencia.
Al implementar este sistema de control de versiones tenemos grandes ventajas para trabajar en equipo haciéndolo de forma ordenada, uniendo códigos, deshacer cambios, establecer versiones, revisar los cambios, ver responsables, arreglar conflictos, etc..

#### Requisitos:
- Conocimientos básicos de computación.
- Muchas ganas de aprender

#### Metodología:
- Exposición teórica de los temas.
- Desarrollo de casos prácticos progresivos.
- Evaluación continua (teórica y práctica en cada sesión).
- Tecnologías:
- Versión Git: 2.0 a más
- IDE Visual Studio Code



## Sesiones:
### Sesión 1: Introducción a Git
Descripción: 
- ¿Qué es Git? y ¿Cómo funciona? (Historia, evolución, tendencias, ventajas y desventajas).
- Instalación y configuración.
- Comandos útiles en la terminal (Vim, cd, touch, mkdir, cat, pwd,).
- Las 3 áreas y estados de git.
- Mi primer repositorio. (git init)
- Agregar, quitar y ver el estado de archivos. (git add,rm,status)
- Deshacer cambios realizados. (git checkout .)
- Confirmar cambios. (git commit)
- Corregir el nombre de un commit. (git amend)
- Quitar archivos del área de preparación. (git reset)
- Ver cambios realizados en cada archivo. (git diff filename)
- Ver el historial de proyecto. (git log)
- Generar tu llave pública. (SSH)
- Subir los archivos a un repositorio remoto. (GitHub) (git push)
- Clonar un repositorio. (git clone) (HTTPS/SSH)
- Versionar un repositorio existente. (git remote add)
- Ejercicios



### Sesión 2: 

```
git branch, git tag, git merge,  git rebase, git alias, 
git log --oneline --graph, git log --oneline --branches
```

- ¿Qué es una rama? (git branch)
- Crear ramas locales y remotas. (git branch, git checkout -b)
- Mover entre ramas y versiones. (git checkout hash)
- Descargar una rama remota. (git fetch)
- Borrar rama. (git branch -d/ git branch -D)
- Combinar ramas. (git merge)
- Forzar la actualización de una rama remota.(git push origin +branchname)
- Resolver conflictos.
- Renombrar rama. (git branch -m branche_name new_branche_name)
- Ignorar archivos. (git .gitignore)
- Etiquetas y versiones “banderas”. (git tag)
- Eliminar Etiquetas.
- Subir todas las Etiquetas al servidor remoto (git push --tags)
- Reescribir la historia del proyecto. (git rebase)  <= Investigar que no recuerdo
- Juntar commits (git rebase -i) <= ok esta si me la se 
- Examen




### Sesión 3: 
```
git stash, git clean, git reset, git revert, 
git cherry-pick, git log grep
```

- Guardar cambios temporales. (git stash)
- Guardar nuestro cambio temporal con un nombre. (git stash save)
- Eliminar los cambios temporales guardados. (git stash drop)
- Eliminar todos los cambios temporales guardados. (git stash clear)
- Limpiar el proyecto de archivos no deseados. (git clean)
- ¿Cómo revertir un cambio? (git reset soft,mixed,hard, revert )
- Traer un commit específico de una rama. (git cherry-pick)
- Git log (git log --author=”juan”, git grep )
- Examen

### Sesión 4:
```
git rm --cached, fileMode, git submodule, git bisect, git bare, git reflog,
```
- Eliminar archivos del repo que están versionados a pesar que se han ignorado. ( rm --cached)
- Ignorar cambios de los permisos de archivos. (fileMode)
- Git dentro de Git. (git submodule)
- Encontrar errores. (git bisect)
-  Por investigar (git bare)
- Encontrar commits borrados. (git reflog)
- Migración de un repositorio a otro.
- Examen




