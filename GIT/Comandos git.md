Ordenes para copiar y pegar directamente en la terminal [[Atajos]]
# Guía Definitiva de Git y GitHub

Esta guía es una "chuleta" completa para todas las operaciones comunes y algunas avanzadas que realizamos con Git para interactuar con GitHub. Ideal para recordar comandos rápidamente.

-----

## Configuración Inicial de Git

Antes de empezar, asegúrate de que Git está configurado correctamente en tu máquina.

```bash
# Configurar tu nombre de usuario (aparecerá en tus commits)
git config --global user.name "Tu Nombre Completo"

# Configurar tu correo electrónico (asociado a tu cuenta de GitHub)
git config --global user.email "tu_email@example.com"

# Configurar el editor de texto predeterminado para Git (ej. VS Code)
git config --global core.editor "code --wait" # Para VS Code
# git config --global core.editor "vim" # Para Vim
# git config --global core.editor "nano" # Para Nano

# Ver la configuración actual
git config --list
```

-----

## Clonar Repositorios (Cloning)

Trae un repositorio existente de GitHub a tu máquina local.

```bash
# Clonar un repositorio usando HTTPS (el más común)
git clone https://github.com/usuario/nombre-del-repositorio.git

# Clonar un repositorio usando SSH (si ya tienes configurada tu clave SSH)
git clone git@github.com:usuario/nombre-del-repositorio.git

# Clonar un repositorio en un directorio específico
git clone https://github.com/usuario/nombre-del-repositorio.git mi-proyecto-local
```

-----

## Flujo de Trabajo Básico: Add, Commit, Push

Este es el ciclo de vida fundamental para subir tus cambios.

### 1\. **`git status`**: Revisa el Estado

Verifica qué archivos han cambiado, cuáles están preparados para el commit y cuáles no.

```bash
git status
```

### 2\. **`git add`**: Prepara los Cambios

Mueve los cambios del directorio de trabajo al "staging area" (área de preparación).

```bash
# Añadir un archivo específico
git add nombre-del-archivo.js

# Añadir todos los archivos modificados y nuevos en el directorio actual y subdirectorios
git add .

# Añadir todos los archivos modificados y eliminados (pero no nuevos)
git add -u

# Añadir todos los cambios (modificados, nuevos, eliminados)
git add -A # Equivalente a git add . y git add -u juntos
```

### 3\. **`git commit`**: Guarda los Cambios Localmente

Crea un "snapshot" de tus cambios en el historial de Git.

```bash
# Commit con un mensaje corto y descriptivo
git commit -m "feat: Añadir nueva funcionalidad de login"

# Commit con un mensaje más largo (abre el editor de texto)
git commit

# Commit saltándose el staging area (solo para archivos ya trackeados)
git commit -am "fix: Corregir error de validación en formulario"
```

**Reglas para Mensajes de Commit (Clean Code):**

  * **Tipo:** `feat` (nueva funcionalidad), `fix` (corrección de error), `docs` (documentación), `style` (formato, sin cambios de código), `refactor` (refactorización sin cambio de comportamiento), `test` (añadir tests), `chore` (cambios de build, herramientas, etc.).
  * **Alcance (opcional):** `(auth)`, `(ui)`, `(database)`.
  * **Asunto:** Corto, en imperativo, minúscula, no termina con punto.

Ejemplo: `feat(api): Implementar endpoint para usuarios`

### 4\. **`git push`**: Sube los Cambios a GitHub

Envía tus commits locales al repositorio remoto en GitHub.

```bash
# Sube tus cambios a la rama actual en el repositorio remoto "origin"
git push origin nombre-de-tu-rama

# La primera vez que haces push de una nueva rama, establece el upstream
git push -u origin nombre-de-tu-rama

# Push simple (si ya tienes el upstream configurado)
git push
```

-----

## Gestión de Ramas (Branching)

Las ramas son esenciales para trabajar en nuevas funcionalidades o correcciones sin afectar la línea principal de desarrollo (`main` o `master`).

### Crear y Cambiar de Rama

