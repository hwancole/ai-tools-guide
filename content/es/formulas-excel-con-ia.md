---
title: "Cómo hacer fórmulas de Excel con IA (gratis y con Copilot)"
description: "Pide a ChatGPT, Claude, Gemini o Copilot fórmulas de Excel y Google Sheets que funcionen a la primera: cómo describir tu hoja, prompts para copiar y el lío del punto y coma."
date: 2026-10-26
key: ai-excel-formulas
tags: [excel, hojas-de-calculo, google-sheets, copilot, gemini, chatgpt, claude]
cover: /images/formulas-excel-con-ia.svg
coverAlt: "Una petición en lenguaje normal que se convierte en una fórmula de hoja de cálculo en una celda resaltada"
---

Ya no hace falta saberse de memoria BUSCARV ni SUMAR.SI.CONJUNTO. Cualquier chatbot de IA puede escribirte una fórmula si le cuentas tres cosas: qué hay en cada columna, dónde están los datos y qué resultado quieres en qué celda. Y en español hay una cuarta que casi nadie menciona: decirle que tu Excel está en español, porque si no te devolverá la fórmula en inglés y con comas, y no funcionará al pegarla.

> **Respuesta rápida:** abre ChatGPT, Claude o Gemini (los planes gratuitos sirven). Describe tu hoja así: *"Uso Excel 365 en español con punto y coma como separador. En A2:A500 hay fechas y en C2:C500 importes. En F2 quiero el total de la columna C del mes de la fecha que escribo en E2."* Pega la fórmula en la celda y compruébala con dos o tres filas que puedas calcular a mano. Si pagas Microsoft 365 con Copilot o un plan de Google con Gemini, también puedes pedirlo dentro de la propia hoja.

## Tus opciones de un vistazo

A octubre de 2026, según las páginas de ayuda de cada empresa:

| Opción | Coste | Dónde preguntas | ¿Ve tu archivo? |
|---|---|---|---|
| **Chat de ChatGPT, Claude o Gemini** | Los planes gratuitos bastan para fórmulas | Una pestaña del navegador al lado de tu hoja | Solo lo que pegues o subas |
| **Copilot en Excel** | Microsoft 365 Personal o Familia con un plan de créditos de IA, Microsoft 365 Premium, o un plan de empresa compatible | Panel de Copilot dentro de Excel | Sí, el libro abierto |
| **Gemini en Google Sheets** | Un plan de Google Workspace o Google AI compatible | Escribiendo `=` en una celda, o en el panel lateral de Gemini | Sí, la hoja abierta |

Dos novedades que conviene saber:

- **La función `=COPILOT()` ya no existe.** Microsoft indica que dejó de estar disponible en Excel el 14 de septiembre de 2026. Los libros que la usaban conservan los resultados ya calculados, pero al recalcular muestran `#¿NOMBRE?`. Copilot sigue funcionando desde su panel.
- **Gemini en Sheets entiende español.** Google incluye el español entre los idiomas admitidos en el panel lateral de Gemini en Hojas de cálculo, y también puede arreglar fórmulas rotas: pasa el ratón por la celda con error y pulsa **Fix**.

Si no tienes ninguno de los planes de pago, el método gratuito de abajo hace lo mismo con un paso más: copiar y pegar.

## El detalle que rompe la mitad de las fórmulas: idioma y separador

Excel traduce los nombres de las funciones al idioma de la instalación, y el separador de argumentos depende de la configuración regional del sistema. Por eso una fórmula perfectamente correcta copiada de un chatbot puede dar error en tu ordenador.

| En inglés | En Excel en español |
|---|---|
| `SUMIFS` | `SUMAR.SI.CONJUNTO` |
| `COUNTIFS` | `CONTAR.SI.CONJUNTO` |
| `VLOOKUP` | `BUSCARV` |
| `XLOOKUP` | `BUSCARX` |
| `IFERROR` | `SI.ERROR` |
| `EOMONTH` | `FIN.MES` |
| `TRIM` / `PROPER` | `ESPACIOS` / `NOMPROPIO` |
| `IF` / `AND` / `TODAY` | `SI` / `Y` / `HOY` |

- **Separador:** en España y en buena parte de Latinoamérica, donde la coma es el separador decimal, Excel usa **punto y coma** entre argumentos: `=SI(A2>100;"Alto";"Bajo")`. Donde el decimal es un punto, como suele ocurrir en México, se usa la coma. Si no sabes cuál es el tuyo, escribe `=SUMA(` en una celda y mira la ayuda que aparece debajo.
- **Google Sheets** también traduce los nombres de función según la configuración regional de la hoja (**Archivo > Configuración > Configuración regional**), y el separador cambia con ella.
- **La solución es simple:** en cada prompt, di "Excel en español con punto y coma" (o con coma). Si ya te dio la fórmula en inglés, pídele: *"Tradúcela a Excel en español con punto y coma."*

