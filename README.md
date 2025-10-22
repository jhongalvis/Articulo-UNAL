Este proyecto contiene una versión inicial del artículo derivado de la monografía.

## Estructura del proyecto

```
overleaf-project/
├── main.tex                    # Archivo principal del artículo
├── revcoles.cls                # Clase de la Revista Colombiana de Estadística
├── references.bib              # Base de datos bibliográfica
├── sections/                  # Secciones del manuscrito
│   ├── 00_title_abstract.tex  # Título, autores, resúmenes y palabras clave
│   ├── 01_introduction.tex    # Introducción
│   ├── 02_methods.tex         # Métodos
│   ├── 03_results.tex         # Resultados
│   ├── 04_discussion.tex      # Discusión
│   ├── 05_conclusions.tex     # Conclusiones
│   └── 06_ack_funding_ethics_data.tex # Agradecimientos y otras secciones editoriales
├── figures/                  # Figuras utilizadas en el artículo
│   ├── modelo.pdf
│   └── modelosem_216.pdf
└── tables/                   # Tablas en formato LaTeX (vacío por ahora)
```

### Compilación

El archivo `main.tex` utiliza la clase `revcoles.cls` proporcionada por la revista.  Para compilar el manuscrito se recomienda utilizar `latexmk` o la interfaz de Overleaf con el motor *pdfLaTeX*.  El preámbulo está ajustado para incluir las secciones mediante `\input`.  Recuerde ejecutar BibTeX para generar la bibliografía.

### Contenido por completar

- **Agradecimientos y secciones editoriales**: Deben especificarse los agradecimientos, las fuentes de financiación, la disponibilidad de datos y las contribuciones de autoría en el archivo `06_ack_funding_ethics_data.tex`.
- **Citas y referencias**: Asegúrese de que todas las citas en el texto correspondan con una entrada en `references.bib` y viceversa.  El estilo de citación por defecto es de la clase `revcoles`, basado en `natbib`.
- **Datos de participantes**: Algunos valores demográficos (edad media, proporción de hombres/mujeres) se indican como variables por completar en la sección de Métodos.

Esta estructura se ajusta a las directrices de la Revista Colombiana de Estadística y está lista para su edición y mejora iterativa.