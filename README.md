### Proyecto LLM-Psychometric-Comparsion

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

graph TD
    A[Proyecto] --> B[docs]
    A --> C[src]
    A --> D[tests]
    A --> E[data]
    A --> F[scripts]
    A --> G[configs]
    A --> H[README.md]

    C --> C1[frontend]
    C --> C2[backend]
    C --> C3[mobile]