## Paso a paso con un chatbot gratuito

1. **Mira tu hoja y apunta la estructura.** Qué contiene cada columna, en qué fila empiezan los datos (normalmente la 2 si la 1 tiene encabezados) y hasta dónde llegan.
2. **Indica programa, versión, idioma y separador.** "Excel 365 en español con punto y coma", "Excel 2019" o "Google Sheets". Funciones nuevas como `BUSCARX` o `FILTRAR` no existen en versiones antiguas: la propia Microsoft aclara que BUSCARX no está disponible en Excel 2016 ni en Excel 2019.
3. **Describe el resultado, no la fórmula.** "En D2, pon 'Vencida' si la fecha de C2 es anterior a hoy y el estado de E2 no es 'Pagada'." No necesitas saber cómo se llama la función.
4. **Pide una explicación junto con la fórmula.** Así detectas antes si la IA ha supuesto algo que no es.
5. **Pégala primero en una sola celda.** Comprueba el resultado en dos o tres filas que puedas calcular tú, y luego arrastra hacia abajo.
6. **Si da error, pégale el error** junto con la fórmula y unas filas de ejemplo, en el mismo chat, para que la corrija.

## Prompts para copiar

**1. La petición básica**

> Uso [Excel 365 / Excel 2019 / Google Sheets] en español, con [punto y coma / coma] como separador. Mi hoja tiene encabezados en la fila 1 y datos de la fila 2 a la [última fila]. Columnas: A = [qué], B = [qué], C = [qué]. En la celda [celda] quiero [el resultado en palabras normales]. Dame la fórmula con los nombres de función en español, explica cada parte en una línea y dime qué has supuesto sobre mis datos.

**2. Buscar un valor en otra tabla**

> En la Hoja1, la columna A tiene códigos de producto. En una hoja llamada Precios, la columna A tiene los mismos códigos y la columna B los precios. En la columna D de la Hoja1 quiero el precio de cada código, y "No encontrado" si el código no está en Precios. Uso [programa/versión], en español con [separador].

**3. Sumar o contar con condiciones**

> La columna A tiene fechas, la B el nombre del vendedor y la C el importe. En G2 quiero el total de importe del vendedor que escribo en F2, solo de las fechas del mes que pongo en E2 (como fecha, por ejemplo 01/10/2026). Fórmula para [programa/versión] en español con [separador].

**4. Arreglar una fórmula que no funciona**

