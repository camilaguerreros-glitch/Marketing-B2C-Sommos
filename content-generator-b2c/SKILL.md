---
name: generador-contenidos-b2c
description: Desarrolla una pieza de contenido B2C de Sommos (post, carrusel o Reel) a partir de una idea, una fila del calendario B2C o una solicitud directa, entregando hook, estructura, texto de la pieza, copy, CTA y dirección visual según los lineamientos creativos del proyecto, listos para pasar a producción. Usar siempre que el usuario pida escribir, desarrollar o crear un copy, caption, hook, guion, carrusel, Reel o post para un proyecto de Sommos (por ejemplo ProAhorro, MetaAhorro o SommosAgro), o cuando pegue una fila del calendario de contenidos y quiera convertirla en pieza, aunque no diga "generador". No usar para planificar el calendario mensual, ni para contenido B2B o comercial.
---

# Generador de Contenidos B2C — Sommos

Este skill transforma una **idea de contenido B2C** en una pieza desarrollada y lista para producción, usando el contexto específico del proyecto.

**Contexto del proyecto + idea → desarrollo del contenido → pieza lista para producción.**

Es la etapa siguiente al planificador de contenidos: el planificador define *qué comunicar, cuándo y en qué formato*; este skill desarrolla *cómo se dice*.

---

## 1. Antes de empezar

### Contexto del proyecto

Cada proyecto tiene su carpeta en `projects/<nombre-del-proyecto>/` en la raíz del repositorio (por ejemplo, `projects/proahorro/`), con dos archivos que debes leer **siempre** antes de desarrollar una pieza:

- **`PROJECT.md`: contexto del proyecto.** Es la fuente principal de verdad sobre el negocio: producto, aliado o entidad, país, moneda, público, objetivos, beneficios, características, mecánica, tono, canales de conversión y campañas activas.
- **`CREATIVE-GUIDELINES.md`: lineamientos creativos.** Definen la identidad gráfica del proyecto: líneas gráficas, paleta de colores, tipografías y demás criterios visuales de la marca (ver "Lineamientos creativos" más abajo).

1. Identifica el proyecto y lee ambos archivos. Si la carpeta tiene otros, revísalos si son relevantes.
2. Si el nombre no coincide exactamente con ninguna carpeta, usa la más parecida solo si es evidente; si hay duda, pregunta.
3. Si la carpeta no existe o `PROJECT.md` falta, díselo al usuario y pide el contexto (puede adjuntarlo o pegarlo) antes de desarrollar la pieza. No lo reemplaces por suposiciones ni uses el de otro proyecto.
4. Si el contexto fija un tono, lenguaje, formato o lineamiento específico, ese tiene prioridad sobre las reglas generales de este skill.
5. Si no encuentras algo que necesitas, revisa `projects/README.md`, que explica cómo está organizada la carpeta.

### Lineamientos creativos

Cada cliente tiene una identidad distinta, por eso hay un `CREATIVE-GUIDELINES.md` por proyecto. **Todo lo visual de la pieza debe guiarse por el de ese proyecto**: paleta de colores, tipografías, estilo gráfico, uso del logo, tipo de imágenes y personas, y cualquier criterio que el documento defina.

- **Aplica solo lo que el documento dice.** No inventes colores, códigos hex, tipografías ni estilos. Si necesitas un dato visual que el documento no define, escribe `[VALIDAR]`.
- **No mezcles marcas.** Nunca uses los lineamientos de otro proyecto ni un estilo "genérico" de Sommos como reemplazo.
- **Si el proyecto no tiene `CREATIVE-GUIDELINES.md`**, dilo al usuario y desarrolla el contenido de texto igualmente, dejando la dirección visual como `[VALIDAR: lineamientos creativos del proyecto]`.
- **Prioridad:** para lo visual y de producción, mandan los lineamientos del proyecto; donde no digan nada, aplican los lineamientos generales de `resources/Formatos.md` (por ejemplo, personas reales, voz en off y subtítulos en Reels). Si `PROJECT.md` y `CREATIVE-GUIDELINES.md` se contradicen, avísalo y no elijas por tu cuenta.

### Formatos

Antes de desarrollar una pieza, lee `resources/Formatos.md`. Los formatos válidos son **Post, Carrusel y Reel**; sus lineamientos de producción (personas reales, voz en off, subtítulos) están en la sección 5 de ese archivo.

### Pilares

Si la pieza viene de una fila del calendario (o el usuario indica un pilar), lee `resources/Pilares.md` para respetar el enfoque y las precauciones del pilar: por ejemplo, en Producto y funcionamiento los beneficios y condiciones salen solo del contexto, y en Confianza y experiencia no se usan testimonios ni cifras que no estén documentados.

### Tipos de contenido

Si el usuario pide un **testimonio** o un **tutorial**, no son formatos sino tipos de contenido: desarrollarlos dentro de un Post, Carrusel o Reel (ver sección 5).

---

## 2. Qué recibe el skill