```bash
# Crear una nueva rama basada en la rama actual
git branch nombre-de-la-rama

# Cambiar a una rama existente
git checkout nombre-de-la-rama

# Crear una nueva rama y cambiar a ella inmediatamente (¡el más usado!)
git checkout -b nombre-de-la-rama

# Cambiar a la rama anterior
git checkout -
```

### Listar Ramas

```bash
# Listar todas las ramas locales
git branch

# Listar todas las ramas (locales y remotas)
git branch -a

# Listar solo ramas remotas
git branch -r
```

### Publicar una Rama Nueva

```bash
# Sube la rama local al repositorio remoto (creándola si no existe)
git push -u origin nombre-de-la-rama
```

### Eliminar Ramas

```bash
# Eliminar una rama local (solo si ya está fusionada o pushada)
git branch -d nombre-de-la-rama

# Eliminar una rama local (forzado, aunque no esté fusionada)
git branch -D nombre-de-la-rama

# Eliminar una rama remota (en GitHub)
git push origin --delete nombre-de-la-rama
# O su forma abreviada
git push origin :nombre-de-la-rama
```

-----

## Fusionar Ramas (Merging)

Integra los cambios de una rama en otra.

```bash
# Primero, asegúrate de estar en la rama que recibirá los cambios (ej. main)
git checkout main

# Luego, fusiona la rama de características en la rama actual
git merge nombre-de-la-rama-a-fusionar

# Si hay conflictos de fusión, resuelve manualmente los archivos conflictivos y luego:
git add .
git commit -m "Merge branch 'nombre-de-la-rama-a-fusionar'"

# Abortar una fusión si te arrepientes antes de commitear
git merge --abort
```

-----

## Traer Cambios Remotos (Pulling & Fetching)

Mantén tu repositorio local actualizado con los cambios de GitHub.

### `git fetch`

Descarga los objetos y referencias de ramas del repositorio remoto, pero **no los integra** en tus ramas locales de trabajo. Es útil para ver qué cambios hay sin aplicarlos inmediatamente.

```bash
git fetch origin
```

### `git pull`

Es un atajo para `git fetch` seguido de `git merge`. Descarga los cambios y los fusiona automáticamente en tu rama actual.

```bash
# Trae y fusiona los cambios de la rama remota configurada como upstream
git pull

# Trae y fusiona los cambios de una rama específica del repositorio remoto
git pull origin nombre-de-la-rama-remota
```

-----

## Deshacer Cambios

A veces necesitamos volver atrás. ¡Cuidado con estos comandos\!

### `git restore` (o `git checkout`)

Deshace cambios en el directorio de trabajo o en el staging area.

```bash
# Descartar cambios en un archivo no staged
git restore nombre-del-archivo.js

# Deshacer cambios de un archivo que ya está en el staging area
git restore --staged nombre-del-archivo.js

# Volver un archivo a su estado en el último commit (en el directorio de trabajo y staging area)
git restore --source=HEAD nombre-del-archivo.js
```

**Nota:** `git checkout` también se usaba para esto, pero `git restore` es más claro y está diseñado específicamente para deshacer cambios.

### `git reset`

Deshace commits locales, pero puede ser peligroso si los commits ya se han subido.

```bash
# Deshacer el último commit, manteniendo los cambios en el staging area
git reset --soft HEAD~1

# Deshacer el último commit, moviendo los cambios al directorio de trabajo (no staged)
git reset --mixed HEAD~1 # Este es el predeterminado si no especificas nada

# Deshacer el último commit y descartar todos los cambios (¡PELIGROSO!)
git reset --hard HEAD~1

# Deshacer un commit específico (y todos los subsiguientes) a un commit determinado
git reset --hard <hash-del-commit>

# Deshacer un archivo específico a su estado en un commit anterior
git reset <hash-del-commit> nombre-del-archivo.js
git checkout -- nombre-del-archivo.js # para quitarlo del staging area
```

### `git revert`

Crea un nuevo commit que deshace los cambios de un commit anterior. **Es la forma segura de deshacer cambios en commits que ya se han subido**, ya que no reescribe el historial.