> Esta fórmula me da [el error, por ejemplo #N/A, #¡VALOR! o un número que no cuadra]: `[pega la fórmula]`. Estas son 5 filas de ejemplo de mis datos, con las letras de columna: [pega las filas]. ¿Qué falla y cuál es la fórmula corregida?

**5. Entender una fórmula que hizo otra persona**

> Explícame esta fórmula paso a paso, como si nunca hubiera usado estas funciones: `[pega la fórmula]`. Después dime qué cosas podrían hacer que dejara de funcionar.

**6. Limpiar texto desordenado**

> En la columna A hay nombres como "  garcía lópez, MARÍA " con espacios de más y mayúsculas mezcladas. En la columna B quiero "María García López". Dame una fórmula para Excel en español con punto y coma, y dime si necesita una versión reciente de Excel.

## Ejemplo: cómo es una buena respuesta

Imagina que pides: "En A hay fechas de pedido y en C importes. En F2 quiero el total de C del mes de la fecha que hay en E2. Excel 365 en español con punto y coma."

Una respuesta correcta sería algo así:

```
=SUMAR.SI.CONJUNTO(C:C; A:A; ">="&FIN.MES(E2;-1)+1; A:A; "<="&FIN.MES(E2;0))
```

`FIN.MES(E2;-1)+1` es el primer día de ese mes y `FIN.MES(E2;0)` el último, así que `SUMAR.SI.CONJUNTO` suma todos los importes cuya fecha cae entre los dos. Una buena respuesta de la IA lo explicará más o menos así. Si no lo hace, pídeselo.

## Copilot o Gemini dentro de la hoja

Los asistentes integrados te ahorran el copiar y pegar porque ven tus columnas, así que puedes referirte a ellas por el nombre del encabezado.

- **Copilot en Excel:** pulsa el botón **Copilot** de la pestaña Inicio y pide, por ejemplo: "Añade una columna con los días entre Fecha de pedido y Fecha de envío". Microsoft incluye la creación de fórmulas entre sus funciones y recomienda revisar y verificar lo que genere. Necesita el libro en un formato moderno como .xlsx y el cálculo en **Automático** (Fórmulas > Opciones de cálculo).
- **Gemini en Google Sheets:** en cualquier celda escribe `=` y describe lo que quieres, o abre el panel de Gemini y pide "Crea una fórmula que divida Goles entre Partidos". Es una función de ordenador, no del móvil.

Si la hoja es de tu empresa o de tu centro de estudios, revisa su política antes de pegar datos en una cuenta personal de un chatbot: muchas organizaciones solo permiten las herramientas de IA que ellas mismas ofrecen.

## Cómo comprobar una fórmula de IA antes de fiarte

Las fórmulas generadas por IA a menudo parecen correctas y fallan sin avisar. Antes de usarlas en serio:

- **Pruébala con filas que puedas calcular tú**, incluido algún caso límite: una celda vacía, un cero, una fecha en el último día del mes.
- **Revisa los rangos.** Una fórmula con `C2:C100` dejará fuera la fila 101 cuando crezcan los datos. Pide referencias a columnas completas o que use una Tabla de Excel.
- **Cuidado con números y fechas guardados como texto.** Los datos importados de un banco o de un programa de facturación suelen traer "01/10/2026" como texto, y entonces las fórmulas de fechas devuelven 0. Pregúntale a la IA cómo convertirlos.
- **Ojo con el formato de fecha.** En España y Latinoamérica se escribe día/mes/año. Si en el prompt pones "10/01/2026", aclara si es 10 de enero o 1 de octubre.
- **No dejes que adivine tu estructura.** Si dice "suponiendo que tus datos están en la columna B" y no es así, corrígela y vuelve a pedirla.

## Preguntas frecuentes

**¿ChatGPT puede hacer fórmulas de Excel gratis?**
Sí. Los planes gratuitos de ChatGPT, Claude y Gemini escriben y explican fórmulas. Solo tienes que copiar el resultado en Excel o Sheets.

**¿Por qué la fórmula que me da la IA dice #¿NOMBRE??**
Casi siempre porque está en inglés (`SUMIFS` en lugar de `SUMAR.SI.CONJUNTO`) o porque usa una función que tu versión de Excel no tiene. Pide la fórmula "en español" e indica tu versión.

**¿Necesito Copilot para usar IA en Excel?**
No. Copilot pone el asistente dentro de Excel, pero a octubre de 2026 requiere un plan de Microsoft 365 compatible. Cualquier chatbot gratuito puede escribir las mismas fórmulas si le describes tu hoja.

**¿Qué pasó con la función =COPILOT?**
Microsoft la retiró el 14 de septiembre de 2026. Los libros que la usaban conservan los resultados guardados, pero muestran `#¿NOMBRE?` al recalcular. Usa el panel de Copilot o sustituye esas celdas por fórmulas normales.

**¿Puedo subir mi Excel a ChatGPT en lugar de describirlo?**
Sí. ChatGPT admite archivos .xls, .xlsx y .csv para análisis de datos, y Claude y Gemini también aceptan archivos. Aun así, para una sola fórmula suele ser más rápido describir las columnas y pegar unas filas de ejemplo, y compartes menos datos.

**¿La IA también escribe macros o Apps Script?**
Sí, puede escribir macros VBA para Excel y Apps Script para Google Sheets. Ejecuta solo código que entiendas o que hayas probado en una copia del archivo, porque una macro puede modificar o borrar datos.

**¿Es seguro pegar mis datos en un chatbot?**
No pegues datos personales o confidenciales que no hagan falta, como DNI, CURP, RUT o cuentas bancarias. Para pedir una fórmula, unas filas inventadas con la misma estructura funcionan igual de bien.

## Fuentes

- [Soporte de Microsoft: ¿Qué es Copilot en Excel? (en inglés)](https://support.microsoft.com/en-us/Excel/copilot/frequently-asked-questions-about-copilot-in-excel)
- [Soporte de Microsoft: función COPILOT (en inglés)](https://support.microsoft.com/en-us/excel/copilot-function)
- [Soporte de Microsoft: función BUSCARX](https://support.microsoft.com/es-es/Excel/functions/xlookup-function)
- [Ayuda de Editores de Documentos de Google: funciones de Gemini en Sheets (en inglés)](https://support.google.com/docs/answer/14218565)
- [Ayuda de Google: idiomas admitidos en Google Workspace con Gemini (en inglés)](https://support.google.com/docs/answer/14925782?hl=en)
- [Centro de ayuda de OpenAI: análisis de datos con ChatGPT (en inglés)](https://help.openai.com/en/articles/8437071-data-analysis-with-chatgpt)