**A. Una idea de contenido.** Ejemplo: *"Quiero un carrusel para explicar cómo ProAhorro ayuda a organizar una meta de ahorro."*

**B. Una fila del calendario B2C** (Fecha, Canal, Pilar, Objetivo, Formato, Tema / idea). Úsala como base: respeta el objetivo, el formato y el enfoque del tema / idea.
- Si la fila trae `[VALIDAR]`, mantenlo y repórtalo al final.
- Si el tema / idea choca con el contexto del proyecto, dilo y propón cómo ajustarlo antes de desarrollar.
- Si recibes varias filas, desarrolla cada una en orden y mantén coherencia entre ellas; si son muchas, pregunta si quiere todas o algunas.

**C. Una solicitud directa.** Ejemplos: *"Haz un Reel sobre…"*, *"Dame un copy para…"*. Usa el contexto del proyecto y las instrucciones del usuario.

Si no se indica el formato, elige el más adecuado según el archivo de formatos y menciónalo en una línea.

---

## 3. Principios

**No inventes datos.** Sommos trabaja con productos financieros: un beneficio, tasa, monto, promoción, condición, fecha, funcionalidad, dato, estadística, testimonio, caso de éxito o resultado inventado puede tener implicaciones legales y de confianza. Si falta información necesaria, escribe `[VALIDAR]` en el punto exacto del texto y agrégalo a "Pendientes de validación".

**Prudencia con las promesas.**
- No transformes una característica en un beneficio que no esté validado.
- No conviertas una posibilidad en una promesa.
- No presentes resultados como garantizados si el contexto no los respalda.
- Si el contexto incluye textos legales, condiciones o avisos obligatorios, inclúyelos donde corresponda.

**Cada pieza debe** tener un mensaje central claro, responder al objetivo, ser relevante para el público, mantener el tono del proyecto y usar solo información validada.

**Claro, natural y fácil de entender.** Evita el lenguaje corporativo, técnico o artificial cuando no corresponda al público. No asumas conocimientos financieros o del producto que el público probablemente no tiene; si un concepto es complejo, explícalo de forma sencilla. Adapta el lenguaje al país, la moneda y la etapa del usuario.

**Sin relleno.** No agregues información solo para alargar la pieza ni elementos que el usuario no pidió.

---

## 4. Copy, CTA y hooks

### Copy / caption
- Complementa la pieza visual; no repite todo lo que aparece en ella.
- Mantiene el tono del proyecto y habla al público correspondiente.
- Las primeras líneas deben sostener el mensaje central, porque es lo primero que se lee.
- Emojis, hashtags y estilo siguen los lineamientos del contexto; si no hay, mantén un uso sobrio.

### CTA
- Debe corresponder al objetivo de la publicación y a una acción que el usuario **realmente pueda hacer**.
- Usa los **canales de conversión del contexto** (app, formulario, agencia, etc.). Si el contexto no los indica, escribe `[VALIDAR: canal de conversión]`.
- Nunca inventes enlaces, URLs ni acciones que el producto no permite.
- Ejemplos de tipo de CTA (solo si aplican al proyecto): conocer más, descubrir cómo funciona, registrarse, descargar la app, configurar una meta, acercarse a una agencia.

### Hook
- Capta la atención y se relaciona directamente con el contenido. Puede ser una pregunta, un problema, una situación cotidiana, un beneficio validado, una afirmación o una idea que genere curiosidad.
- Sin exageraciones que no puedan sustentarse.
- Por defecto entrega **una** propuesta clara. Ofrece **hasta 3 opciones** de hook o CTA cuando el usuario las pida o cuando el hook sea decisivo (por ejemplo, en un Reel).

---

## 5. Desarrollo según el formato

El formato define la estructura. No uses una estructura rígida para todos.

### Post
Concepto · texto de la pieza (breve, si corresponde) · copy / caption · CTA.
La cantidad de texto se adapta al objetivo y al diseño.

### Carrusel
Concepto · hook o portada · estructura y texto de cada lámina · cierre · copy / caption · CTA.
La cantidad de láminas depende de la información necesaria; no hay un número fijo. Organiza el contenido **por lámina**.

### Reel
Concepto · hook · estructura · escenas o momentos principales · texto en pantalla · voz en off · copy / caption · CTA.
Siguiendo los lineamientos de formatos: prioriza **personas reales**, usa **voz en off** para desarrollar el mensaje y prevé **subtítulos** durante todo el Reel. Estructura clara, duración acorde al contenido y recursos visuales que refuercen el mensaje. Organiza el contenido **por escena o momento**.

### Testimonio (dentro de un Post, Carrusel o Reel)
Idea central · estructura · preguntas sugeridas para recoger el testimonio · texto de apoyo · copy · CTA.
**No inventes testimonios ni atribuyas declaraciones a personas reales.** Trabaja solo con testimonios que el usuario o el contexto aporten; si falta el material, `[VALIDAR]`.

### Tutorial (dentro de un Carrusel o Reel)
Objetivo · introducción · pasos · texto de apoyo · cierre · copy · CTA.
Los pasos se basan **únicamente** en funcionalidades o procesos confirmados del producto.

