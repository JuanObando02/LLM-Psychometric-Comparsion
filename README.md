# 📊 Proyecto Psicometría y LLM

Este repositorio contiene el desarrollo del **aplicativo web para la evaluación de rasgos no cognitivos** 
mediante pruebas psicométricas y su comparación con modelos de lenguaje (LLM).  

## 🔄 Flujo de Trabajo (Git Flow)

Para mantener el desarrollo ordenado, seguimos la siguiente estrategia de ramas:

- **`main`** → Rama estable (solo versiones probadas y listas para entrega).  
- **`develop`** → Rama de integración de funcionalidades antes de pasar a `main`.  
- **`feature/*`** → Cada funcionalidad o historia de usuario tendrá su propia rama.   

### Pasos para trabajar en una nueva historia de usuario

1. Crear una nueva rama a partir de `develop`:
   ```bash
   git checkout develop
   git pull origin develop
   git checkout -b feature/NEEDS-XX-descripcion

2. Realizar los commits siguiendo la siguiente convención `tipo(ID-Historia): descripción breve`:
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

# Como crear commits

## 📂 Estructura del Proyecto

    ```plaintext
    📂 proyecto-psicometria-llm
    ├── 📂 docs/                   # Documentación del proyecto
    ├── 📂 src/                    # Código fuente (HTML, CSS, JS)
    ├── 📂 templates/              # Plantillas (Excel de entrada)
    ├── .gitignore                 # Archivos ignorados en Git
    ├── README.md                  # Documentación principal
    └── LICENSE                    # Licencia del repositorio

