# Publication Radar

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22662044.svg)](https://doi.org/10.5281/zenodo.22662044)

**Aplicación:** https://fborrasumh.github.io/publication_radar/

Sigue **lo último de las revistas de tu tema**. Escribes el tema, el radar descubre en qué revistas se publica de verdad, eliges las que quieres seguir y te muestra sus artículos nuevos. Cada vez que vuelves, marca lo que ha salido desde tu última visita. **Todos los artículos son reales**, de OpenAlex y PubMed: la IA nunca genera referencias. Aplicación de un solo fichero (`index.html`), sin servidor ni cuenta.

## Novedades de la versión 2.0

- **Ya no inventa artículos.** La versión 1 pedía a GPT registros bibliográficos «realistas» (con DOI falsos) cuando había pocos resultados y los mezclaba con los reales. Al migrar un radar antiguo, esos artículos se eliminan y se avisa.
- **Las revistas elegidas filtran de verdad**: en OpenAlex por su identificador y en PubMed por su ISSN. Antes se ignoraban. Si un artículo aparece en las dos fuentes, se muestra una sola vez.
- **Revistas con datos**: cada una viene con el número de artículos sobre el tema en los últimos cinco años. Las sugerencias de la IA y las añadidas a mano se comprueban en OpenAlex.
- **Funciona sin clave.** Con una clave de OpenAI (opcional), resumen de novedades en español basado solo en los resúmenes reales y citando cada artículo por su número.
- Recorrido guiado con el estilo de Forja (**Tema → Revistas → Novedades**), temas de ejemplo y un ejemplo que hace la búsqueda real sin clave.
- **Varios radares**, marca de **nuevo** desde la última revisión, filtros (nuevos, sin leer, leídos y texto) y ventana temporal de 30 días a 12 meses.
- **Exportación a RIS y BibTeX** (Zotero, Mendeley, EndNote) y CSV.
- Migración automática de la versión 1. La clave pasa a ser la compartida del catálogo (`ia_openai_key`).

## Cómo funciona

| Paso | Qué hace | Fuente |
|---|---|---|
| Tema | Pocas palabras, mejor en inglés | — |
| Revistas | Cuenta los artículos del tema por revista (últimos cinco años) | OpenAlex |
| Novedades | Artículos recientes de las revistas elegidas | OpenAlex y PubMed (por ISSN) |
| Resumen (opcional) | Boletín en español con citas numeradas | OpenAI, solo con títulos y resúmenes |

## Privacidad

Los radares se guardan solo en el navegador (`localStorage`). Las búsquedas van a OpenAlex y PubMed. Solo el resumen opcional envía títulos y resúmenes a OpenAI.

## Cómo citar

Borrás Rocher, F. (2026). *Publication Radar* (versión 2.0.0) [Software]. Universidad Miguel Hernández de Elche. https://doi.org/10.5281/zenodo.22662044

El DOI es el de concepto: apunta siempre a la última versión. GitHub ofrece la cita en APA y BibTeX con el botón *Cite this repository*, a partir de `CITATION.cff`.

Forma parte del catálogo [Herramientas IA para la academia](https://fborrasumh.github.io/ia/).

## Licencia

MIT © 2026 Fernando Borrás Rocher · Universidad Miguel Hernández de Elche.
