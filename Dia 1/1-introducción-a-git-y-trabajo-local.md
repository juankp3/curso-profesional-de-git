# Día 1: Introducción a Git y Trabajo Local 

## 1. Introducción a Git y Configuración (30 minutos)
### ¿Qué es Git?
Git es un sistema de control de versiones distribuido (DVCS, por sus siglas en inglés) diseñado para gestionar el seguimiento de cambios en el código fuente durante el desarrollo de software. Fue creado por Linus Torvalds en 2005 y se ha convertido en una herramienta fundamental en el desarrollo de software colaborativo.

#### Características clave de Git:

1. **Distribuido:**
   - Cada desarrollador tiene una copia completa del historial de cambios del proyecto, lo que permite trabajar de forma independiente y sin conexión a internet.

2. **Historial de cambios:**
   - Git mantiene un registro detallado de cada cambio realizado en el código, lo que facilita la revisión del historial y la identificación de quién realizó cada modificación.

3. **Ramificación y fusión:**
   - Permite la creación de ramas independientes para el desarrollo de nuevas funciones o corrección de errores. Posteriormente, estas ramas se pueden fusionar de nuevo en la rama principal.

4. **Eficiencia:**
   - Git es eficiente en términos de almacenamiento, ya que utiliza técnicas como la compresión y el almacenamiento de cambios en lugar de archivos completos.

5. **Velocidad:**
   - Las operaciones en Git, como la creación de ramas y la fusión, son generalmente rápidas debido a su diseño eficiente.

6. **Colaboración:**
   - Facilita la colaboración entre desarrolladores, ya que pueden trabajar en diferentes partes del código simultáneamente y luego combinar sus cambios de manera controlada.

7. **Integridad de datos:**
   - Utiliza un sistema de suma de comprobación criptográfica (hash) para asegurar la integridad de los datos almacenados.

8. **Compatibilidad con plataformas:**
   - Git es compatible con múltiples plataformas, incluyendo Windows, macOS y Linux.

### Conceptos fundamentales de Git:

1. **Repositorio:**
   - Es un espacio de almacenamiento de datos de Git que contiene el historial completo de cambios y metadatos del proyecto.

2. **Commit:**
   - Un commit es un conjunto de cambios realizados en el código que se ha registrado en el historial del repositorio.

3. **Rama:**
   - Una rama es una línea independiente de desarrollo. Se utilizan para trabajar en características aisladas sin afectar la rama principal.

4. **Clonación:**
   - Es la acción de copiar un repositorio Git existente para trabajar con él de forma local.

5. **Fusión (Merge) y Rebase:**
   - Operaciones para combinar cambios realizados en diferentes ramas.

Git se ha convertido en una herramienta esencial en el desarrollo de software debido a su flexibilidad, eficiencia y capacidad para gestionar proyectos de diferentes tamaños y complejidades.

### Instalación de Git.
La instalación de Git puede realizarse en diferentes sistemas operativos. A continuación, te proporcionaré instrucciones básicas para la instalación en sistemas Windows, macOS y distribuciones de Linux basadas en Debian (como Ubuntu). Ten en cuenta que los procedimientos pueden cambiar con el tiempo, así que es recomendable verificar la documentación oficial para obtener la información más reciente.

### Configuración de nombre de usuario y correo electrónico.
Configurar el nombre de usuario y la dirección de correo electrónico en Git es una parte esencial del proceso de configuración inicial. Estos detalles se utilizan para identificar al autor de los commits. Aquí tienes los comandos para configurar esta información:

### Configuración Global:

Estos comandos establecen la configuración a nivel global, lo que significa que se aplicarán a todos los repositorios Git en tu sistema.

#### 1. Configurar el Nombre de Usuario:
```bash
git config --global user.name "Tu Nombre"
```

#### 2. Configurar la Dirección de Correo Electrónico:
```bash
git config --global user.email "tu@email.com"
```

### Verificar la Configuración:

Puedes verificar que la configuración se ha realizado correctamente utilizando el siguiente comando:

```bash
git config --global --get user.name
git config --global --get user.email
```

Estos comandos deberían mostrar tu nombre y dirección de correo electrónico, respectivamente.

### Configuración Específica del Repositorio:

Si deseas configurar el nombre de usuario y la dirección de correo electrónico solo para un repositorio específico, puedes omitir la opción `--global` y ejecutar los comandos en el directorio del repositorio.

```bash
cd /ruta/del/repositorio
git config user.name "Tu Nombre"
git config user.email "tu@email.com"
```

### Notas Importantes:

- La dirección de correo electrónico que configuras en Git generalmente debe coincidir con la que utilizas en servicios de alojamiento remoto como GitHub o GitLab para que los commits se asocien correctamente con tu cuenta.
  
- Puedes verificar la configuración actual en un repositorio específico abriendo el archivo `.git/config` en el directorio del repositorio.

Establecer correctamente el nombre de usuario y la dirección de correo electrónico es fundamental para mantener una trazabilidad clara de los cambios en el historial de Git.