### Texto de la pieza vs. copy
Cuando haya texto dentro de una pieza gráfica, sepáralo claramente del copy / caption:
- **Texto de la pieza:** breve, fácil de leer, jerarquizado y compatible con el formato. No llenes las piezas de texto.
- **Copy / caption:** complementa; no duplica.

---

## 6. Estructura de salida

Adapta la respuesta al formato y a lo que se pidió; no es obligatorio usar todas las secciones. Estructura general:

```
### Concepto
[Descripción breve de la idea.]

### Objetivo y formato
[Objetivo de la pieza y formato.]

### Hook
[Hook principal.]

### Desarrollo
[Contenido estructurado según el formato: láminas, escenas, pasos…]

### Texto para la pieza
[Texto que aparecerá dentro de la pieza, cuando corresponda.]

### Dirección visual
[Indicaciones visuales tomadas de CREATIVE-GUIDELINES.md del proyecto: paleta, tipografía, estilo, personas o imágenes, uso del logo. Solo lo que el documento define; lo que falte, [VALIDAR].]

### Copy
[Copy o caption.]

### CTA
[CTA.]

### Pendientes de validación
- [Dato pendiente]
```

Reglas según lo solicitado:
- Si piden **solo un copy**, entrega solo el copy y lo necesario (CTA).
- Si piden **varias alternativas**, entrega las solicitadas.
- Si piden **una pieza gráfica**, entrega el contenido que debe aparecer en ella y su dirección visual.
- La **Dirección visual** debe ser breve y referirse a los lineamientos del proyecto (por ejemplo, "usar la paleta principal", "tipografía de títulos según el documento"); no repitas el documento completo. En Carruseles y Reels, si algo cambia por lámina o escena, indícalo en el Desarrollo.
- Si el usuario pide solo un copy, omite la Dirección visual.
- Cada `[VALIDAR]` del texto debe aparecer también en "Pendientes de validación". Omite esa sección si no hay pendientes.

---

## 7. Ejemplo (ilustrativo)

Los datos son de muestra y no corresponden a un proyecto real; se usa `[VALIDAR]` donde el contexto no aporta el dato. Muestra el nivel de detalle esperado.

Entrada (fila del calendario):

| Fecha | Canal | Pilar | Objetivo | Formato | Tema / idea |
|---|---|---|---|---|---|
| 02/10/2026 | Facebook | Educación | Educar | Carrusel | Explicar por qué definir una meta concreta de ahorro facilita mantener el hábito. |

Salida:

**Concepto:** una meta clara convierte "quiero ahorrar" en un plan concreto.
**Objetivo y formato:** educar · Carrusel.
**Hook (portada):** "¿Ahorrar sin saber para qué? Así es más difícil".

**Desarrollo:**
- Lámina 1 (portada): el hook.
- Lámina 2: ahorrar "sin más" suele quedarse en buenas intenciones.
- Lámina 3: una meta concreta (qué, cuánto, para cuándo) da dirección al ahorro.
- Lámina 4: ejemplo cotidiano: comparar "quiero ahorrar" con "quiero juntar [VALIDAR: monto y moneda de ejemplo] para [objetivo]".
- Lámina 5 (cierre): definir tu meta es el primer paso.

**Dirección visual:** aplicar la paleta, tipografías y estilo gráfico definidos en `CREATIVE-GUIDELINES.md` del proyecto [en este ejemplo no se detallan por ser ilustrativo]; un solo mensaje por lámina.

**Copy:** "Ahorrar es más fácil cuando sabes para qué. Empieza por ponerle nombre y fecha a tu meta. ¿Cuál es la tuya?"
**CTA:** [VALIDAR: canal de conversión y acción disponible para el usuario].

### Pendientes de validación
- Monto y moneda del ejemplo de la lámina 4.
- Canal de conversión y acción para el CTA.

---

## 8. Revisión antes de entregar

**Contexto**
- [ ] Corresponde al proyecto correcto y no se mezclaron datos de otros.
- [ ] Se respetaron público, tono, moneda, condiciones y lineamientos.
- [ ] La dirección visual sigue el `CREATIVE-GUIDELINES.md` del proyecto correcto, sin colores, tipografías ni estilos inventados ni de otras marcas.

**Contenido**
- [ ] Hay un mensaje central claro y responde al objetivo (y al tema / idea, si vino de una fila).
- [ ] El formato es Post, Carrusel o Reel y está bien desarrollado (por lámina o por escena).
- [ ] Reel: personas reales, voz en off y subtítulos previstos.
- [ ] El copy complementa la pieza y el CTA es una acción real del producto.
- [ ] No hay datos, testimonios, promesas ni URLs inventados.
- [ ] Los datos faltantes están como `[VALIDAR]` y listados al final.

**Producción**
- [ ] El texto de la pieza es breve y claro, sin exceso de texto.
- [ ] La entrega está organizada de forma útil para quien produce.
