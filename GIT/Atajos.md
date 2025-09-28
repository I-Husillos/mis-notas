Primera vez que subes un repo

```bash
git init
git remote add origin git@github.com:TU_USUARIO/TU_REPO.git
git branch -M main
git add .
git commit -m "Primer commit"
git push -u origin main
```

---

### Flujo normal (ya configurado)

```bash
git pull origin main --allow-unrelated-histories
git add .
git commit -m "Actualización"
git push origin main
```

---

### Resolver conflictos

```bash
git add .
git commit -m "Conflictos resueltos"
git push origin main
```

---
