---
name: planificador-contenidos-b2c
description: Convierte la información de un proyecto de Sommos en un calendario mensual de contenidos B2C para Facebook (fechas, pilares, objetivos, formatos y tema/idea de cada publicación). Usar siempre que el usuario pida un plan, calendario, parrilla o cronograma de contenidos para un producto o proyecto de Sommos (por ejemplo ProAhorro, MetaAhorro o SommosAgro) y un mes concreto, aunque no use la palabra "calendario"; por ejemplo "planifica los contenidos de octubre", "qué publicamos en noviembre" o "arma el plan del mes". No usar para escribir el copy, el guion o el diseño de una pieza, ni para contenido B2B o comercial.
---

# Planificador de Contenidos B2C — Sommos

Este skill transforma la información de un proyecto de Sommos en un **calendario mensual de contenidos B2C**. Para cada publicación define: cuándo sale, en qué canal, con qué objetivo, dentro de qué pilar, en qué formato y qué idea debe desarrollarse.

El skill **planifica, no produce**. El copy, el hook, el guion, el texto de cada lámina, el CTA y los detalles visuales se desarrollan después, en otra etapa.

---

## 1. Antes de empezar

### Contexto del proyecto

El **contexto del proyecto** es la fuente principal de verdad. Está en la carpeta `projects/<nombre-del-proyecto>/` en la raíz del repositorio (por ejemplo, `projects/proahorro/`). Suele incluir producto, aliado o entidad, país, moneda, público, objetivos, beneficios, mecánica, tono, fechas y campañas activas.

1. Identifica el proyecto que menciona el usuario y lee **todos los archivos** de su carpeta.
2. Si el nombre del usuario no coincide exactamente con ninguna carpeta (por ejemplo, "Pro Ahorro" vs. `proahorro`), usa la más parecida solo si es evidente; si hay duda, pregunta.
3. Si la carpeta no existe o está vacía, díselo al usuario y pídele el contexto antes de planificar (puede adjuntarlo o pegarlo en el chat). No lo reemplaces por suposiciones ni uses el de otro proyecto.
4. Si no encuentras la información que necesitas, revisa `projects/README.md`, que explica cómo está organizada la carpeta.

### Solicitud

Necesitas dos datos: **proyecto/producto** y **mes**.

- Si falta el mes, o el producto es ambiguo, pregunta antes de asumir.
- Si piden varios meses, genera un calendario por mes.
- Si no se indica el año, usa el actual, salvo que el contexto diga otro.

### Archivos de referencia

Lee ambos antes de armar el calendario:

- `references/content-pillars-b2c.md`: pilares disponibles y cuándo usar cada uno.
- `references/content-formats-b2c.md`: formatos disponibles y cuándo conviene cada uno.

Usa **únicamente** los pilares y formatos que estén definidos ahí. No los amplíes ni los renombres desde este skill; así, si cambias esos archivos, el skill sigue siendo coherente.

---

## 2. Principios

**Cada proyecto es independiente.** No uses información de otros proyectos de Sommos, aunque parezca similar.

**No inventes datos.** Sommos trabaja con productos financieros, y un beneficio, tasa, monto, promoción, condición, fecha, testimonio o resultado inventado puede tener implicaciones legales y de confianza. Si falta un dato necesario para planificar una publicación, escribe `[VALIDAR]` en la celda correspondiente y agrégalo a "Pendientes de validación".

**El contexto manda.** Si el contexto del proyecto fija frecuencia, canal, tono o cantidad de contenidos, eso prevalece sobre las reglas generales de este skill.

**Calidad sobre cantidad.** No agregues publicaciones solo para llenar el calendario. Cada publicación necesita una razón estratégica.

---

## 3. Frecuencia y canal

**Frecuencia base: 1 contenido B2C por semana**, lo que da entre 4 y 5 publicaciones al mes.

- Cuenta semanas de lunes a domingo. Se planifica una publicación por cada semana que tenga al menos 4 días dentro del mes solicitado.
- Puede haber más publicaciones si el contexto lo justifica: lanzamientos, campañas de duración limitada, promociones, eventos o fechas comerciales relevantes. Indica brevemente la razón.

**Canal por defecto: Facebook.** No incluyas otros canales salvo que el usuario lo pida explícitamente.

---

## 4. Estrategia del mes

Antes de armar la tabla:

1. Revisa el objetivo del proyecto, el público y sus necesidades.
2. Identifica los problemas o necesidades que el producto puede abordar, y los beneficios y características que pueden comunicarse.
3. Selecciona los pilares más relevantes (no hace falta usarlos todos).
4. Distribuye los contenidos con una secuencia lógica. Cuando aplique, combina **educación → necesidad → solución → producto → consideración → conversión**, sin aplicarla de forma rígida.
5. Evita que el calendario sea exclusivamente promocional.

---

## 5. Cómo definir cada publicación

### Objetivo
Para qué existe la publicación. Ejemplos: educar, generar awareness, explicar el producto, mostrar un beneficio, explicar el funcionamiento, resolver una objeción, generar interés, registros o descargas, recordar una acción.

### Formato
Elige del archivo de formatos el que mejor comunique el objetivo y el tema.

### Tema / idea
Funciona como un **brief estratégico breve**: quien desarrolle la pieza debe poder hacerlo sin reinterpretar el objetivo. Debe indicar:

- Qué se quiere comunicar y desde qué enfoque.
- Qué aspecto del producto se pone en contexto.
- Qué debe comprender el usuario.

Debe ser concreta, sin convertirse en el desarrollo de la pieza (sin copy, hook, CTA, número de láminas, escenas ni indicaciones visuales).

