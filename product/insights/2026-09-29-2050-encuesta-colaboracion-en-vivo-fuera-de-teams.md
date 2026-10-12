---
date: 2026-09-29
source: survey
survey_design: product/surveys/2026-09-23-1944-colaboracion-en-vivo-fuera-de-teams.md
results: product/surveys/2026-09-26-1800-respuestas-colaboracion-en-vivo-fuera-de-teams.csv
n: 215 calificados (187 trabajaron en herramienta externa · 28 «En ninguna»)
opportunity: trabajo-en-vivo-fuera-de-teams
---

# Análisis de la encuesta: trabajo colaborativo fuera de Teams

- **Diseño de la encuesta:** `product/surveys/2026-09-23-1944-colaboracion-en-vivo-fuera-de-teams.md`
- **Resultados:** `product/surveys/2026-09-26-1800-respuestas-colaboracion-en-vivo-fuera-de-teams.csv` (respuestas del 23/09 12:39 al 25/09 09:39)
- **n:** 249 registros → 34 descalificados en el filtro → **215 califican** (210 completas + 5 parciales). De los 215, **187** trabajaron en una herramienta externa (Q1 ≠ «En ninguna») y **28** no.
- **source:** survey

## Denominador y límites (todo lo que sigue los hereda)

| Canal | Entraron | Descalificados | Califican | Alcance | Tasa de respuesta |
|---|---|---|---|---|---|
| email (organizadores del segmento) | 85 | 8 | 77 (76 completas + 1 parcial) | unknown (el diseño lo deja «a confirmar») | no calculable |
| panel B2B | 164 | 26 | 138 (134 completas + 4 parciales) | 150 (cuota comprada) | 134 completas = 89% de la cuota |

**Meta de n del diseño vs. lo logrado**
- ≥150 que trabajaron afuera: **187** ✓ (email 66 · panel 121).
- ≥30 por canal: ✓ (77 y 138).
- ≥30 que **no** trabajaron afuera («En ninguna»): **28** ✗ (email 11 · panel 17). **Ese segmento es direccional**, y el corte por canal dentro de él lo es doblemente.

**Límites que pesan sobre las conclusiones**
- **Autoselección.** Respondieron personas a quienes una encuesta sobre «trabajo fuera de Teams» les resultó relevante o que cobran incentivo (panel). Los porcentajes describen esta muestra, no el segmento.
- **Firmografía sin verificar.** En el email la garantiza la lista (100+ licencias); en el panel es autodeclarada. Ninguno de los dos canales separa cuentas medianas (100–1.000) de grandes, y las creencias #5 y #6 hablan de cuentas medianas.
- **Q1 está en tramos**, no en conteos: «menos de la mitad» no permite ubicar el umbral de 1 de cada 3.
- **Q2–Q9 refieren a «la última reunión»**: recuerdo de un solo caso por persona, no frecuencia.
- **El n por pregunta varía** (parciales y «No lo sé»); se indica en cada cifra. Los «No lo sé» se excluyen de los porcentajes de Q6, Q7 y Q8, salvo que se diga otra cosa.
- **Calidad de datos:** no hay filas duplicadas. Hay tres pares de textos abiertos casi idénticos entre respondentes distintos (R-077/R-196, R-207/R-224, R-046/R-170), pero con respuestas cerradas distintas; se mantienen y ninguno mueve una cifra. Duración mediana: ~4 minutos.

## Primero, la muestra: diferencias entre canales

Antes de leer segmentos hay que leer canales. Comparación exploratoria (test exacto de Fisher, 16 comparaciones, **sin corrección por comparaciones múltiples**: con 16 pruebas, alguna sale con p<0,05 por azar; solo la primera es robusta).

| Medida | email | panel | p |
|---|---|---|---|
| Aproximadamente la mitad o más de las reuniones con trabajo afuera (Q1) | 47% (36/77) | 69% (95/138) | 0,002 |
| El tablero/documento ya existía antes de la reunión (Q4) | 42% (28/66) | 60% (72/121) | 0,03 |
| Acepta una conversación de 30 min (R3) | 25% (19/76) | 43% (58/134) | 0,01 |
| «No sabía que existía» el resumen de IA en Teams (Q10) | 5% (4/76) | 16% (22/134) | 0,02 |
| Trabajó afuera al menos alguna vez (Q1) | 86% | 88% | 0,68 |
| Enlace pegado en el chat (Q3) | 55% | 54% | 1,0 |
| Tardaron ≥5 min en entrar (Q6) | 29% | 30% | 1,0 |
| Al menos 1 participante no logró entrar (Q7) | 52% | 52% | 1,0 |
| Reunión con externos (Q8) | 19% | 25% | 0,36 |
| Decisión sin registro (Q9) | 25% | 24% | 1,0 |
| Usó Jira, Confluence o un dashboard (Q2) | 45% | 46% | 1,0 |
| Usó una herramienta tipo pizarra (Q2) | 38% | 35% | 0,75 |