```bash
# Revierte el último commit
git revert HEAD

# Revierte un commit específico (abre el editor para el mensaje del commit de revert)
git revert <hash-del-commit>

# Revierte un commit específico sin abrir el editor
git revert -m "Revert: Deshaciendo el commit <hash>" <hash-del-commit>
```

-----

## Etiquetas (Tags)

Los tags se usan para marcar puntos específicos en el historial (como versiones de lanzamiento).

```bash
# Crear un tag ligero (solo un puntero)
git tag v1.0.0

# Crear un tag anotado (recomendado, incluye mensaje, autor, fecha)
git tag -a v1.0.0 -m "Versión de lanzamiento 1.0.0"

# Listar tags
git tag

# Subir tags al repositorio remoto
git push origin --tags

# Eliminar un tag local
git tag -d v1.0.0

# Eliminar un tag remoto
git push origin --delete v1.0.0
```

-----

## stash Guardar Cambios Temporalmente (Stashing)

Si necesitas cambiar de rama pero tienes cambios sin commitear que no quieres perder, `git stash` es tu amigo.

```bash
# Guardar los cambios actuales (trackeados y no trackeados)
git stash save "Mensaje opcional para el stash"
# O la forma abreviada y común
git stash

# Ver la lista de stashes guardados
git stash list

# Aplicar el stash más reciente y mantenerlo en la lista
git stash apply

# Aplicar el stash más reciente y eliminarlo de la lista (¡el más común!)
git stash pop

# Aplicar un stash específico por su índice (ej. stash@{1})
git stash apply stash@{1}

# Eliminar un stash específico
git stash drop stash@{1}

# Eliminar todos los stashes
git stash clear
```

-----

## Reorganizar Commits (Rebase)

Reescribe el historial de commits. Útil para mantener un historial de proyecto limpio y lineal. **¡Úsalo con precaución, especialmente en ramas compartidas\!**

```bash
# Rebase interactivo (para modificar, reordenar, combinar commits)
# HEAD~3 significa los últimos 3 commits
git rebase -i HEAD~3

# Rebase de tu rama actual sobre otra rama (ej. main)
# Esto aplica tus commits sobre los commits más recientes de 'main'
git rebase main

# Continuar un rebase después de resolver conflictos
git rebase --continue

# Abortar un rebase
git rebase --abort
```

**Cuándo usar Rebase vs. Merge:**

  * **Rebase:** Para mantener un historial lineal y limpio, especialmente en tus propias ramas de trabajo antes de fusionar en una rama principal. **No lo uses en ramas que ya han sido publicadas y compartidas**, ya que reescribe el historial.
  * **Merge:** Mantiene el historial de commits tal cual, mostrando la fusión explícitamente. Es la opción más segura para ramas compartidas y para el `main`.

-----

## Eliminar Repositorios Remotos

Esto se hace directamente en GitHub.

1.  Ve al repositorio en GitHub.
2.  Haz clic en **Settings**.
3.  Desplázate hasta la parte inferior y haz clic en **Delete this repository**.
4.  Confirma ingresando el nombre del repositorio.

**Nota:** Esto solo elimina el repositorio remoto. La copia local en tu máquina permanece a menos que la elimines manualmente:

```bash
# En tu terminal
rm -rf nombre-del-repositorio-local
```

-----

## Otros Comandos Útiles

```bash
# Ver el historial de commits
git log

# Ver el historial de commits de forma concisa y gráfica
git log --oneline --graph --all

# Ver los cambios entre el último commit y el directorio de trabajo/staging area
git diff

# Ver los cambios entre el staging area y el último commit
git diff --staged # o git diff --cached

# Ver los cambios entre dos commits
git diff <commit1> <commit2>

# Renombrar la rama actual
git branch -m nuevo-nombre-de-la-rama

# Eliminar archivos no trackeados o directorios
git clean -n # Simula la limpieza (Dry run)
git clean -f # Limpia archivos no trackeados (¡Cuidado!)
git clean -df # Limpia archivos y directorios no trackeados (¡Cuidado!)
```

-----