| ❌ Demasiado vago | ✅ Brief útil |
|---|---|
| "Beneficios de ProAhorro." | "Explicar cómo ProAhorro puede ayudar a organizar un objetivo de ahorro mediante una planificación anticipada." |
| "Cómo funciona el producto." | "Presentar el funcionamiento general de ProAhorro para que el usuario entienda qué debe hacer para comenzar." |

---

## 6. Fechas

- Todas las fechas deben caer dentro del mes solicitado, en orden cronológico.
- Las fechas específicas del contexto (inicio o cierre de campaña, eventos) tienen prioridad. Planifica también las acciones necesarias antes o después de una fecha importante.
- **Varía los días de la semana** a lo largo del mes en lugar de publicar siempre el mismo día, manteniendo una distribución equilibrada.
- **No inventes fechas importantes.** Usa las del contexto. Si consideras relevante una fecha comercial conocida del país del proyecto (por ejemplo, un Día de la Madre), inclúyela marcada con `[VALIDAR]`.

---

## 7. Estructura de la tabla

Usa **exactamente** estas columnas, sin cambiar nombres, sin agregar ni quitar ninguna (aunque algún campo esté pendiente):

| Fecha | Canal | Pilar | Objetivo | Formato | Tema / idea | Link para la pieza gráfica | Estado |
|---|---|---|---|---|---|---|---|

Cada fila es una publicación. El público, la segmentación y el copy **no** van como columnas: el público sale del contexto y el copy se desarrolla después.

| Columna | Qué poner |
|---|---|
| **Fecha** | `DD/MM/YYYY`, dentro del mes solicitado. |
| **Canal** | `Facebook` (salvo pedido explícito). |
| **Pilar** | Uno de los definidos en `content-pillars-b2c.md`. |
| **Objetivo** | Para qué se hace la publicación. |
| **Formato** | Uno de los definidos en `content-formats-b2c.md`. |
| **Tema / idea** | Brief estratégico (sección 5). |
| **Link para la pieza gráfica** | El enlace real si existe; si no, `Pendiente`. Nunca inventes una URL. |
| **Estado** | Solo `En proceso`, `En revisión`, `Programado` o `Publicado`. Toda publicación nueva empieza en `En proceso`, salvo que el usuario indique otro estado. |

---

## 8. Formato de la respuesta

Presenta primero una síntesis y después el calendario:

```
**Proyecto:** [nombre]
**Producto:** [producto]
**Mes:** [mes y año]
**Objetivo:** [objetivo]
**Canal:** Facebook
**Público:** [público]
**Pilares:** [pilares seleccionados]
```

Luego, la tabla del calendario (sección 7).

Si hay datos por confirmar, cierra con:

```
### Pendientes de validación
- [Dato pendiente]
```

No agregues recomendaciones ni comentarios extra si el usuario solo pidió el calendario.

---

## 9. Ejemplo (ilustrativo)

Los datos son de muestra y no corresponden a ningún proyecto real. Sirve para fijar el nivel de detalle y el tipo de distribución esperados.

Solicitud: *"Haz un plan de contenidos para ProAhorro de octubre."*

| Fecha | Canal | Pilar | Objetivo | Formato | Tema / idea | Link para la pieza gráfica | Estado |
|---|---|---|---|---|---|---|---|
| 02/10/2026 | Facebook | Educación | Educar | Post | Explicar por qué definir una meta concreta de ahorro facilita mantener el hábito, poniendo el foco en la importancia de tener un objetivo claro. | Pendiente | En proceso |
| 06/10/2026 | Facebook | Necesidad y objetivos | Generar interés | Carrusel | Mostrar situaciones cotidianas en las que ahorrar con anticipación evita apuros, para que el usuario se identifique con la necesidad. | Pendiente | En proceso |
| 14/10/2026 | Facebook | Producto y funcionamiento | Explicar el funcionamiento | Reel | Presentar el funcionamiento general de ProAhorro para que el usuario entienda qué debe hacer para comenzar. | Pendiente | En proceso |
| 22/10/2026 | Facebook | Confianza y experiencia | Resolver una objeción | Post | Aclarar una duda frecuente sobre el uso del producto `[VALIDAR: dudas reales del público]`. | Pendiente | En proceso |
| 26/10/2026 | Facebook | Producto y funcionamiento | Generar registros | Carrusel | Recordar el beneficio principal de ProAhorro y cómo empezar, como cierre del mes. | Pendiente | En proceso |

### Pendientes de validación
- Dudas o preguntas frecuentes reales del público para la publicación del 22/10.

---

## 10. Revisión antes de entregar

**Proyecto**
- [ ] La información corresponde al proyecto correcto y no se usaron datos de otros.
- [ ] Se respetan público, tono, moneda y condiciones.
- [ ] No hay beneficios, tasas, promociones ni funcionalidades inventadas.

**Estrategia**
- [ ] Cada publicación tiene un objetivo y una función estratégica.
- [ ] Hay variedad de pilares y formatos, y una secuencia lógica durante el mes.
- [ ] No todo el contenido es promocional.
- [ ] La cantidad de publicaciones está justificada.

**Calendario**
- [ ] Fechas dentro del mes solicitado, en orden cronológico y con días de la semana variados.
- [ ] Pilares y formatos pertenecen a los archivos de referencia.
- [ ] Columnas exactas, canal válido, estados válidos.
- [ ] Links inexistentes como `Pendiente`.
- [ ] Cada tema / idea es claro y no incluye copy ni desarrollo de la pieza.
- [ ] Los `[VALIDAR]` de la tabla aparecen también en "Pendientes de validación".
