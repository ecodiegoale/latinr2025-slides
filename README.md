# LatinR 2025 – Slides (código fuente)

Este repositorio contiene el **código fuente** de la charla presentada en **LatinR 2025**, el 5 de diciembre de 2025 ([enlace al programa](https://latinr.org/cronograma/programa/)), elaborada en **R Markdown**, junto con los archivos necesarios para reproducir el estilo visual (tema, logos e imágenes).

---

## Descripción

Esta presentación analiza la dinámica de relocalización empresarial en la frontera norte de México, con énfasis en el papel de los incentivos diferenciados —en particular, un salario mínimo más alto que en el resto del país y la presencia de estímulos fiscales— en las decisiones de localización de las unidades económicas.

El análisis se basa en registros administrativos a nivel empresa para el periodo 2018–2021. A partir de esta información, se construye una tipología de migración territorial y se estiman modelos de riesgos proporcionales de Cox para examinar cómo las firmas ajustan sus decisiones de ubicación en respuesta a estos incentivos.

---

## Estructura del repositorio

El repositorio está organizado de la siguiente manera:

- `latinR_slides.Rmd`  
  Archivo principal en R Markdown que genera la presentación.

- `latinR.css`  
  Hoja de estilos personalizada utilizada para definir el tema visual de las diapositivas.

- `plots/`  
  Carpeta con gráficos utilizados en la presentación.

- Archivos de imágenes y logotipos (`.png`, `.svg`)  
  Incluidos para permitir que terceros puedan **replicar el diseño y el estilo visual** de la presentación.

Los archivos gráficos se incluyen como *assets estáticos*. El objetivo del repositorio es reproducir la presentación y su formato visual, no compartir el código necesario para replicar todos los resultados a partir de los datos originales.

---

## Nota sobre datos y resultados

Por razones de confidencialidad, **no se incluyen microdatos** ni bases administrativas utilizadas en el análisis.

Los resultados presentados en las diapositivas se apoyan en versiones preliminares de mi investigación que fueron publicadas en el *Informe sobre el comportamiento de la economía* correspondiente al mes de julio de 2025, elaborado por la Dirección Técnica y presentado al Consejo de Representantes de la **Comisión Nacional de los Salarios Mínimos (CONASAMI)**.

Asimismo, versiones preliminares del trabajo han sido discutidas en otros espacios académicos, incluyendo el [**Congreso SobreMéxico2025**](https://sobremexico.ibero.mx/es/congreso/call-for-papers) de la Universidad Iberoamericana.

Una versión preliminar del informe institucional puede consultarse en el siguiente enlace:

- https://www.gob.mx/cms/uploads/attachment/file/1013236/Informe_Julio_2025.pdf

Esta versión del código corresponde a la presentación realizada en **LatinR 2025**, aunque parte del trabajo ha sido discutido previamente en otros foros.
---

## Reproducibilidad

Para generar la presentación a partir del código fuente:

```r
rmarkdown::render("latinR_slides.Rmd")

