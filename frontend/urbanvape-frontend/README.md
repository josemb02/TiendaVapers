# 🛍️ TiendaVapers - UrbanVapeFrontend

Este proyecto forma parte de la asignatura **Puesta en Producción Segura**.  
El objetivo es desarrollar y desplegar una tienda web de vapers aplicando buenas prácticas de seguridad, control de versiones y trabajo en equipo.

El frontend está desarrollado con **Angular 21 + Tailwind CSS**.

---

## 👥 Organización del trabajo en Git (flujo seguro)

Utilizamos un flujo basado en ramas para evitar errores en producción y asegurar calidad:

| Rama                | Propósito                                        | Responsable          |
|---------------------|--------------------------------------------------|----------------------|
| `main`              | Versión estable y lista para producción         | Protegida (solo PR) |
| `dev`               | Integración y pruebas del equipo                | Revisor / líder     |
| `feature/frontend`  | Desarrollo del frontend en Angular              | Programador frontend |
| `feature/database`  | Scripts y estructura de BD MySQL                | Programador BD       |

✔ Los cambios se suben a ramas `feature/*`  
✔ Se fusiona a `dev` mediante **Pull Request**  
✔ `main` recibe solo código probado y aprobado 🛡️  

---

## 📚 Comandos básicos de Git para el equipo

### 🚀 Clonar el proyecto
```bash
git clone https://github.com/josemb02/TiendaVapers.git
cd TiendaVapers

### descargar ultimos cambios de la rama actual 
git pull

###ver la rama donde estas 
git checkout

###  refrescar la rama 
git fetch

### Ver en qué rama estamos
git branch

### Ver todas las ramas (locales y remotas)
git branch -a

###Cambiar de rama
git checkout nombre-de-la-rama

git checkout feature/frontend
git checkout feature/database
git checkout dev

### Subir código al repositorio (ciclo completo)
git add .
git commit -m "Descripción del cambio realizado"
git push

###git status
git status

###Ver el historial de commits
git log
