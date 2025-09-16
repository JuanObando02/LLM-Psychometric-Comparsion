# 📊 Proyecto Psicometría y LLM

1. 📖 Descripción del Proyecto
Este repositorio contiene el desarrollo del **aplicativo web para la evaluación de rasgos no cognitivos** 
mediante pruebas psicométricas y su comparación con modelos de lenguaje (LLM).  

2. 👥 Equipo de Desarrollo

Lista los integrantes con sus roles:

Juan – Control de versiones / DevOps

Ana – Frontend

Carlos – Backend

Laura – Documentación

3. 🛠️ Tecnologías y Herramientas

Enumera el stack que usarán:

HTML, CSS, JavaScript

Node.js / React (si aplica)

Git & GitHub

Excel como entrada

PDF como salida

4. 📂 Estructura del Repositorio
<pre>
📂 proyecto-psicometria-llm
├── 📂 docs/                     # Documentación del proyecto
├── 📂 src/                      # Código fuente (HTML, CSS, JS)
│    ├── 📂 assets/              # Imágenes, estilos, etc.
│    └── 📂 pages/               # Páginas principales
├── 📂 test/                     # Pruebas y resultados de los LLM 
│    ├── 📂 unit/                # Pruebas unitarias (frontend/backend)
│    ├── 📂 integration/         # Pruebas de integración
│    └── 📂 llm/                 # Pruebas específicas de modelos LLM
│         ├── 📂prompts/         # Conjuntos de prompts usados en pruebas
│         ├── 📂results/         # Resultados obtenidos
│         └── 📂reports/         # Reportes y métricas de evaluación
├── 📂 templates/                # Plantillas (Excel de entrada)
├── .gitignore                   # Archivos ignorados en Git
├── README.md                    # Documentación principal
└── LICENSE                      # Licencia del repositorio </pre>

5. 🔄 Flujo de Trabajo (Git Flow)

Para mantener el desarrollo ordenado, seguimos la siguiente estrategia de ramas:

- **`main`** → Rama estable (solo versiones probadas y listas para entrega).  
- **`develop`** → Rama de integración de funcionalidades antes de pasar a `main`.  
- **`feature/*`** → Cada funcionalidad o historia de usuario tendrá su propia rama.   

6. ✅ Convenciones de Commits

Usamos el formato **Conventional Commits** para mantener un historial ordenado:

- `feat:` → Nueva funcionalidad  
- `fix:` → Corrección de errores  
- `docs:` → Cambios en documentación  
- `style:` → Formato (indentación, espacios, etc.) sin cambios de lógica  
- `refactor:` → Reestructuración de código sin cambiar comportamiento  
- `test:` → Añadir o modificar tests  
- `chore:` → Tareas de mantenimiento (build, dependencias, configs)  

### Pasos para trabajar en una nueva historia de usuario

1. Crear una nueva rama a partir de `develop`:
   ```bash
   git checkout develop
   git pull origin develop
   git checkout -b feature/NEEDS-XX-descripcion

2. Realizar los commits siguiendo la siguiente convención `tipo(ID-Historia): descripción breve`:
    ```bash
    git add .
    git commit -m "feat: implementar NEEDS-XX sección de evaluación de rasgos"
Ejemplos:
    ```bash
    feat(NEEDS-20): mostrar inventario psicométrico en pantalla
    feat(NEEDS-21): generar gráfico de resultados por rasgo
    fix(NEEDS-23): corregir descarga del PDF de reporte
    docs: agregar guía de instalación en README
    refactor(NEEDS-26): simplificar validación del archivo cargado
    test(NEEDS-24): agregar pruebas para reporte comparativo

3. Subir la rama al repositorio.
    ```bash
    git push origin feature/NEEDS-XX-descripcion
    
4. Crear un Pull Request (PR) hacia develop:
    - En GitHub, abrir un PR de la rama feature/NEEDS-XX-descripcion hacia develop.
    - Solicitar revisión de al menos 1 compañero.

5. Integrar cambios a develop (solo el responsable de merges)
    ```bash 
    git checkout develop
    git pull origin develop
    git merge feature/NEEDS-XX-descripcion
    git push origin develop