**Lectura:** la *forma* de los hallazgos es la misma en los dos canales (cuánta gente sale, cuánto tarda, cuántos quedan afuera, qué se pierde al cierre). Lo que cambia es la *intensidad*: el panel (Engineering/Product Managers de tecnología) trabaja afuera con más frecuencia y más con herramientas ya existentes, y acepta más entrevistas (incentivo). El email es el canal más cercano al usuario real de Teams, pero es canal propio y sobrerrepresenta a los conformes. **Cuando el nivel importe, se citan ambos canales y se usa el email como cota conservadora.**

## O1 · Origen del artefacto

**Qué creíamos.** Que el tablero o documento externo se crea para la reunión. Si mayormente preexiste, el problema es de integración con los sistemas donde ya vive el trabajo, no de colaboración en vivo (decisión del diseño).

**Qué muestran los datos** (Q4, n=187):

| El tablero o documento… | n | % |
|---|---|---|
| ya existía y se siguió usando | 95 | 51% |
| ya existía y no se volvió a usar | 5 | 3% |
| se creó para la reunión y se siguió usando | 45 | 24% |
| se creó para la reunión y no se volvió a usar | 29 | 16% |
| no lo sé | 13 | 7% |

Mayormente preexiste (53%; 57% sin contar «No lo sé»; email 42%, panel 60%). Pero el promedio esconde dos poblaciones, separadas por el tipo de herramienta (Q2):

- **64% (120/187) trabajó solo en herramientas donde el trabajo ya vive** (Google Docs, Jira, Confluence, dashboards, Notion, otras): **72% preexistía** (86/120).
- **36% (67/187) usó al menos una herramienta tipo pizarra** (Miro, Mural, FigJam, Lucidspark, Slido/Mentimeter): **solo 13% preexistía** (9/67); **82% se creó para la reunión** (55/67) y en 54% (36/67) se siguió usando después.

Herramientas (Q2, n=187, opción múltiple): Google Docs/Sheets/Slides 33% · Jira u otro gestor 28% · Miro 19% · dashboard 17% · Confluence 14% · FigJam 12% · Notion 11% · Slido/Mentimeter 10% · Mural 9% · Lucidspark 4% · otra 5%.

**Cómo llegaron** (Q3, n=187): enlace pegado en el chat 54% · ya la tenían abierta 21% · compartí pantalla y cada uno la abrió por su cuenta 16% · la abrí como app dentro de Teams **8%** (15) · otro (correo) 1%. **El 46% no pasó por un enlace en el chat**: la telemetría (29% de reuniones grandes con enlace externo) ve solo un camino y probablemente subestima el fenómeno.

**Decisión que sigue.** La creencia se divide en dos problemas que no admiten una sola solución: (a) **integración** con donde ya vive el trabajo, que es la mayoría del uso externo; (b) **colaboración en vivo sobre un tablero nuevo**, que es la minoría pero donde el artefacto sí nace en la reunión. Tratar todo como «pizarra en Teams» resuelve solo (b).

## O2 · Costo de acceso

**Qué creíamos.** Que entrar a la herramienta cuesta más de 5 minutos y deja gente afuera; si la fricción se concentra en reuniones con externos, es de otro segmento (decisión del diseño).

**Qué muestran los datos**
- **Tiempo hasta que todos estuvieron dentro** (Q6, n=173): <1 min 20% · 1–2 min 29% · 3–4 min 21% · 5–9 min 23% · ≥10 min 6%. **≥5 min: 29% (51/173).**
- **Participantes que siguieron mirando la pantalla de otro** (Q7, n=178): ninguno 48% · 1: 28% · 2–3: 19% · ≥4: 6%. **Al menos uno: 52% (93/178).**
- **Reuniones con externos** (Q8, n=178): 23% (41).

