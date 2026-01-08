
# Instrucciones para subir a GitHub

Sigue estos pasos para subir este proyecto a tu repositorio de GitHub.

## 1. Preparación del Repositorio Local

Abre la terminal en la carpeta del proyecto (`c:\xampp\htdocs\html\og-type`) y ejecuta los siguientes comandos:

```bash
# Inicializar el repositorio
git init

# Configurar tu identidad (para este repositorio)
git config user.name "Alejandro Figuera"
git config user.email "github@alejandrofiguera.link"

# Agregar archivos al área de preparación
git add .

# Crear el primer commit
git commit -m "Initial commit: Open Graph Examples collection"

# Renombrar la rama principal a 'main'
git branch -M main
```

## 2. Conectar con GitHub

Asegúrate de haber creado un **repositorio vacío** en GitHub (sin README, ni .gitignore) con el nombre deseado (por ejemplo, `og-type-examples`).

Luego, vincula tu repositorio local con el remoto:

```bash
# Reemplaza 'og-type-examples' con el nombre de tu repositorio real si es diferente
git remote add origin https://github.com/alejandro-figuera/og-type-examples.git

# Subir los cambios
git push -u origin main
```

---
**Nota**: Si el repositorio remoto ya tiene archivos (como un README creado al inicio), podrías necesitar hacer un `git pull origin main --allow-unrelated-histories` antes del push, pero es mejor empezar con un repo vacío en GitHub.
