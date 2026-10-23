---
title: "Cómo resumir un PDF con IA (ChatGPT, Claude y Gemini)"
description: "Paso a paso para subir un PDF a ChatGPT, Claude o Gemini y obtener un resumen fiable: límites de cada herramienta, prompts para copiar y qué hacer con PDF largos o escaneados."
date: 2026-10-23
key: summarize-pdf-with-ai
tags: [pdf, resumir, chatgpt, claude, gemini, principiantes]
cover: /images/resumir-pdf-con-ia.svg
coverAlt: "Un documento PDF que se convierte en una lista de puntos clave dentro de un chat"
---

No necesitas una aplicación especial para "resumir PDF". Las versiones gratuitas de ChatGPT, Claude y Gemini pueden leer un PDF que subas y resumirlo en segundos. Lo que marca la diferencia entre un resumen vago y uno útil es cómo se lo pides y conocer los límites de cada herramienta con archivos largos o escaneados.

> **Respuesta rápida:** abre ChatGPT, Claude o Gemini, pulsa el botón **+** (o el clip) junto al cuadro de texto, sube tu PDF y escribe: *"Resume este PDF para [a quién va dirigido]. Dame un resumen de 3 frases, los 5 puntos clave y todas las cifras, fechas y plazos, con su página."* Después comprueba lo importante en el documento original, porque la IA puede omitir o equivocar detalles.

## Paso a paso

1. **Abre el chatbot** en el navegador o en la app del móvil: ChatGPT (chatgpt.com), Claude (claude.ai) o Gemini (gemini.google.com). Con una cuenta gratuita basta para la mayoría de documentos.
2. **Adjunta el PDF.** Pulsa el icono **+** o el clip junto al cuadro de mensaje y elige el archivo del ordenador o del móvil. En Gemini también puedes importarlo desde Google Drive si tienes conectadas las apps de Google Workspace.
3. **Di para quién es el resumen y qué necesitas.** "Resume esto" funciona, pero "Resume este contrato de alquiler para alguien que alquila por primera vez y dime qué gastos me tocan a mí" funciona mucho mejor.
4. **Haz preguntas de seguimiento** en el mismo chat: "¿Qué dice la cláusula 4 sobre la fianza?" o "Cítame la frase exacta sobre la duración del contrato". La IA mantiene el documento en la conversación.
5. **Verifica.** Pide que indique la página o el apartado de cada dato clave, abre el PDF y comprueba los que importan.

## Límites de cada herramienta (a octubre de 2026)

Estos son los límites que cada empresa publica en sus páginas de ayuda oficiales. Cambian a menudo, así que si un archivo no se sube, consulta el enlace de la sección de fuentes.

| | ChatGPT | Claude | Gemini |
|---|---|---|---|
| **Tamaño máximo** | 512 MB por archivo | 500 MB por archivo | 100 MB por archivo (salvo vídeo) |
| **Extensión máxima** | 2 millones de tokens por archivo de texto | 1.000 páginas por PDF | Depende del plan; Google AI Pro y Ultra amplían el contexto a 1 millón de tokens |
| **Plan gratuito** | Permite subir archivos, pero solo 3 al día | Permite subir archivos, con límites de uso más bajos que los planes de pago | Permite subir archivos; los planes de pago tienen límites más altos |
| **Archivos a la vez** | Sin límite por chat publicado | Hasta 20 por chat | Hasta 10 por mensaje |
| **Gráficos e imágenes dentro del PDF** | Solo analiza el texto | Texto e imágenes en PDF de hasta 100 páginas; solo texto entre 101 y 1.000 páginas | No lo detalla por tipo de archivo |

Un "token" es un trozo de palabra. Como referencia aproximada, 1 millón de tokens equivale a cientos de páginas de texto, así que el límite rara vez es un problema con documentos normales.

**Qué significa en la práctica:**

- **PDF del día a día** (un contrato, unos apuntes, un informe de 20 páginas): cualquiera de los tres funciona bien con el plan gratuito.
- **Varios PDF al día con plan gratuito:** ChatGPT gratis solo permite 3 archivos diarios, así que si resumes mucho, Claude o Gemini pueden resultarte más cómodos.
- **PDF donde importan los gráficos o las tablas en imagen:** Claude analiza los elementos visuales en PDF de hasta 100 páginas. ChatGPT, según su propia ayuda, solo analiza el texto del PDF.
- **Documentos muy largos** (un libro, un manual de 600 páginas, un temario completo de oposiciones): los tres aceptan archivos largos, pero el resumen de un documento enorme sale superficial. Mejor por capítulos (lo explicamos más abajo).