**Corte por externos** (Q6 n=166, Q7 n=172)

| | ≥5 min en entrar | ≥1 quedó afuera |
|---|---|---|
| Con externos | 64% (25/39) | 65% (26/40) |
| Sin externos | 19% (24/127) | 48% (63/132) |

**Corte por origen del artefacto y externos** (≥5 min en entrar; n=154, celdas chicas → direccional)

| | Sin externos | Con externos |
|---|---|---|
| Ya existía | **4%** (3/68) | 52% (11/21) |
| Creado para la reunión | 41% (20/49) | **75%** (12/16) |

**Corte por tipo de herramienta:** pizarra ≥5 min 49% (31/63) vs. resto 18% (20/110); ≥1 quedó afuera 71% (44/62) vs. 42% (49/116).

**Decisión que sigue.**
1. **El umbral de 5 minutos no es la condición general** (29%). Se cumple en dos situaciones: tableros nuevos (41% incluso sin externos) y reuniones con externos (52–75%).
2. **La fricción de los externos existe pero no explica todo**: 25 de los 49 casos lentos tienen externos (51% vs. 23% de base). La otra mitad es interna.
3. Para el Team Lead que conduce reuniones internas con herramientas ya existentes, **casi no hay problema de entrada (4%)**. Diseñar para el tablero nuevo; tratar a los externos como un corte propio, no descartarlo ni ponerlo primero.
4. Aun sin externos, **casi la mitad de las reuniones (48%) tiene a alguien mirando la pantalla de otro**: un problema de participación que el tiempo de entrada no capta.

## O3 · Qué se hace afuera y dónde queda la decisión

**Qué creíamos.** Que lo que se hace afuera es votar, priorizar, editar, revisar datos y registrar acuerdos, y que la decisión queda dispersa.

**Qué hace el grupo** (Q5, n=185, opción múltiple; «Otro» 5% → la lista es suficiente): votar o priorizar 39% · editar un documento entre varios 35% · revisar datos y señalar algo 34% · anotar decisiones 32% · aportar ideas 30% · actualizar tareas o tickets 25% · agrupar ideas 23% · dibujar un diagrama 14%.
Depende del tipo de herramienta: en **pizarras** dominan aportar ideas (58%), agrupar (54%) y votar (52%); en **Docs/Jira/dashboards**, revisar datos (53%), actualizar tareas (40%) y editar (40%).

**Dónde quedó lo decidido** (Q9, n=182, opción múltiple): no quedó registrado en ningún lado **24%** · chat fuera de Teams (Slack, WhatsApp) **23%** · Jira u otro gestor 23% · **Otro 18%** · misma herramienta externa 15% · chat o notas de la reunión de Teams 13% · documento de actas 12% · correo 10% · no se tomaron decisiones 7%.

**«Otro» supera el 15%** que fijó el diseño: la lista de Q9 está incompleta. De las 32 respuestas de «Otro», **26 (14% de los 182) son el resumen, recap, transcripción o grabación de Teams/Copilot**, una opción que faltaba. En **12 de esas 26** la persona agrega una salvedad, por ejemplo: «En el recap de Copilot, que resume todo pero no distingue lo decidido» (Q9, «Otro»; en Q11 lo dicen también R-109, R-149 y R-153); «En el resumen de IA, que nadie leyó»; «En la grabación, se supone».

**Lo más difícil para trabajar juntos y decidir** (Q11, n=95, opcional; menciones, una respuesta puede tener más de un tema):

| Tema | Menciones | % de 95 |
|---|---|---|
| **T1 · Cierre y seguimiento de decisiones** (acuerdos sin dueño, sin registro, «el por qué se pierde», resumen de IA que no distingue lo decidido) | 22 | 23% |
| **T2 · Continuidad entre reuniones** (encontrar lo trabajado antes, retomar) | 15 | 16% |
| T9 · Tiempo, cantidad de reuniones y logística (husos, idioma) | 13 | 14% |
| **T5 · La pizarra nativa no alcanza** (sin votación ni plantillas, lenta con más de 8, no se encuentra después) | 12 | 13% |
| T8 · Participación y dinámica (callados, cámaras apagadas, atención) | 12 | 13% |
| **T4 · Converger, priorizar y votar** | 10 | 11% |
| T6 · Acceso a la herramienta (externos, permisos, SSO, no la ven en el chat) | 9 | 9% |
| **T3 · Trabajo invisible posterior** (pasar a mano del tablero a Jira, escribir el acta) | 5 | 5% |
| T7 · Compliance, seguridad o licencias que limitan lo externo | 4 | 4% |
| Otros / nada en particular / desconocía lo nativo | 3 + 3 + 1 | 7% |

