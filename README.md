# 💰 Compendio de normas de Derecho Tributario chileno

[![Última versión](https://img.shields.io/github/v/release/n-a-monterocarvajal/Compendio-Derecho-Tributario-Chile?sort=date&display_name=tag&label=%C3%BAltima%20versi%C3%B3n)](https://github.com/n-a-monterocarvajal/Compendio-Derecho-Tributario-Chile/releases/latest)
[![Revisión semanal](https://github.com/n-a-monterocarvajal/Compendio-Derecho-Tributario-Chile/actions/workflows/revisar-versiones.yml/badge.svg?branch=main)](https://github.com/n-a-monterocarvajal/Compendio-Derecho-Tributario-Chile/actions/workflows/revisar-versiones.yml)
[![Generación](https://github.com/n-a-monterocarvajal/Compendio-Derecho-Tributario-Chile/actions/workflows/generar-compendio.yml/badge.svg?branch=main)](https://github.com/n-a-monterocarvajal/Compendio-Derecho-Tributario-Chile/actions/workflows/generar-compendio.yml)
[![Licencia: MIT](https://img.shields.io/github/license/n-a-monterocarvajal/Compendio-Derecho-Tributario-Chile?label=licencia)](https://github.com/n-a-monterocarvajal/Compendio-Derecho-Tributario-Chile/blob/main/LICENSE)

Genera y actualiza automáticamente un compendio en PDF de normas tributarias chilenas obtenidas desde el servicio Ley Chile, de la Biblioteca del Congreso Nacional de Chile.

Este repositorio revisa semanalmente las versiones de sus normas y genera un nuevo compendio PDF solo cuando detecta una actualización.

## 📚 Normas incluidas

1. [Decreto Ley N.º 830, de 1974, del Ministerio de Hacienda, que aprueba el Código Tributario.](https://www.bcn.cl/leychile/navegar?idNorma=6374)
2. [Decreto Ley N.º 824, de 1974, del Ministerio de Hacienda, que aprueba el texto de la Ley sobre Impuesto a la Renta.](https://www.bcn.cl/leychile/navegar?idNorma=6368)
3. [Decreto Ley N.º 825, de 1974, del Ministerio de Hacienda, que aprueba la Ley sobre Impuesto a las Ventas y Servicios.](https://www.bcn.cl/leychile/navegar?idNorma=6369)
4. [Decreto Supremo N.º 55, de 1977, del Ministerio de Hacienda, que aprueba el Reglamento de la Ley sobre Impuesto a las Ventas y Servicios.](https://www.bcn.cl/leychile/navegar?idNorma=8355)
5. [Decreto N.º 79, de 1991, del Ministerio de Economía, Fomento y Reconstrucción, que fija disposiciones por las cuales los exportadores que indica podrán recuperar el impuesto señalado en el Título II del Decreto Ley N.º 825, de 1974.](https://www.bcn.cl/leychile/navegar?idNorma=123235)
6. [Ley N.º 4.533, de 1929, del Ministerio de Hacienda, sobre impuesto a las herencias y donaciones.](https://www.bcn.cl/leychile/navegar?idNorma=237759)
7. [Decreto Ley N.º 3.475, de 1980, del Ministerio de Hacienda, que modifica la Ley de Timbres y Estampillas contenida en el Decreto Ley N.º 619, de 1974.](https://www.bcn.cl/leychile/navegar?idNorma=7137)
8. [Decreto con Fuerza de Ley N.º 7, de 1980, del Ministerio de Hacienda, que fija el texto de la Ley Orgánica del Servicio de Impuestos Internos y adecua disposiciones legales que señala.](https://www.bcn.cl/leychile/navegar?idNorma=3747)
9. [Ley N.º 20.322, que fortalece y perfecciona la jurisdicción tributaria y aduanera, Ley Orgánica de Tribunales Tributarios y Aduaneros.](https://www.bcn.cl/leychile/navegar?idNorma=286151)
10. [Ley N.º 21.713, que dicta normas para asegurar el cumplimiento de las obligaciones tributarias dentro del Pacto por el Crecimiento Económico, el Progreso Social y la Responsabilidad Fiscal.](https://www.bcn.cl/leychile/navegar?idNorma=1207746)
11. [Decreto Ley N.º 910, de 1975, del Ministerio de Hacienda, que modifica los Decretos Leyes N.os 619, 824, 825, 826, 827 y 830, y establece el crédito especial para empresas constructoras.](https://www.bcn.cl/leychile/navegar?idNorma=6399)
12. [Ley N.º 21.078, sobre transparencia del mercado del suelo e impuesto al aumento de valor por ampliación del límite urbano.](https://www.bcn.cl/leychile/navegar?idNorma=1115067)
13. [Decreto con Fuerza de Ley N.º 1, de 1998, del Ministerio de Hacienda, que fija el texto refundido, coordinado, sistematizado y actualizado de la Ley N.º 17.235, sobre Impuesto Territorial.](https://www.bcn.cl/leychile/navegar?idNorma=128563)

*La selección de las normas está basada en el índice de la publicación [Compendio Tributario (Hammurabi)](https://editorial.tirant.com/cl/libro/compendio-de-normas-ambientales-de-chile-pavez-torrealba-felipe-ignacio-9791370402808).*

## 📄 PDF generado

El *workflow* produce un archivo PDF con nombre versionado por fecha y hora UTC:

```text
CompendioDerechoTributarioChile_YYYYMMDD_HHMM_UTC.pdf
```

## 📥 Descarga del compendio

La versión más reciente del compendio se publica como *release* del repositorio:

[Descargar última versión publicada del compendio](https://github.com/n-a-monterocarvajal/Compendio-Derecho-Tributario-Chile/releases/latest)

El historial de versiones anteriores se encuentra disponible en la sección de *releases* del repositorio.

Cada publicación nueva incluye un archivo `.sha256`, una certificación de procedencia de GitHub y un enlace al *run* que produjo el PDF. Las notas del *release* contienen el comando exacto para verificar la certificación. Las publicaciones futuras son inmutables: una corrección siempre origina una versión nueva.

Los *artifacts* del PDF y su *checksum* se mantienen adicionalmente como respaldo temporal durante 30 días.

## 🔄 Actualización automática

El estado normalizado de las versiones se compara semanalmente con la información vigente de Ley Chile. Una nueva vigencia, un cambio de versión actual, un evento pendiente o una modificación de las alertas de texto diferido dispara una ejecución separada del generador. Las notas del *release* indican qué normas cambiaron.

El obtenedor, el ensamblador PDF, el monitor de versiones y sus decisiones técnicas se mantienen en [GeneradorCompendiosLeyChile](https://github.com/n-a-monterocarvajal/GeneradorCompendiosLeyChile). Este repositorio fija una revisión inmutable de ese motor para que sus actualizaciones sean explícitas y auditables.

## 🔐 Licencia

El código de este repositorio se publica bajo licencia MIT. Las normas descargadas pertenecen a sus respectivas fuentes oficiales y se obtienen desde sitios públicos al momento de cada ejecución.