## 2. Creación y Clonación de Repositorios (30 minutos)


#### 1. Introducción a Git y Configuración (30 minutos)
   - ¿Qué es Git?
   - Instalación de Git.
   - Configuración de nombre de usuario y correo electrónico.

#### 2. Creación y Clonación de Repositorios (30 minutos)
   - `git init`: Inicialización de un nuevo repositorio.
   - `git clone`: Clonación de un repositorio existente.
   - Ejemplos prácticos.

#### 3. Commits y Historial (30 minutos)
   - `git add`: Agregar cambios al área de preparación.
   - `git commit`: Creación de commits.
   - `git log`: Revisión del historial.
   - Ejemplos prácticos.

#### 4. Ramificación Básica (30 minutos)
   - `git branch`: Creación y gestión de branches.
   - `git checkout`: Cambio entre branches.
   - Ejemplos prácticos.

----
#### 1. Introducción a Git y Configuración (30 minutos)
¿Que es el working directory?
Es la área donde podemos hacer cualquier cambio que se desee sin afectar nuestro repositorio en lo absoluto.

Nota : 
Cuando pasas el código de Working Directory a Staging Area, cambias el estado del
código de modificado a preparado.

¿Que es el staging area?
Es el área donde guardamos temporalmente nuestros archivos antes de hacerlos definitivos y registrarlos en el repositorio.

Nota : 
Nota que cuando haces el commit el código pasa de estado preparado a confirmado.

¿Que es el repository?
Es el área donde finalmente se guardan los cambios confirmados desde la zona temporal de intercambio. 



# Comandos Básicos de GIT

## git config

`git config` es un comando que define valores de configuración de Git a nivel de un proyecto global o local

```
git config --global user.name "Juan Kuga”
git config --global user.email juankp3@gmail.com
```

## git init
`git init` es un comando que se utiliza una sola vez durante la configuración inicial de un repositorio nuevo. Al ejecutar este comando, se crea un directorio `.git/` en tu directorio de trabajo actual. 

```
git init
```

## git remote
`git remote` muestra el nombre del repositorio remoto al que estamos conectado.

```
git remote
git remote -v
```
## git add
`git add` añade un cambio del directorio de trabajo en el entorno de ensayo. De este modo, indica a Git que quieres incluir actualizaciones en un archivo concreto en la próxima confirmación.
```
git add .
git add --all
```
## git commit
`git commit` captura una instantánea de los cambios preparados en ese momento del proyecto. Las instantáneas confirmadas pueden considerarse como versiones "seguras" de un proyecto: Git no las cambiará nunca a no ser que se lo pidas expresamente.

```
git commit -m "mensaje de confirmación de los cambios realizados"
```

## git push
El comando git push se usa para cargar contenido del repositorio local a un repositorio remoto. El envío es la forma de transferir confirmaciones desde tu repositorio local a un repositorio remoto.

```
git push origin <branch-name>
```

## git pull
El comando git pull se emplea para extraer y descargar contenido desde un repositorio remoto y actualizar al instante el repositorio local para reflejar ese contenido. La fusión de cambios remotos de nivel superior en tu repositorio local es una tarea habitual de los flujos de trabajo de colaboración basados en Git.

```
git pull origin <branch-name>
```

## git branch
El comando git branch te permite crear, enumerar y eliminar ramas, así como cambiar su nombre. No te permite cambiar entre ramas o volver a unir un historial bifurcado. Por este motivo, git branch está estrechamente integrado con los comandos git checkout y git merge .

```
git branch <branch-name>
```

Elimina una rama sin cambios nuevos. (Rama ya fusionada)
```
git branch -d <branch-name>
```

Elimina una rama de forma definitiva con o sin cambios nuevos
```
git branch -D <branch-name>
```

## git checkout
El comando git checkout te permite desplazarte entre las ramas creadas por git branch . Al extraer una rama, se actualizan los archivos en el directorio de trabajo para reflejar la versión almacenada en esa rama y se indica a Git que registre todas las confirmaciones nuevas en dicha rama.
```
git checkout <branch-name>
```

## git merge
El comando git merge permite tomar las líneas independientes de desarrollo creadas por git branch e integrarlas en una sola rama. Ten en cuenta que todos los comandos presentados a continuación se fusionan en la rama actual

```
git merge <branch-name>
```

## git log
El comando git log es una herramienta básica de Git para explorar el historial del repositorio. Este comando se usa cuando necesitas buscar una versión concreta de un proyecto o saber los cambios que se introducirán mediante la fusión en una rama de función.

```
git log <branch-name>
```

## git ignore
gitignore , es un archivo de texto que le dice a Git qué archivos o carpetas ignorar en un proyecto. Un archivo local . gitignore generalmente se coloca en el directorio raíz de un proyecto. También puedes crear un archivo global

```
.gitignore
```

## git clone
git clone es una utilidad de línea de comandos de Git que se utiliza para fijar como objetivo un repositorio existente con el fin de clonarlo o copiarlo.

```
git clone
```