T1 + T2 + T3 (**lo que pasa después de la reunión o entre reuniones**): 36 respuestas, **38%**. Converger/votar y pizarra nativa (T4 + T5, sin doble conteo) suman 20 respuestas, 21%.

> «Después de la planning me paso casi una hora pasando lo del FigJam a Jira. Y hay gente que nunca entra al tablero» — R-024
> «Que quede registro del por qué decidimos algo. El qué queda en Jira, el por qué se pierde en un hilo» — R-224
> «Arme una retro en la whiteboard de Teams y a la semana siguiente no la pude encontrar para continuar. Volvimos a Miro» — R-089
> «Con la agencia externa perdemos 5 o 10 minutos solo en que entren al FigJam» — R-072
> «Aqui compliance no nos deja meter datos de clientes en Miro, asi que o lo hacemos en Teams o no se hace. Y en Teams cuesta» — R-190

**Quienes no salen** (Q12, n=16 de 28 «En ninguna»; direccional): 5 lo resuelven hablando (levantan la mano, comentarios en voz alta; 2 dejan una nota en el chat o en OneNote) · 2 comparten pantalla un Excel y escriben lo que dicen · 2 votan con reacciones o Forms en el chat · 2 preparan por correo antes · 2 usan la pizarra o las notas de Teams · **2 lo hacen por compliance, no por preferencia** (R-009, R-143) · 1 dice que no hace falta.

**Decisión que sigue.** Cualquier solución tiene que cubrir votar/priorizar y agrupar en vivo, pero el hallazgo mayor es otro: **la decisión se pierde después de la reunión** (24% sin registro, 23% en Slack/WhatsApp, y el recap de IA existente no distingue decisión de conversación). Es la oportunidad adyacente que la framing dejó fuera («reuniones sin cierre de decisiones y responsables»), y en Q11 pesa tanto como las capacidades en vivo.

## O4 · Conocimiento y uso de lo nativo

