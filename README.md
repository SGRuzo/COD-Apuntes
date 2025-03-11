# 📌 Git & GitHub: Guía Completa 🚀  

Bienvenido/a a esta guía sobre Git y GitHub. Aquí encontrarás explicaciones detalladas de los conceptos clave, junto con pasos prácticos para usarlos en IntelliJ, GitHub y la terminal de comandos.  

## 📖 Tabla de Contenidos  
1. [📥 Clonar un repositorio (`clone`)](#-clonar-un-repositorio-clone)  
2. [🍴 Hacer un fork (`fork`)](#-hacer-un-fork-fork)  
3. [✅ Realizar un commit (`commit`)](#-realizar-un-commit-commit)  
4. [🌿 Trabajar con ramas (`branches`)](#-trabajar-con-ramas-branches)  
5. [🎭 Main vs Master (`main/master`)](#-main-vs-master-mainmaster)  
6. [📩 Pull Request (`PR`)](#-pull-request-pr)  
7. [🔀 Merge (`merge`)](#-merge-merge)  
8. [🔄 Merge Squash (`merge squash`)](#-merge-squash-merge-squash)  
9. [⬇️ Actualizar cambios (`pull`)](#-actualizar-cambios-pull)  
10. [⬆️ Subir cambios (`push`)](#-subir-cambios-push)  
11. [🤝 Colaboradores (`collaborator`)](#-colaboradores-collaborator)  
12. [🐞 Issues (`issues`)](#-issues-issues)  
13. [🔨 Squash (`squash`)](#-squash-squash)  

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

