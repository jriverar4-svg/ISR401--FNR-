# GA-SUM-02 | EXP-1 — Técnicas de elicitación y herramientas de apoyo a la Ingeniería de Requerimientos

Repositorio de la presentación académica correspondiente a la asignatura **Ingeniería de Requerimientos (ISR-401)** de la Universidad Técnica Estatal de Quevedo (UTEQ).

El trabajo aborda las técnicas de elicitación de requisitos, la comparación de herramientas de apoyo a la Ingeniería de Requerimientos y una demostración práctica de **StrictDoc**, aplicada al proyecto formativo de curso (PFC) *Local de Manualidades*.

## 1. Información general

| Campo | Descripción |
|---|---|
| Institución | Universidad Técnica Estatal de Quevedo (UTEQ) |
| Carrera | Ingeniería en Software |
| Asignatura | Ingeniería de Requerimientos (ISR-401) |
| Actividad | GA-SUM-02 |
| Experiencia | EXP-1 |
| Estudiante | Rivera Rodriguez Joseph Jeremy |
| Semestre | Cuarto semestre |
| Paralelo | A |
| Equipo | FNR |
| Docente | Dr. Gleiston Cicerón Guerrero Ulloa |
| Fecha | 21 de noviembre de 2026 |

## 2. Contenido de la presentación

La presentación desarrolla los siguientes apartados:

1. **Introducción y propósito:** importancia de la elicitación y la trazabilidad de requisitos.
2. **Contexto del PFC:** descripción del Local de Manualidades y sus necesidades.
3. **Técnicas de elicitación:** entrevista semiestructurada, observación no participante y cuestionarios.
4. **Herramientas de apoyo a la IR:** comparación entre Jira, Enterprise Architect y StrictDoc.
5. **Recomendación:** justificación de StrictDoc como herramienta para el PFC.
6. **Demostración práctica:** estructuración de necesidades, requisitos funcionales y casos de prueba mediante archivos `.sdoc`.
7. **Conclusiones:** resultados y aportes de las técnicas y herramientas estudiadas.
8. **Uso de IA y referencias:** declaración de asistencia mediante inteligencia artificial y fuentes bibliográficas.

## 3. Estructura del repositorio

```text
ISR401--FNR-/
│
├── main.tex
├── referencias.bib
├── README.md
├── main.pdf
│
└── evidencias/
    ├── captura-export-html.png
    └── captura-trazabilidad.png
```

**Nota:** `main.tex` es el archivo fuente principal. `referencias.bib` contiene las referencias bibliográficas utilizadas mediante BibTeX. La carpeta `evidencias/` almacena las capturas utilizadas en la presentación.

El archivo `main.pdf` corresponde al documento compilado y puede regenerarse utilizando el procedimiento descrito a continuación.

## 4. Entorno de compilación

La presentación está desarrollada utilizando **LaTeX con la clase Beamer**, con una relación de aspecto panorámica 16:9.

### 4.1. Software necesario

| Herramienta | Función |
|---|---|
| MiKTeX o TeX Live | Distribución de LaTeX |
| pdfLaTeX | Compilación del archivo `.tex` |
| BibTeX | Procesamiento de referencias bibliográficas |
| Git | Clonación y gestión del repositorio |
| TeXstudio (opcional) | Editor de archivos LaTeX |

Se recomienda utilizar una distribución completa de TeX Live o MiKTeX con instalación automática de paquetes.

### 4.2. Dependencias LaTeX

El documento utiliza los siguientes paquetes:

- `beamer`: estructura y formato de la presentación.
- `inputenc`: codificación de caracteres UTF-8.
- `fontenc`: codificación de fuentes.
- `babel`: configuración del idioma español.
- `lmodern`: fuentes tipográficas.
- `booktabs`: formato de tablas.
- `array`: personalización de columnas.
- `colortbl`: colores en tablas.
- `tikz`: elaboración de diagramas.
- `positioning` y `arrows.meta`: bibliotecas de TikZ.
- `listings`: presentación de código fuente.
- `graphicx`: inclusión de imágenes.
- `xcolor`: definición y aplicación de colores.
- `hyperref`: enlaces y referencias.
- `IEEEtran`: estilo bibliográfico IEEE utilizado por BibTeX.

