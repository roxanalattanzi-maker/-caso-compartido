---
source: secondary
method: web
date: 2026-09-21
question: ¿Hay evidencia de mercado de que (P1) las herramientas de colaboración se compran por fuera del contrato principal y IT quiere consolidarlas; (P2) qué ofrecen los competidores para trabajar juntos en la reunión y dónde fallan las funciones nativas de Teams; (P3) cuánto cuesta el trabajo de reunión fragmentado; (P4) cómo se empaqueta y cobra la colaboración en reunión?
opportunity: trabajo-en-vivo-fuera-de-teams
---

# Research: colaboración en vivo dentro de la reunión — mercado

> Límite de este documento: la evidencia es de **mercado**. No verifica nada sobre los usuarios de Teams ni sobre las cuentas medianas del caso; eso queda para el survey y las entrevistas. Todas las consultas se hicieron el 2026-09-21.

**Los tres hallazgos que cambian decisiones:**

1. **El shadow IT es real, pero la señal es sobre todo de *volumen de apps*, no de gasto.** Según Zylo, las apps pagadas con gastos de empleados son el 45% de las aplicaciones pero apenas el 3,7% del gasto SaaS, y Miro y Notion no figuran entre las 15 más pagadas así. Aun así, cuando Miro se compra por contrato hay desperdicio: el 61% de las licencias no se usa. La creencia #5 se sostiene como "IT quiere consolidar". En cambio, "el ahorro es grande" es más débil de lo que se asumió. Tiene que contrastarse con los datos propios.
2. **Competir con "tener un pizarrón" no alcanza. Lo que hace falta es que funcione en vivo con muchas personas.** Zoom incluye Whiteboard y Docs en todos sus planes, y Google empuja notas y acciones generadas por IA dentro de Meet (110M asistentes en un mes). Microsoft ya incluye Loop, las notas colaborativas con tareas sincronizadas a Planner y Whiteboard en M365 Business Standard y Premium. Aun así, hay quejas públicas de lentitud y cuelgues de Whiteboard en tableros grandes. Esto **apoya la creencia #2** (las nativas no cubren la necesidad, no es que no se conozcan), aunque no la prueba.
3. **La competencia usa la colaboración en reunión como palanca de tier.** Zoom limita Pro a 3 pizarras y da pizarras ilimitadas en Business (USD 13,33 contra 18,33 por usuario al mes). Es un precedente de que "colaboración ilimitada en reunión" puede anclar el valor de un salto de plan, lo que importa para la creencia #1 y la métrica de upgrade a Max.

## Competidores directos