## Prompts para copiar y pegar

Cambia lo que va entre corchetes por tu caso.

**Resumen general**

> Resume el PDF adjunto para [público, por ejemplo "un jefe con poco tiempo" o "un estudiante de bachillerato"]. Dame: 1) un resumen de 3 frases, 2) los 5 puntos más importantes en viñetas, 3) todas las cifras, fechas, plazos o importes que aparezcan, con el número de página. No añadas nada que no esté en el documento.

**Contratos de alquiler, pólizas de seguro y condiciones**

> Resume este [contrato de alquiler / póliza / condiciones del servicio] en lenguaje sencillo para alguien sin formación jurídica. Enumera: qué obligaciones tengo, qué tengo que pagar y cuándo, cómo se cancela o se rescinde, qué penalizaciones hay y cualquier cláusula poco habitual en un documento de este tipo. Cita el texto exacto de cada punto e indica el número de cláusula.

La IA no es abogada. Úsala para entender el documento y preparar preguntas, no como asesoramiento legal. Las normas de alquiler cambian mucho entre países (y, en España, entre comunidades autónomas), así que confirma lo importante con un profesional o con el organismo oficial de tu país.

**Apuntes de estudio a partir de un tema o un artículo**

> Convierte este tema en apuntes de estudio: la idea central en 2 frases, los conceptos clave con una definición de una línea, las 3 ideas con más probabilidad de salir en el examen y 5 preguntas de práctica. Espera a que responda antes de darme las soluciones.

Funciona igual para la EBAU o la PAU en España, el examen de ingreso a la universidad en México o un parcial en Argentina o Colombia: indica en el prompt qué examen preparas para que ajuste el nivel.

**Artículo científico o trabajo académico**

> Resume este artículo: pregunta de investigación, método, muestra, resultados principales con las cifras que se reportan, limitaciones que mencionan los autores y lo que el estudio NO demuestra. Máximo 250 palabras.

**Informes antes de una reunión**

> Tengo 10 minutos antes de una reunión sobre este informe. Dime las 3 decisiones que plantea, el mejor argumento a favor y en contra de cada una, y 3 preguntas inteligentes que podría hacer.

**Documentos oficiales**

> Este PDF es [una resolución / una convocatoria de becas / una normativa]. Explícame en lenguaje claro a quién afecta, qué requisitos hay, qué documentos piden, cuáles son los plazos exactos y dónde se presenta la solicitud. Indica la página de cada dato.

Para plazos y requisitos, consulta siempre la fuente oficial (el boletín o la web del organismo) antes de presentar nada.

## Cómo resumir un PDF muy largo

Aunque una herramienta acepte un archivo de 500 páginas, pedir un único resumen de todo suele dar una visión genérica. Hazlo por capas:

1. **Pide primero la estructura:** "Haz una lista de los capítulos o apartados principales de este PDF con sus rangos de páginas".
2. **Resume por partes:** "Ahora resume el capítulo 3 (páginas 41 a 78) en 10 viñetas".
3. **Únelo al final:** "Con los resúmenes de capítulos anteriores, escribe un resumen de una página de todo el libro".

Si el archivo es demasiado grande, divídelo con cualquier herramienta gratuita de PDF (o con la opción "Imprimir a PDF" de tu ordenador eligiendo un rango de páginas) y sube las partes una a una en el mismo chat.

## ¿Y los PDF escaneados?

Un PDF escaneado es en realidad un conjunto de fotos de páginas, sin texto seleccionable. Para saberlo, intenta seleccionar una palabra en tu visor de PDF: si no puedes, es un escaneo.

- **Claude** analiza el contenido visual en PDF de hasta 100 páginas, así que los escaneos cortos suelen funcionar.
- **ChatGPT** solo analiza el texto de los PDF, y su ayuda indica que los PDF formados solo por imágenes no son compatibles. Alternativas: pasa primero el archivo por OCR (muchas apps de PDF lo hacen, y también Google Drive con "Abrir con Documentos de Google") o sube las páginas como imágenes, que ChatGPT sí puede leer.
- **Gemini** acepta PDF e imágenes; si un escaneo da malos resultados, prueba a subir fotos nítidas de las páginas.

