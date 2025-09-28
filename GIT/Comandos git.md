Guía Definitiva de Git y GitHub

Esta guía es una chuleta completa para todas las operaciones comunes y algunas avanzadas que realizamos con Git para interactuar con GitHub. Ideal para recordar comandos rápidamente.

---

Configuración Inicial de Git

Antes de empezar, asegúrate de que Git está configurado correctamente en tu máquina.

```
git config --global user.name "Tu Nombre Completo"
git config --global user.email "tu_email@example.com"
git config --global core.editor "code --wait"
git config --list
```

---

Clonar Repositorios

```
git clone https://github.com/usuario/nombre-del-repositorio.git
git clone git@github.com:usuario/nombre-del-repositorio.git
git clone https://github.com/usuario/nombre-del-repositorio.git mi-proyecto-local
```

---

Flujo de Trabajo Básico: Add, Commit, Push

1. git status
    

```
git status
```

2. git add
    

```
git add nombre-del-archivo.js
git add .
git add -u
git add -A
```

3. git commit
    

```
git commit -m "feat: Añadir nueva funcionalidad de login"
git commit
git commit -am "fix: Corregir error de validación en formulario"
```

Reglas de commits:

- Tipo: feat, fix, docs, style, refactor, test, chore
    
- Alcance (opcional): (auth), (ui), (database)
    
- Asunto: corto, imperativo, sin punto final
    

Ejemplo: feat(api): Implementar endpoint para usuarios

4. git push
    

```
git push origin nombre-de-tu-rama
git push -u origin nombre-de-tu-rama
git push
```

---

Gestión de Ramas

Crear y cambiar ramas:

```
git branch nombre-de-la-rama
git checkout nombre-de-la-rama
git checkout -b nombre-de-la-rama
git checkout -
```

Listar ramas:

```
git branch
git branch -a
git branch -r
```

Publicar ramas:

```
git push -u origin nombre-de-la-rama
```

Eliminar ramas:

```
git branch -d nombre-de-la-rama
git branch -D nombre-de-la-rama
git push origin --delete nombre-de-la-rama
git push origin :nombre-de-la-rama
```

---

Fusionar Ramas

```
git checkout main
git merge nombre-de-la-rama-a-fusionar
git add .
git commit -m "Merge branch 'nombre-de-la-rama-a-fusionar'"
git merge --abort
```

---

Traer Cambios Remotos

```
git fetch origin
git pull
git pull origin nombre-de-la-rama-remota
```

---

Deshacer Cambios

git restore:

```
git restore nombre-del-archivo.js
git restore --staged nombre-del-archivo.js
git restore --source=HEAD nombre-del-archivo.js
```

git reset:

```
git reset --soft HEAD~1
git reset --mixed HEAD~1
git reset --hard HEAD~1
git reset --hard <hash>
git reset <hash> nombre-del-archivo.js
```

git revert:

```
git revert HEAD
git revert <hash>
git revert -m "Revert: Deshaciendo el commit <hash>" <hash>
```

---

Etiquetas

```
git tag v1.0.0
git tag -a v1.0.0 -m "Versión 1.0.0"
git tag
git push origin --tags
git tag -d v1.0.0
git push origin --delete v1.0.0
```

---

Stash (Guardar cambios temporalmente)

```
git stash save "mensaje"
git stash
git stash list
git stash apply
git stash pop
git stash apply stash@{1}
git stash drop stash@{1}
git stash clear
```

---

Rebase

```
git rebase -i HEAD~3
git rebase main
git rebase --continue
git rebase --abort
```

Rebase se usa para mantener historial lineal en ramas personales.  
Merge se usa en ramas compartidas para no reescribir historial.

---

Eliminar Repositorios

En GitHub: Settings > Delete this repository  
En local:

```
rm -rf nombre-del-repositorio-local
```

---

Otros Comandos Útiles

```
git log
git log --oneline --graph --all
git diff
git diff --staged
git diff <commit1> <commit2>
git branch -m nuevo-nombre
git clean -n
git clean -f
git clean -df
```

---

Buenas Prácticas

- Commits pequeños y con un único propósito.
    
- Mensajes claros con convención tipo(alcance): asunto.
    
- Mantener main estable y desplegable.
    
- Trabajar en ramas separadas.
    
- Hacer git pull frecuentemente.
    
- Usar git status y git diff antes de commitear.
    
- Evitar git push --force en ramas compartidas.
    

---
