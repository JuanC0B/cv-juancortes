# CV Juan Cortes (LaTeX)

Repositorio con las fuentes en LaTeX de documentos profesionales de Juan Diego Cortes Barbosa. El propósito es mantener una fuente editable, versionada y reproducible para generar PDFs cuando sea necesario.

## Estructura

### Currículum Vitae
- `CV.JuanCortes.tex` — CV en inglés (versión principal).
- `CV.JuanCortes.ES.tex` — CV en español.

### Archivos Generados
- `*.aux`, `*.bbl`, `*.blg`, `*.log`, `*.out` — Archivos auxiliares de compilación LaTeX.

## Requisitos

1. Una distribución de LaTeX instalada (MiKTeX o TeX Live).
2. `pdflatex` y `bibtex` disponibles en la variable PATH.
3. (Opcional) Editor recomendado: TeXstudio o VS Code con LaTeX Workshop.

## Cómo compilar (PowerShell)

Abre PowerShell en la carpeta del repositorio y ejecuta los siguientes comandos según el documento que quieras generar:

### Compilar CV en inglés
```powershell
pdflatex "CV.JuanCortes.tex"
bibtex "CV.JuanCortes"
pdflatex "CV.JuanCortes.tex"
pdflatex "CV.JuanCortes.tex"
```

### Compilar CV en español
```powershell
pdflatex "CV.JuanCortes.ES.tex"
```


> **Nota:** La doble compilación es necesaria para resolver referencias cruzadas y bibliografía correctamente. Si faltan paquetes, MiKTeX suele preguntar para instalarlos automáticamente.
