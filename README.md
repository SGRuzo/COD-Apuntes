# 📌 Git & GitHub: Guía Completa 🚀  

## 📖 Tabla de Contenidos  
1. [📥 Clonar un repositorio (`clone`)](#-clonar-un-repositorio-clone)  
2. [🍴 Hacer un fork (`fork`)](#-hacer-un-fork-fork)  
3. [✅ Realizar un commit (`commit`)](#-realizar-un-commit-commit)  
4. [🗑️ Borrar un commit (`commit`)](#-borrar-un-commit-commit)
5. [🌿 Trabajar con ramas (`branches`)](#-trabajar-con-ramas-branches)
6. [🎭 Main vs Master (`main/master`)](#-main-vs-master-mainmaster)  
7. [📩 Pull Request (`PR`)](#-pull-request-pr)  
8. [🔀 Merge (`merge`)](#-merge-merge)  
9. [🔄 Merge Squash (`merge squash`)](#-merge-squash-merge-squash)  
10. [⬇️ Actualizar cambios (`pull`)](#-actualizar-cambios-pull)  
11. [⬆️ Subir cambios (`push`)](#-subir-cambios-push)  
12. [🤝 Colaboradores (`collaborator`)](#-colaboradores-collaborator)  
13. [🐞 Issues (`issues`)](#-issues-issues)  
14. [🔨 Squash (`squash`)](#-squash-squash)  
15. [📄 Añadir un archivo `.gitignore`](#-añadir-un-archivo-gitignore)  
16. [🏷️ Crear un Release (`v1.0`)](#-crear-un-release-v10)  

---

## 📥 Clonar un repositorio (`clone`)  

Clonar un repositorio significa descargar una copia exacta del código fuente en tu máquina local.  

### 🔹 Pasos en **IntelliJ**  
1. Abre IntelliJ IDEA.  
2. Ve a **File > New > Project from Version Control**.  
3. Pega la URL del repositorio en el campo correspondiente.  
4. Selecciona la carpeta donde quieres guardarlo y haz clic en **Clone**.  

### 🔹 Pasos en **GitHub**  
1. Ve al repositorio que deseas clonar.  
2. Haz clic en el botón **Code** y copia la URL.  

### 🔹 Pasos en **Consola**  
```bash
git clone https://github.com/usuario/repositorio.git
```


## 🍴 Hacer un fork (`fork`)  

Un **fork** es una copia de un repositorio en tu cuenta de GitHub. Sirve para modificar el código sin afectar el original.  

### 🔹 Pasos en **GitHub**  
1. Ve al repositorio que quieres forkar.  
2. Haz clic en el botón **Fork** (arriba a la derecha).  
3. Ahora tienes una copia en tu cuenta.  


## ✅ Realizar un commit (`commit`)  

Un **commit** es un guardado de cambios en el historial del proyecto.  

### 🔹 Pasos en **IntelliJ**  
1. Ve a **Git > Commit**.  
2. Escribe un mensaje claro sobre los cambios realizados.  
3. Haz clic en **Commit** o en **Commit & Push**.  

### 🔹 Pasos en **Consola**  
```bash
git add .
git commit -m "Mensaje descriptivo del cambio"
```
Aquí tienes la guía actualizada con los nuevos temas añadidos. Puedes usarla como `README.md` en tu repositorio de GitHub o como referencia personal.  

---

## 🗑️ Borrar un commit (`commit`) 

### 🔹 En IntelliJ IDEA  
- **Revisar el historial de commits:** Ve a **Git > Show History**.  
- **Deshacer un commit:** Haz clic derecho sobre el commit y selecciona **"Undo Commit"**.  
- **Eliminar commits permanentemente:** Ve a **Git > Reset HEAD** y selecciona **Hard**.  

### 🔹 Comandos de Git  
```bash
# Deshacer el último commit (manteniendo los cambios en el área de trabajo)
git reset --soft HEAD~1

# Eliminar el último commit y los cambios asociados
git reset --hard HEAD~1
```

---

## 🌿 Trabajar con ramas (`branches`)  

Las **ramas** permiten desarrollar nuevas características sin afectar el código principal.  

### 🔹 Crear una rama en **IntelliJ**  
1. Ve a **Git > Branches > New Branch**.  
2. Escribe un nombre para la nueva rama y crea la rama.  

### 🔹 Crear una rama en **Consola**  
```bash
git branch nombre-de-la-rama
git checkout nombre-de-la-rama  # Cambiar a la nueva rama
```


## 🎭 Main vs Master (`main/master`)  

- **`main`**: La rama principal por defecto en repositorios nuevos.  
- **`master`**: Era la rama principal en versiones antiguas de Git.  

Para cambiar la rama en consola:  
```bash
git checkout main
```


## 📩 Pull Request (`PR`)  

Un **Pull Request (PR)** es una solicitud para fusionar cambios en otro repositorio.  

### 🔹 Pasos en **GitHub**  
1. Ve a tu repositorio y selecciona la rama que modificaste.  
2. Haz clic en **New Pull Request**.  
3. Agrega una descripción y envíalo.  


## 🔀 Merge (`merge`)  

El **merge** combina los cambios de una rama con otra.  

### 🔹 Pasos en **IntelliJ**  
1. Ve a **Git > Branches**.  
2. Selecciona la rama donde quieres hacer el merge.  
3. Haz clic en **Merge into Current**.  

### 🔹 Pasos en **Consola**  
```bash
git checkout main
git merge nombre-de-la-rama
```


## 🔄 Merge Squash (`merge squash`)  

El **merge squash** combina varios commits en uno solo antes de fusionarlos.  

### 🔹 Pasos en **Consola**  
```bash
git checkout main
git merge --squash nombre-de-la-rama
git commit -m "Un solo commit con todos los cambios"
```


## ⬇️ Actualizar cambios (`pull`)  

El **pull** trae los cambios del repositorio remoto al local.  

### 🔹 Pasos en **Consola**  
```bash
git pull origin main
```


## ⬆️ Subir cambios (`push`)  

El **push** envía los cambios locales al repositorio remoto.  

### 🔹 Pasos en **Consola**  
```bash
git push origin nombre-de-la-rama
```


## 🤝 Colaboradores (`collaborator`)  

Los **colaboradores** son usuarios con permiso para modificar un repositorio.  

### 🔹 Pasos en **GitHub**  
1. Ve a **Settings > Collaborators**.  
2. Añade el nombre de usuario de GitHub.  
3. Envía la invitación.  


## 🐞 Issues (`issues`)  

Las **issues** sirven para reportar problemas o sugerir mejoras.  

### 🔹 Pasos en **GitHub**  
1. Ve a la pestaña **Issues** en el repositorio.  
2. Haz clic en **New Issue**.  
3. Describe el problema y publícalo.  



## 🔨 Squash (`squash`)  

El **squash** combina múltiples commits en uno solo.  

### 🔹 Pasos en **Consola**  
1. Usa `git log` para ver los commits.  
2. Ejecuta:  
```bash
git rebase -i HEAD~3  # Para combinar los últimos 3 commits
```
3. Cambia `pick` por `squash` en los commits que deseas fusionar.  
4. Guarda y cierra.  

---

## 📄 Añadir un archivo `.gitignore`  

Un archivo `.gitignore` especifica qué archivos deben ser ignorados por Git.  

### 🔹 En IntelliJ IDEA  
1. Haz clic derecho en la raíz del proyecto y selecciona **New > File**.  
2. Nombra el archivo como `.gitignore`.  
3. Agrega reglas, por ejemplo:  
```plaintext
# Ignorar archivos de compilación
/target/
/build/

# Ignorar archivos de configuración local
*.iml
.idea/
```
4. Agrégalo al repositorio: **Git > Add**.  

### 🔹 Comandos de Git  
```bash
touch .gitignore
git add .gitignore
git commit -m "Añadir archivo .gitignore"
```

---

## 🏷️ Crear un Release (`v1.0`)  

Un **release** permite marcar una versión estable del código.  

### 🔹 En IntelliJ IDEA  
1. Ve a **Git > Tag**.  
2. Asigna un nombre como `v1.0` y añade una descripción.  
3. Para subir el tag, ve a **Git > Push** y selecciónalo.  

### 🔹 En GitHub  
1. Ve a tu repositorio y haz clic en **Releases > Draft a new release**.  
2. Selecciona el tag `v1.0` y añade una descripción.  

### 🔹 Comandos de Git  
```bash
# Crear un tag
git tag -a v1.0 -m "Release v1.0"

# Subir el tag a GitHub
git push origin v1.0
```

---