**Qué creíamos.** Que salen porque lo nativo no cubre la necesidad, no por desconocimiento (creencia #2).

**Qué muestran los datos** (Q10, n=210)

| Función | No sabía que existía | Sé que existe, nunca la usé | La usé y la dejé | La uso en algunas | La uso en la mayoría | De los que la probaron, la dejó |
|---|---|---|---|---|---|---|
| Whiteboard | 8% (17) | 27% (57) | **43%** (91) | 17% (36) | 4% (9) | **67%** (91/136) |
| Notas de la reunión (Loop) | **31%** (65) | 28% (59) | 14% (29) | 20% (41) | 8% (16) | 34% (29/86) |
| Apps de otras herramientas en la reunión | **40%** (85) | 28% (58) | 9% (19) | 18% (38) | 5% (10) | 28% (19/67) |
| Resumen o asistente de IA | 12% (26) | **39%** (81) | 13% (27) | 22% (47) | 14% (29) | 26% (27/103) |

- **Whiteboard: no es desconocimiento, es abandono.** La conoce el 92%; **dos de cada tres que la probaron la dejaron**. Sostiene la creencia #2 para esta función. Motivos (Q11, texto libre): sin votación ni plantillas, lenta con más de 8 editores, difícil de abrir en medio de la reunión, y «a la semana no sé dónde está».
- **Notas y apps en Teams: desconocimiento alto** (31% y 40%). Solo el 8% abrió la herramienta como app dentro de la reunión (Q3). Parte de lo que se hace afuera **no se sabe que puede hacerse adentro**.
- **IA:** se conoce (12% no sabía) pero el 39% nunca la usó; tres respuestas de Q11 (R-109, R-149, R-153) dicen que el resumen no distingue lo decidido de lo conversado.
- Entre quienes no salen nunca (n=28), el perfil es igual: 50% dejó la Whiteboard. **El conocimiento de lo nativo no distingue a quienes salen de quienes no.**
- Diferencia de canal: IA «no sabía que existía» 5% (email) vs. 16% (panel).

**Decisión que sigue.** Separar «no me sirve» de «no sé que existe» **por función**: Whiteboard es «no me sirve»; apps y notas son en buena parte «no sé que existe». La segunda mitad admite soluciones de descubrimiento, no de construcción.

## Cortes por región

España (n=27, direccional): 81% (22) trabajó afuera y 63% (17) en aproximadamente la mitad o más; 48% (13) no sabía que existen las apps en Teams. Sin diferencia visible respecto del resto. Una respuesta cita la normativa europea como límite de lo externo (R-173). No hay n para separar más países.

## Insights (priorizados por impacto)

## 1. Son dos problemas con un mismo síntoma: el 64% trabaja donde el trabajo ya vive; solo el 36% usa tableros nuevos

El trabajo afuera es mayoritario (87% lo hizo alguna vez; 61% en aproximadamente la mitad o más de sus reuniones; email 47%, panel 69%), pero el 64% ocurre en Docs, Jira, Confluence y dashboards que ya existían (72% preexistía), mientras que en las pizarras el 82% se crea para la reunión. Implica no tratar «pizarra en Teams» como respuesta única: la mayoría del uso externo pide traer ese trabajo a la reunión, no reemplazarlo.

> Evidence: Q4 según tipo de herramienta: 72% preexistente en herramientas donde el trabajo vive (86/120) vs. 13% en pizarras (9/67). — encuesta, n=187

## 2. Lo que se pierde es la decisión: 38% de lo más difícil ocurre después o entre reuniones, y el 24% no la registra

Q11 pone en primer lugar el cierre y seguimiento de decisiones (23%), seguido por la continuidad entre reuniones (16%). Q9: 24% sin registro, 23% en Slack o WhatsApp, y 14% en el recap o la transcripción de Teams/Copilot, con salvedades en 12 de 26. Implica evaluar como oportunidad propia el cierre de decisiones con responsables (hoy «adyacente, no enmarcada»), con un requisito concreto: distinguir lo decidido de lo conversado.

> Evidence: «El resumen automático sirve para saber de qué se habló pero no para saber qué quedó decidido, lo tengo que corregir siempre» — R-149

## 3. La Whiteboard nativa se conoce y se abandona: 2 de cada 3 que la probaron la dejaron, y votar/priorizar es lo que más se hace afuera

Q10: 92% la conoce, 43% la dejó. Votar o priorizar es la actividad #1 en Q5 (39%; 52% en pizarras). Los motivos abiertos son concretos: sin votación ni plantillas, lenta con más de 8 editores, y no encontrarla a la semana. Implica que cualquier alternativa nativa necesita, como mínimo, votar/agrupar, rendir con 8+ editores y **persistir en un lugar fijo**; sin eso repite el abandono.

> Evidence: «Probamos la whiteboard de Teams hace un tiempo, no tenia plantillas ni votacion y a la retro siguiente no la encontramos. Desde ahi todo en Miro» — R-113

## 4. La fricción de entrada se concentra en tableros nuevos y en reuniones con externos; con herramientas ya existentes casi no hay

≥5 min en entrar: 4% (ya existía, sin externos) vs. 41% (creado para la reunión, sin externos) vs. 52–75% (con externos). El promedio (29%) no representa a ninguno de los grupos. Aun sin externos, el 48% de las reuniones tiene a alguien mirando la pantalla de otro. Implica diseñar el acceso para el tablero nuevo y separar el segmento de externos.

> Evidence: «Con la agencia externa perdemos 5 o 10 minutos solo en que entren al FigJam» — R-072

## 5. Parte de lo que se hace afuera es descubrimiento: el 40% no sabía que hay apps de terceros dentro de la reunión, y solo el 8% las usó así

Es un hallazgo de acceso a lo que ya existe: 31% no sabía de las notas de reunión (Loop). Debilita la parte «no por desconocimiento» de la creencia #2 para apps y notas, aunque la sostiene para Whiteboard. Implica una línea de bajo costo (mostrar lo que ya existe en el flujo de la reunión) que se puede probar antes de construir.

> Evidence: «No sabia que Teams tenia notas de reunion hasta que alguien las abrio de casualidad. Estaban ahi y nadie las usaba» — R-040

## Lo que la encuesta no midió (y qué preguntas quedan para entrevistas)

Una encuesta dice qué, no por qué. Candidatos a entrevista:
1. **¿Cuánto tiempo pierde quien conduce consolidando después?** No se preguntó: la mitad de la creencia #6 (≥1 h/semana) sigue sin medición. Solo dos respuestas dan magnitud: «casi una hora» tras una planning (R-024) y «media hora» por reunión (R-050).
2. **¿Por qué se abandona la Whiteboard?** Qué momento dispara la vuelta a Miro (¿votación, plantillas, rendimiento, no encontrarla?).
3. **¿Por qué el 24% no registra la decisión?** Falta de dueño, de herramienta o de costumbre.
4. **¿Por qué no salen los 28 de «En ninguna»?** Compliance (2 de 16 lo dicen), reuniones solo informativas o costo de la herramienta.
5. **¿Cómo se descubre lo nativo?** Qué haría que alguien encontrara las apps y notas en Teams.
6. **¿Por qué el email trabaja afuera con menos intensidad que el panel (47% vs. 69%)?** ¿Es el sesgo del canal propio, o son dos poblaciones distintas?
7. **Creencia #5 e IT:** la encuesta no habló con IT. Seis respuestas (Q11 y Q12) mencionan compliance, seguridad, normativa o licencias como límite a lo externo (R-009, R-126, R-143, R-173, R-183, R-190), lo que sugiere que en algunas cuentas «afuera» está vetado; falta la ronda de IT del plan de investigación.

## Pool de reclutamiento (opt-in)

77 respondentes aceptaron una conversación (R3). Se excluyen 6 que administran M365/Teams (IT, entrevistados en otra ronda) y 9 que conducen 0–1 reuniones grandes por semana (2 coinciden): **64 candidatos**, 58 con contacto (email 16, panel 48). El contacto está en el CSV, no se copia acá.

Etiquetado según la regla del diseño: **contradice** si Q1 «En ninguna», Q4 «Ya existía…» o Q6 «<3 min»; **confirma** si no tiene ninguna. 17 con 2 señales, 30 con 1, 17 que confirman. Advertencia: «Q4 ya existía» es el patrón mayoritario (53%), así que la etiqueta pesa menos que «En ninguna» o dos señales juntas. Primero los que contradicen con 2 señales.


| Respondente | Canal | Perfil | Señales | Reuniones >5/sem | Contacto |
|---|---|---|---|---|---|
| R-036 | email | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | sí |
| R-131 | email | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | sí |
| R-180 | email | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | sí |
| R-057 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | sí |
| R-094 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | sí |
| R-102 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | sí |
| R-128 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | sí |
| R-144 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | sí |
| R-151 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | sí |
| R-176 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | sí |
| R-224 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 4 o más | sí |
| R-229 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 4 o más | sí |
| R-234 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 4 o más | sí |
| R-235 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | sí |
| R-240 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | sí |
| R-247 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | sí |
| R-194 | panel | Contradice (2 señales) | Q4 «ya existía», Q6 <3 min | 2 o 3 | no |
| R-009 | email | Contradice (1 señal) | Q1 «En ninguna» | 2 o 3 | sí |
| R-013 | email | Contradice (1 señal) | Q6 <3 min | 2 o 3 | sí |
| R-042 | email | Contradice (1 señal) | Q4 «ya existía» | 2 o 3 | sí |
| R-046 | email | Contradice (1 señal) | Q1 «En ninguna» | 2 o 3 | sí |
| R-135 | email | Contradice (1 señal) | Q1 «En ninguna» | 2 o 3 | sí |
| R-143 | email | Contradice (1 señal) | Q1 «En ninguna» | 4 o más | sí |
| R-153 | email | Contradice (1 señal) | Q1 «En ninguna» | 4 o más | sí |
| R-065 | panel | Contradice (1 señal) | Q4 «ya existía» | 2 o 3 | sí |
| R-074 | panel | Contradice (1 señal) | Q6 <3 min | 2 o 3 | sí |
| R-085 | panel | Contradice (1 señal) | Q1 «En ninguna» | 4 o más | sí |
| R-086 | panel | Contradice (1 señal) | Q4 «ya existía» | 2 o 3 | sí |
| R-088 | panel | Contradice (1 señal) | Q1 «En ninguna» | 2 o 3 | sí |
| R-089 | panel | Contradice (1 señal) | Q6 <3 min | 2 o 3 | sí |
| R-090 | panel | Contradice (1 señal) | Q6 <3 min | 4 o más | sí |
| R-093 | panel | Contradice (1 señal) | Q6 <3 min | 2 o 3 | sí |
| R-120 | panel | Contradice (1 señal) | Q1 «En ninguna» | 2 o 3 | sí |
| R-159 | panel | Contradice (1 señal) | Q4 «ya existía» | 4 o más | sí |
| R-170 | panel | Contradice (1 señal) | Q1 «En ninguna» | 2 o 3 | sí |
| R-171 | panel | Contradice (1 señal) | Q4 «ya existía» | 2 o 3 | sí |
| R-173 | panel | Contradice (1 señal) | Q6 <3 min | 2 o 3 | sí |
| R-196 | panel | Contradice (1 señal) | Q1 «En ninguna» | 4 o más | sí |
| R-201 | panel | Contradice (1 señal) | Q4 «ya existía» | 2 o 3 | sí |
| R-228 | panel | Contradice (1 señal) | Q4 «ya existía» | 2 o 3 | sí |
| R-230 | panel | Contradice (1 señal) | Q6 <3 min | 2 o 3 | sí |
| R-238 | panel | Contradice (1 señal) | Q4 «ya existía» | 4 o más | sí |
| R-242 | panel | Contradice (1 señal) | Q1 «En ninguna» | 4 o más | sí |
| R-244 | panel | Contradice (1 señal) | Q4 «ya existía» | 2 o 3 | sí |
| R-110 | panel | Contradice (1 señal) | Q1 «En ninguna» | 2 o 3 | no |
| R-132 | panel | Contradice (1 señal) | Q4 «ya existía» | 4 o más | no |
| R-227 | panel | Contradice (1 señal) | Q4 «ya existía» | 2 o 3 | no |
| R-006 | email | Confirma | — | 4 o más | sí |
| R-011 | email | Confirma | — | 2 o 3 | sí |
| R-019 | email | Confirma | — | 2 o 3 | sí |
| R-024 | email | Confirma | — | 2 o 3 | sí |
| R-031 | email | Confirma | — | 4 o más | sí |
| R-038 | email | Confirma | — | 2 o 3 | sí |
| R-070 | panel | Confirma | — | 2 o 3 | sí |
| R-077 | panel | Confirma | — | 4 o más | sí |
| R-097 | panel | Confirma | — | 4 o más | sí |
| R-099 | panel | Confirma | — | 2 o 3 | sí |
| R-101 | panel | Confirma | — | 2 o 3 | sí |
| R-103 | panel | Confirma | — | 2 o 3 | sí |
| R-113 | panel | Confirma | — | 4 o más | sí |
| R-204 | panel | Confirma | — | 2 o 3 | sí |
| R-205 | panel | Confirma | — | 2 o 3 | sí |
| R-076 | panel | Confirma | — | 4 o más | no |
| R-245 | panel | Confirma | — | 4 o más | no |

## Contraste con las creencias del overview (aprobado y anotado el 2026-09-29)

- **#6 [opportunity: trabajo-en-vivo-fuera-de-teams] [value]**, primera mitad (≥1 de cada 3 reuniones sale a una herramienta externa): **prometedora, no confirmada.** 87% trabajó afuera alguna vez y 61% en aproximadamente la mitad o más (email 47%, panel 69%); el tramo «menos de la mitad» (26%) no permite ubicar el umbral, la muestra es autoseleccionada y no distingue cuentas medianas. La segunda mitad (≥1 h/semana de consolidación) **no se midió.** No propongo anotarla.
- **#2 [product] [value]** (salen porque lo nativo no cubre, no por desconocimiento): **propongo `weakened`.** Se sostiene para Whiteboard (92% la conoce, 67% de quienes la probaron la dejó), pero el 40% no sabía que existen las apps en la reunión y el 31% las notas.
  - Línea propuesta: `— weakened by product/insights/2026-09-29-2050-encuesta-colaboracion-en-vivo-fuera-de-teams.md (2026-09-29)`
- **#5 (shadow IT, IT quiere eliminarlo)**: **no evaluable** con esta encuesta. Solo hay una señal indirecta: seis respuestas hablan de compliance, seguridad o licencias como límite de lo externo.
- **#1, #3, #4:** la encuesta no las toca.

**Siguiente paso:** `/design-interview` reclutando del pool de arriba, empezando por quienes contradicen con 2 señales y por los «En ninguna».
