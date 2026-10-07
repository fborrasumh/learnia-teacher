# LEARNIA Teacher

Diseña el curso y mira cómo aprende tu clase. Aplicación web de un solo fichero.

**Usar la app:** https://fborrasumh.github.io/learnia-teacher/

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23218312.svg)](https://doi.org/10.5281/zenodo.23218312)

**Idiomas:** español (por defecto), inglés, portugués; selector en la barra superior (o `?lang=en` / `?lang=pt` en la URL).

## Qué hace

- Gestiona varios cursos: crear, importar, duplicar y eliminar.
- Materiales PDF, DOCX, PPTX, TXT y Markdown: el texto se extrae en el navegador y se guarda por página, diapositiva o sección (las imágenes no se incluyen).
- Mapa de conocimiento: temas, conceptos con prerrequisitos, competencias, dificultad y términos clave, con editor y grafo. La IA puede proponerlo desde los materiales; el código descarta términos clave que no aparecen en ellos, prerrequisitos inexistentes y ciclos, y tú revisas antes de aplicar.
- Actividades (test, respuesta corta, problema numérico, interpretación, explicación, aplicación y caso práctico), manuales o generadas por IA como borrador con comprobación de la cita en los materiales; los borradores no viajan en el curso hasta validarlos. Revisa siempre las soluciones numéricas generadas.
- Rúbricas con pesos (deben sumar 100 %).
- Exporta `curso.learnia.json` con versiones (curso, conocimiento y rúbricas) que suben solas si ese contenido cambia.
- Importa los `student.learnia.json` del alumnado (varios a la vez), recalcula el dominio desde sus evidencias y avisa si un fichero no pasa la comprobación de integridad o es de otra versión del curso.
- Análisis de clase determinista: dominio medio y progreso, mapa de conocimiento, conceptos críticos, errores y patrones compartidos, análisis de recuperación, evolución semanal, comparación de grupos y recomendaciones docentes por reglas.
- Informe en HTML, JSON y CSV (para PDF, imprime el HTML desde el navegador).

## Privacidad

Cursos, materiales y ficheros del alumnado se guardan en el navegador del profesor; el análisis es local y los datos del alumnado nunca se envían a la IA ni a ningún servidor. A la IA solo viajan extractos de los materiales y la petición, con aviso y muestra previos. La clave de IA se guarda solo en el navegador.

## Límites

Probada con IA simulada (suites automáticas de extremo a extremo), no con claves reales; la IA puede equivocarse y todo lo generado debe revisarlo el profesor o el estudiante. Los pesos y umbrales del algoritmo de dominio y de las recomendaciones son heurísticos y no están validados empíricamente. El PDF del informe no se genera directamente. Para uso institucional con clave compartida haría falta un proxy seguro, no incluido.

## Autoría

Fernando Borrás Rocher (Universidad Miguel Hernández de Elche).


ORCID: Fernando Borrás Rocher [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573)

## Cómo citar

Borrás Rocher, F. (2026). *LEARNIA Teacher* (v1.0.0) [Software]. DOI: [10.5281/zenodo.23218312](https://doi.org/10.5281/zenodo.23218312)

## Licencia

MIT. Véase [LICENSE](LICENSE).
