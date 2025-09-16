# 📊 Proyecto Psicometría y LLM

Este repositorio contiene el desarrollo del **aplicativo web para la evaluación de rasgos no cognitivos** 
mediante pruebas psicométricas y su comparación con modelos de lenguaje (LLM).  

---

## 📖 Descripción del Proyecto

El sistema permite cargar pruebas psicométricas en formato Excel, analizarlas, 
y generar reportes comparativos en PDF/Excel.  
El objetivo es apoyar la **evaluación de rasgos no cognitivos** y contrastar 
resultados con modelos de lenguaje (LLM) para investigación académica.  

---

## 👥 Equipo de Desarrollo

- **Juan** – Control de versiones / DevOps  
- **Ana** – Frontend  
- **Carlos** – Backend  
- **Laura** – Documentación  

---

## 🛠️ Tecnologías y Herramientas

- **Frontend:** HTML, CSS, JavaScript  
- **Documentos:** Excel (entrada), PDF (salida)  
- **Gestión de versiones:** Git & GitHub  
- **Documentación técnica:** Markdown (`docs/`)  

---

## 📂 Estructura del Proyecto

```plaintext
📂 proyecto-psicometria-llm
├── 📂 docs/                   # Documentación del proyecto
├── 📂 src/                    # Código fuente (HTML, CSS, JS)
├── 📂 templates/              # Plantillas (Excel de entrada)
├── 📂 reports/                # Reportes exportados (PDF/Excel)
├── .gitignore                 # Archivos ignorados en Git
├── README.md                  # Documentación principal
└── LICENSE                    # Licencia del repositorio

🔄 Flujo de Trabajo (Git Flow)

Para mantener el desarrollo ordenado, seguimos la siguiente estrategia de ramas:

main → Rama estable (solo versiones probadas y listas para entrega).

develop → Rama de integración de funcionalidades antes de pasar a main.

feature/* → Cada funcionalidad o historia de usuario tendrá su propia rama.

fix/* → Ramas para corregir errores detectados.

hotfix/* → Ramas para solucionar errores urgentes en producción.

Pasos para trabajar en una nueva historia de usuario

Crear una nueva rama a partir de develop:

git checkout develop
git pull origin develop
git checkout -b feature/NEEDS-XX-descripcion


Realizar commits con convención tipo(ID-Historia): descripción breve:

git add .
git commit -m "feat(NEEDS-20): mostrar inventario psicométrico en pantalla"


Subir la rama al repositorio:

git push origin feature/NEEDS-XX-descripcion


Crear un Pull Request (PR) hacia develop:

En GitHub, abrir un PR de la rama feature/NEEDS-XX-descripcion hacia develop.

Solicitar revisión de al menos 1 compañero.

Integrar cambios a develop (solo el responsable de merges):

git checkout develop
git pull origin develop
git merge feature/NEEDS-XX-descripcion
git push origin develop


Cuando la versión esté lista para entrega:

git checkout main
git pull origin main
git merge develop
git push origin main

✅ Convenciones de Commits

Usamos el formato Conventional Commits:

feat: → Nueva funcionalidad

fix: → Corrección de errores

docs: → Cambios en documentación

style: → Cambios de formato sin alterar lógica

refactor: → Reestructuración de código sin modificar comportamiento

test: → Añadir o modificar tests

chore: → Tareas de mantenimiento (build, dependencias, configs)

Ejemplos de commits:
feat(NEEDS-20): mostrar inventario psicométrico en pantalla
feat(NEEDS-21): generar gráfico de resultados por rasgo
fix(NEEDS-23): corregir descarga del PDF de reporte
docs: agregar guía de instalación en README
refactor(NEEDS-26): simplificar validación del archivo cargado
test(NEEDS-24): agregar pruebas para reporte comparativo

🚀 Cómo Ejecutar el Proyecto

Clonar el repositorio:

git clone https://github.com/usuario/proyecto-psicometria-llm.git
cd proyecto-psicometria-llm


Abrir index.html en el navegador para ver la aplicación.

🗂️ Documentación

La documentación técnica y el SRS se encuentran en la carpeta docs/
.

📅 Roadmap

 Crear estructura inicial del proyecto

 Implementar carga de archivos Excel

 Generar reportes en PDF

 Comparación con modelos LLM

 Publicar versión estable