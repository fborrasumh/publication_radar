# Publication Radar

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.22662044.svg)](https://doi.org/10.5281/zenodo.22662044)

**Aplicación:** https://fborrasumh.github.io/publication_radar/

Sigue **lo último de las revistas de tu tema**, en cualquier área de investigación. Escribes el tema, el radar descubre en qué revistas se publica de verdad, eliges las que quieres seguir y te muestra sus artículos nuevos. Cada vez que vuelves, marca lo que ha salido desde tu última visita. **Todos los artículos son reales**, de OpenAlex y PubMed: la IA nunca genera referencias. Aplicación de un solo fichero (`index.html`), sin servidor ni cuenta.

**Idiomas:** español (por defecto), inglés y portugués, con selector en la barra superior (o `?lang=en` / `?lang=pt` en la URL).

## Novedades de la versión 3.0

- **Para cualquier investigador:** interfaz completa en español, inglés y portugués, y resumen de novedades en el idioma elegido.
- **Tu proveedor de IA:** OpenAI, Google Gemini o Anthropic Claude, con tu propia clave y el desplegable de los modelos disponibles en ella. La IA sigue siendo opcional.
- **El resumen se comprueba por código:** cada cita [n] debe corresponder a un artículo de la lista (las demás se señalan), las cifras que no aparecen en los títulos ni en los resúmenes se marcan, y debajo se listan los artículos citados con su enlace. El resumen se guarda con el radar.
- **Aviso previo** antes del primer envío a la IA en cada sesión, con una muestra de lo que sale.
- Los radares pasan a guardarse en IndexedDB; los de las versiones 1 y 2 se traen automáticamente, sin perder nada.
- Estilo Forja: portada con autoría y ORCID, «Cómo funciona» y «Dónde va cada cosa».

## Cómo funciona

| Paso | Qué hace | Fuente |
|---|---|---|
| Tema | Pocas palabras, mejor en inglés | — |
| Revistas | Cuenta los artículos del tema por revista (últimos cinco años) | OpenAlex |
| Novedades | Artículos recientes de las revistas elegidas; si un artículo está en las dos fuentes, aparece una vez | OpenAlex y PubMed (por ISSN) |
| Sugerencias de revistas (opcional) | La IA propone; cada revista se comprueba en OpenAlex y las que no existen se descartan | Tu proveedor de IA + OpenAlex |
| Resumen (opcional) | Boletín en tu idioma con citas numeradas, basado solo en títulos y resúmenes | Tu proveedor de IA |

Además: varios radares, filtros (nuevos, sin leer, leídos y texto), ventana de 30 días a 12 meses y exportación a RIS y BibTeX (Zotero, Mendeley, EndNote) y CSV.

## Privacidad

Los radares, lo leído y la clave de IA se guardan solo en el navegador. Las búsquedas van a OpenAlex y PubMed (con tu correo, si lo indicas, para que atiendan mejor las consultas). Solo las sugerencias y el resumen opcionales envían a tu proveedor de IA el tema, los nombres de revista y los títulos y resúmenes de los artículos; antes del primer envío de cada sesión ves una muestra.

## Límites

- La calidad depende de la cobertura de OpenAlex y PubMed: hay revistas sin resumen, con fechas de número futuro o con metadatos incompletos. PubMed solo cubre ciencias de la salud y de la vida.
- El recuento de revistas usa la búsqueda de texto de OpenAlex: un tema ambiguo puede traer revistas poco relacionadas. Revisa la lista antes de seguirla.
- La comprobación del resumen detecta citas [n] fuera de la lista y cifras ausentes del material, pero **no** que una frase atribuya a un artículo algo que no dice: lee los artículos citados antes de usar el resumen.
- El ejemplo hace una búsqueda real: necesita conexión.
- Las pruebas automáticas usan OpenAlex, PubMed y la IA simulados; la versión 3.0 no se ha probado aún con claves reales de cada proveedor.

## Cómo citar

Borrás Rocher, F. (2026). *Publication Radar* (versión 3.0.0) [Software]. Universidad Miguel Hernández de Elche. https://doi.org/10.5281/zenodo.22662044

El DOI es el de concepto: apunta siempre a la última versión. GitHub ofrece la cita en APA y BibTeX con el botón *Cite this repository*, a partir de `CITATION.cff`.

## Autoría

Fernando Borrás Rocher (Universidad Miguel Hernández de Elche) · ORCID [0000-0002-5519-4573](https://orcid.org/0000-0002-5519-4573)

Forma parte del catálogo [Herramientas IA para la academia](https://fborrasumh.github.io/ia/).

## Licencia

MIT © 2026 Fernando Borrás Rocher · Universidad Miguel Hernández de Elche.
