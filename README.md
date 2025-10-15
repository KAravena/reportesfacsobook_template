
# reportesfacsobook

Plantilla **Quarto (project: book)** para tesis, informes e investigaciones en FACSO (U. de Chile).  
Inspirada en *tesisfacsodown*, pero 100% **Quarto** (HTML + PDF + DOCX).

## Requisitos
- Quarto ≥ 1.5
- LaTeX (TinyTeX o TeXLive) para PDF
- (Opcional) R y paquetes `tidyverse`, `knitr`, `gt`, `broom` para ejemplos reproducibles

## Uso rápido
1. Clona o descarga este repo.
2. Edita `_quarto.yml` (título, autores, etc.).
3. Escribe en los capítulos `01-*.qmd`, `02-*.qmd`, etc.
4. Renderiza:
   ```bash
   quarto render
   ```
5. Publica en GitHub Pages:
   - Activa Pages desde la carpeta `_book/`
   - (Opcional) usa el workflow en `.github/workflows/quarto-publish.yml`

## Estructura
- `index.qmd` — portada, resumen, agradecimientos, lista de figuras/tablas.
- `01-introduccion.qmd`...`06-conclusiones.qmd` — capítulos de ejemplo.
- `apendices/` — material suplementario.
- `assets/styles.scss` — estilo visual (HTML + PDF).
- `includes/` — plantillas de portada personalizadas para HTML/PDF.
- `refs/` — bibliografía `.bib` y estilo `.csl`.
- `data/` — coloca tus datos (no versionados por defecto).