**Importante:** estos paquetes se instalan mediante la distribución LaTeX. No es necesario instalarlos individualmente si se dispone de una instalación completa.

## 5. Clonar el repositorio

Para obtener el proyecto en un entorno local, ejecutar:

```bash
git clone https://github.com/jriverar4-svg/ISR401--FNR-.git
```

Ingresar al directorio:

```bash
cd ISR401--FNR-
```

## 6. Compilación del documento

El archivo principal es `main.tex` y el motor de compilación utilizado es **pdfLaTeX**.

Para generar correctamente el PDF, se debe seguir este orden de ejecución:

### 6.1. Primera compilación con pdfLaTeX

```bash
pdflatex main.tex
```

Genera los archivos auxiliares necesarios para el procesamiento de referencias.

### 6.2. Procesamiento bibliográfico con BibTeX

```bash
bibtex main
```

Procesa las referencias definidas en `referencias.bib`.

### 6.3. Segunda compilación con pdfLaTeX

```bash
pdflatex main.tex
```

Actualiza las citas y referencias bibliográficas dentro del documento.

### 6.4. Tercera compilación con pdfLaTeX

```bash
pdflatex main.tex
```

Resuelve las referencias cruzadas y consolida el documento final.

Al finalizar, se obtiene:

```text
main.pdf
```

Este archivo contiene la presentación compilada y puede abrirse con cualquier lector de PDF.

## 7. Compilación desde TeXstudio (opcional)

También es posible compilar el proyecto mediante una interfaz gráfica utilizando TeXstudio.

1. Abrir TeXstudio.
2. Seleccionar **Archivo → Abrir**.
3. Abrir `main.tex`.
4. Configurar `pdfLaTeX` como compilador.
5. Ejecutar pdfLaTeX.
6. Ejecutar BibTeX.
7. Ejecutar pdfLaTeX dos veces adicionales.
8. Revisar el resultado en el visor PDF integrado.

Se debe verificar que `referencias.bib` y la carpeta `evidencias/` se encuentren en las rutas correspondientes.

## 8. Recursos gráficos y evidencias

Las imágenes utilizadas en la presentación se encuentran en:

```text
evidencias/
```

Los archivos esperados son:

- `captura-export-html.png`: evidencia del documento exportado desde StrictDoc.
- `captura-trazabilidad.png`: evidencia de las relaciones de trazabilidad entre los elementos documentados.

Si se modifican las capturas, se deben conservar los nombres y las rutas utilizadas en `main.tex`, o actualizar las referencias correspondientes.

Si las imágenes no están disponibles, el documento contempla marcadores de posición para evitar que su ausencia impida la compilación.

## 9. Demostración de StrictDoc

La presentación incluye una demostración de la estructuración de requisitos mediante StrictDoc.

Los elementos utilizados como ejemplo son:

| Identificador | Tipo | Descripción |
|---|---|---|
| N-01 | Necesidad | Seguimiento de pedidos personalizados |
| RF-01 | Requisito funcional | Registrar pedido |
| CP-01 | Caso de prueba | Registrar pedido con datos válidos |

La relación de trazabilidad se establece de la siguiente manera:

```text
N-01
 └── RF-01
      └── CP-01
```

Los comandos utilizados en la demostración son:

```bash
pip install strictdoc
strictdoc --version
strictdoc export .
strictdoc server .
```

**Nota:** StrictDoc se utiliza para la demostración práctica de la presentación. No es una dependencia necesaria para compilar el archivo `main.tex` y generar el PDF.

## 10. Tecnologías utilizadas

- **LaTeX / Beamer:** elaboración de la presentación.
- **BibTeX / IEEEtran:** gestión de referencias bibliográficas.
- **TikZ:** diagramas y elementos gráficos.
- **StrictDoc:** documentación y trazabilidad de requisitos.
- **Git / GitHub:** control de versiones y almacenamiento del proyecto.

## 11. Autoría

**Rivera Rodriguez Joseph Jeremy**

Ingeniería en Software — Cuarto semestre, paralelo A.

Universidad Técnica Estatal de Quevedo (UTEQ).

Asignatura: Ingeniería de Requerimientos (ISR-401).

Equipo: FNR.

---

**Repositorio:** https://github.com/jriverar4-svg/ISR401--FNR-