Uses la herramienta que uses, revisa con cuidado nombres, cifras e importes en los escaneos, porque el texto borroso es donde más errores aparecen.

## Privacidad: piénsalo antes de subir

Subir un archivo es enviarlo a la empresa que gestiona el chatbot. Antes de hacerlo:

- **No subas** documentos con tu DNI, NIE, CURP o número de identificación, datos bancarios, informes médicos o archivos confidenciales del trabajo, salvo que tu empresa o centro de estudios haya aprobado esa herramienta para ello.
- **Revisa la configuración de datos.** ChatGPT, Claude y Gemini tienen ajustes que controlan si tus conversaciones pueden usarse para mejorar sus modelos. Búscalos en la configuración o en la página de privacidad de cada herramienta.
- **Quita lo que no necesitas.** Si solo te interesa resumir las condiciones, elimina antes las páginas con datos personales o copia y pega solo el apartado relevante.

## Errores que llevan a malos resúmenes

- **No decir para quién ni para qué.** "Resume" a secas da un resumen genérico. Indica quién lo va a leer y qué decisión o tarea debe facilitar.
- **Fiarse de las cifras sin comprobarlas.** La IA puede leer mal una tabla, mezclar datos de páginas distintas o afirmar algo que no está en el documento. Pide números de página y revisa los importantes.
- **Pedirlo todo a la vez.** Un resumen, una traducción, un esquema de diapositivas y un test en el mismo mensaje dan cuatro respuestas flojas. Ve de uno en uno.
- **Abrir un chat nuevo para cada pregunta.** Sigue preguntando en la misma conversación para que la IA conserve el documento.

## Preguntas frecuentes

**¿Se puede resumir un PDF con IA gratis?**
Sí. A octubre de 2026, los planes gratuitos de ChatGPT, Claude y Gemini permiten subir PDF. ChatGPT gratis limita la subida a 3 archivos al día; Claude y Gemini tienen límites de uso más bajos en el plan gratuito que en los de pago.

**¿Qué IA es mejor para resumir PDF?**
Con PDF de texto normales, las tres dan buenos resúmenes si usas un prompt concreto. Claude tiene el soporte publicado más claro para gráficos e imágenes dentro de PDF (hasta 100 páginas), Gemini encaja bien si tus archivos ya están en Google Drive y ChatGPT funciona bien con documentos de texto si no superas su límite diario gratuito. Con un documento importante, prueba el mismo prompt en dos herramientas y compara.

**¿Es seguro subir un PDF a ChatGPT, Claude o Gemini?**
Es como enviar el archivo a un servicio en línea: adecuado para documentos públicos o de poco riesgo, arriesgado para documentos privados o confidenciales. Revisa los ajustes de privacidad de la herramienta y las normas de tu empresa o centro antes de subir archivos sensibles.

**¿Por qué la IA dice que no puede leer mi PDF?**
Los motivos habituales son que el archivo es demasiado grande o largo para esa herramienta, que tiene contraseña o que es un escaneo sin capa de texto. Prueba a quitar la contraseña, dividir el archivo o pasarle OCR.

**¿Puede la IA resumir en español un PDF que está en inglés?**
Sí. Añade "Escribe el resumen en español" al prompt. Para documentos importantes, pide que ponga la frase original junto a cada punto traducido para poder comprobarlo.

**¿Puedo fiarme del resumen sin leer el PDF?**
Para lecturas de poco riesgo, un buen resumen suele bastar. Para contratos, exámenes o documentos médicos, legales o económicos, usa el resumen como mapa y lee tú mismo los apartados que importan.

## Fuentes

- [Centro de ayuda de OpenAI: File Uploads FAQ](https://help.openai.com/en/articles/8555545-file-uploads-faq)
- [Centro de ayuda de Claude: Upload files to Claude](https://support.claude.com/en/articles/8241126-upload-files-to-claude)
- [Ayuda de Gemini: Sube y analiza archivos en Gemini](https://support.google.com/gemini/answer/14903178)
