## Primera vez que subes un proyecto a GitHub

```bash
# Inicializa Git en la carpeta
git init

# Añade el remoto (cambia la URL por la de tu repo en GitHub)
git remote add origin git@github.com:TU_USUARIO/TU_REPO.git

# Renombra la rama actual a main (lo estándar en GitHub)
git branch -M main

# Añade todos los archivos al stage
git add .

# Crea el primer commit
git commit -m "Primer commit"

# Sube todo a GitHub
git push -u origin main
```

---

## Flujo normal de trabajo (cuando ya tienes el repo configurado)

```bash
# Traer los últimos cambios del remoto
git pull origin main --allow-unrelated-histories

# Añadir cambios locales
git add .

# Hacer commit
git commit -m "Descripción de lo que cambiaste"

# Subir cambios
git push origin main
```

---

## Si hay conflictos ⚠️

1. Edita los archivos con conflicto.
    
2. Una vez resueltos:
    
    ```bash
    git add .
    git commit -m "Conflictos resueltos"
    git push origin main
    ```
    

---

## Atajos útiles

- Ver estado de tu repo:
    
    ```bash
    git status
    ```
    
- Ver historial de commits:
    
    ```bash
    git log --oneline
    ```
    

---