| Producto | Para quién | Qué ofrece en la reunión | Precio (lista) | Qué prueba / qué no prueba |
|---|---|---|---|---|
| **Zoom Workplace** | Pymes a enterprise | Whiteboard, Docs y AI Companion en todos los planes. Pizarras limitadas a 3 en Basic y Pro, ilimitadas en Business o superior [verificado: https://pumble.com/zoom-pricing — 2026-09-21] | Pro USD 13,33, Business USD 18,33 por usuario al mes, anual [verificado: ídem] | Prueba que la colaboración en reunión es un diferenciador de tier. No prueba que las cuentas M365 se vayan a Zoom por esto. |
| **Google Meet / Workspace** | Organizaciones en Google Workspace | "Take notes for me": transcripción, resumen y acciones en Docs, también para reuniones presenciales, de Teams y de Zoom. Más de 110M asistentes en el último mes, con crecimiento de 8,5x interanual (anunciado en Cloud Next, abr-2026) [verificado: https://9to5google.com/2026/04/22/google-workspace-next-2026/ — 2026-09-21] | Desconocido en esta búsqueda | Prueba demanda fuerte de que "lo producido quede registrado" y que Google entra en reuniones de Teams. No prueba demanda de *co-creación* en vivo. |
| **Microsoft (nativo)** | Clientes M365 | Notas colaborativas en la reunión con "Follow-up tasks" sincronizadas a Planner. Solo permiten editar título, responsable y fecha [verificado: https://support.microsoft.com/en-us/loop/manage-your-tasks-from-loop-task-lists-and-collaborative-notes-in-planner — 2026-09-21]. Loop Workspaces pasa a ser un servicio core de M365, ya disponible en Business Standard y Premium (despliegue completo en feb-2026) [verificado: https://blog-en.topedia.com/2026/01/microsoft-is-updating-loop-workspaces-licensing-requirements-making-it-a-core-microsoft-365-service/ — 2026-09-21] | Incluido en la suite | Prueba que la brecha **no es de existencia de la función**. Con 5% de uso de Whiteboard y 8% de notas, el problema es de adopción o de desempeño. |
| **Miro** (alternativa que vive *dentro* de Teams) | Equipos de producto, diseño y operaciones | Tiene app de Teams para usar tableros en reuniones y tabs [verificado: https://miro.com/marketplace/microsoft-teams/ — 2026-09-21] | Starter USD 8, Business USD 16 por usuario al mes; contrato anual mediano de USD 17.450 (n=446 deals, Vendr) [verificado: https://www.vendr.com/marketplace/miro — 2026-09-21] | Prueba que las cuentas M365 pagan por colaboración visual aparte. No prueba en qué proporción son cuentas medianas. |

## Alternativas y no-consumo
- **Link externo pegado en el chat.** Es el comportamiento que ya muestran los datos propios (29%). El costo en el mercado: en un estudio de HBR, la gente alterna entre apps unas 1.200 veces por día y pierde casi 4 h por semana (alrededor del 9% del tiempo) en reorientarse. La muestra es chica: 137 usuarios de 3 empresas Fortune 500 [verificado: https://hbr.org/2022/08/how-much-time-and-energy-do-we-waste-toggling-between-applications — 2026-09-21].
- **Reconstruir después.** Se estima que los managers dedican unas 6 h por semana (15% del tiempo) a administrar reuniones: preparar, tomar notas y hacer seguimiento. Es una estimación de LucidMeetings sin n publicado [verificado: https://www.avoma.com/blog/time-spent-on-managing-meetings — 2026-09-21]. Tomarlo solo como orden de magnitud.
- **Compartir pantalla** (67% en los datos propios). Es el "no-consumo" de la co-creación: una persona edita y las demás miran.

## Precio y modelos de negocio
- En Zoom, la colaboración en reunión se incluye pero se **limita por tier** (3 pizarras contra ilimitadas) [verificado: https://pumble.com/zoom-pricing — 2026-09-21].
- En Microsoft, Loop y las notas colaborativas vienen incluidas en la suite, sin add-on. El precio de las suites M365 subió desde el 1-jul-2026, pero el FAQ oficial no menciona Teams, Loop ni Whiteboard dentro del reempaquetado [verificado: https://www.microsoft.com/en-us/licensing/news/2026-m365-packaging-pricing-updates-faq — 2026-09-21].
- Miro cobra por usuario y la negociación típica logra alrededor de 15% de descuento sobre lista [verificado: https://www.vendr.com/marketplace/miro — 2026-09-21].
- **Nota del caso:** los planes "Premium→Max" del overview son del brief del caso y no corresponden a SKUs públicos. No hay benchmark externo directo del salto de USD 8.

## Posicionamiento
- Gartner (Market Guide 2025, vía Lucid) describe la colaboración visual como un mercado **maduro y masivo**. Las tendencias son IA generativa, flujos estructurados, seguridad y residencia de datos, y evaluación por ROI según el caso de uso. Además, "muchos vendors todavía no tienen" controles de residencia de datos [verificado: https://lucid.co/blog/takeaways-gartner-market-guide-for-visual-collaboration — 2026-09-21]. Para cuentas reguladas como la de Marcelo, ese es un espacio donde la suite tiene ventaja.
- El espacio más poblado es "resumen y acciones con IA después de la reunión" (Google, Zoom, Copilot). El menos poblado es la co-creación en vivo con muchos participantes y con gobernanza de la suite.

## Tendencias
- **Descentralización.** Las unidades de negocio controlan el 81% del gasto SaaS e IT solo el 15%. Las compras por gasto de empleados crecieron 267% interanual. En promedio, el 36% de las licencias no se usa (Zylo, 2026 SaaS Management Index, 29-ene-2026, sobre 40M licencias) [verificado: https://zylo.com/news/2026-saas-management-index — 2026-09-21].
- **Apps pagadas por gasto.** Son el 45% de las apps pero el 3,7% del gasto, unos USD 2M al año por empresa en promedio. El 59% tiene rating de seguridad "pobre" o "bajo". Miro y Notion no están en el top 15, donde sí aparecen Canva y Slack [verificado: https://zylo.com/blog/top-expensed-saas-applications — 2026-09-21].
- **Licencias de Miro.** El 61% no se usa: un gasto promedio de USD 85k al año con unos USD 52k desperdiciados (Zylo, sin n publicado) [verificado: https://zylo.com/blog/miro-license-management — 2026-09-21].
- **Consolidación.** El 68% de las organizaciones de IT quiere consolidar proveedores, y la segunda ola apunta a colaboración y productividad (Slack, Teams, Notion). La meta típica es reducir 20%, pero lo que se logra es alrededor de 18% en 24 a 36 meses. La encuesta no tiene muestra publicada y el foco es DACH [verificado: https://www.digital-chiefs.de/en/vendor-consolidation-2026/ — 2026-09-21].
- **Contexto de reuniones M365.** El 57% de las reuniones son llamadas ad hoc sin invitación. Las reuniones de más de 65 asistentes son el tipo que más crece. Hay una interrupción cada 2 minutos (Work Trend Index, jun-2025) [verificado: https://www.microsoft.com/en-us/worklab/work-trend-index/breaking-down-infinite-workday — 2026-09-21]. Que tantas reuniones sean ad hoc hace pensar que no se puede depender de preparar tableros antes. Es una inferencia, no un hallazgo.

## Impacto en creencias
| Creencia (de overview.md) | Veredicto | Evidencia |
|---|---|---|
| #5 [opportunity: trabajo-en-vivo-fuera-de-teams] [viability]: shadow IT de herramientas de colaboración en cuentas medianas que IT quiere eliminar; más downgrade en esas cuentas | **apoya en parte / contradice en magnitud** | Hay descentralización masiva (81% del gasto fuera de IT) e intención de consolidar (68%), incluida la colaboración [verificado]. Pero lo pagado por gasto es solo el 3,7% del gasto y Miro y Notion no están en el top [verificado], así que el "costo recuperable" puede ser chico y el argumento más fuerte es seguridad y gobierno. Nada vincula shadow IT con downgrade: solo lo pueden decir los datos propios. |
| #6 [opportunity: trabajo-en-vivo-fuera-de-teams] [value]: el trabajo conjunto sale afuera en ≥1 de cada 3 reuniones grandes, con ≥1 h por semana de consolidación | **no dice nada directo / apoya débilmente el costo** | El toggling cuesta unas 4 h por semana [verificado, n=137] y la administración de reuniones unas 6 h por semana [verificado, estimación sin n]. Ninguna fuente mide la frecuencia de "sacar el trabajo" en cuentas medianas M365. |
| #2 [product] [value]: se usan externas porque las nativas no cubren la necesidad, no por desconocimiento | **apoya (débil)** | Loop, las notas con tareas en Planner y Whiteboard ya vienen incluidos [verificado], y aun así el uso es bajo. Hay quejas públicas de lentitud y cuelgues de Whiteboard en tableros grandes [verificado: https://learn.microsoft.com/en-us/answers/questions/879950/the-whiteboard-problems-in-teams — 2026-09-21, un caso de 2022]. No descarta el desconocimiento: la persona Norma no conoce las funciones. |
| #1 [product] [viability]: el salto Premium→Max no está anclado a valor percibido | **no dice nada directo / precedente útil** | Zoom usa la colaboración en reunión como diferenciador de tier [verificado]. No hay dato sobre la percepción de valor en cuentas medianas M365. |
| #3 [product] [value] y #4 [product] [value] | no dice nada | Fuera del alcance de esta corrida. |

## Qué sigue necesitando research primario
- **Datos propios, lo primero y más barato:** cruzar el % de reuniones con links externos por cuenta con la tasa de downgrade o no renovación en cuentas de 100 a 1.000 licencias (#5). Ninguna fuente externa puede responderlo.
- **Survey (cuánto y con qué frecuencia):** en cuántas reuniones de más de 5 personas se saca el trabajo afuera y cuántas horas por semana se dedican a consolidar (#6). Separar "no la conocía" de "la probé y no funcionó" (#2). Para IT: qué herramientas se pagan por fuera, cuánto, y si se quieren eliminar en la renovación (#5).
- **Entrevistas (por qué y qué hacen hoy):** qué pasó la vez que probaron Whiteboard, Loop o las notas, qué tipo de trabajo sacan afuera (visual, texto, tareas) y qué pesa más para IT al consolidar: costo, seguridad o adopción (#2, #5).
