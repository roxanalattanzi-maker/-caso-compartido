---
date: 2026-09-29
source: real
opportunity: trabajo-en-vivo-fuera-de-teams
sources:
  - product/interviews/2026-09-25-1000-tomas-aguirre.md (real)
  - product/interviews/2026-09-25-1100-andres-quintero.md (real)
  - product/interviews/2026-09-25-1600-lucia-fernandez.md (real)
  - product/interviews/2026-09-28-0900-javier-molina.md (real)
  - product/interviews/2026-09-28-0930-martina-rojas.md (real)
  - product/interviews/2026-09-28-1000-diego-paredes.md (real)
  - product/interviews/2026-09-28-1200-sofia-martinez.md (real)
  - product/interviews/2026-09-28-1400-paula-benitez.md (real)
  - product/interviews/2026-09-28-1500-valeria-castro.md (real)
  - product/interviews/2026-09-28-1700-ricardo-salinas.md (real)
---

# Insights de las 10 entrevistas a conductores de reuniones grandes

- **Fuentes:** las 10 transcripciones de `product/interviews/interviews.zip` (25 y 28/09/2026, 26 a 34 min, modo exploración). Todas son entrevistas reales (`source: real`) a personas que aceptaron la conversación en el survey (`survey_respondent` en cada cabecera).
- **Perfil:** Engineering, Product, Design, Data y Support Leads de empresas SaaS de 650 a 2.000 empleados en 2 a 4 países. Seis vinieron del panel y cuatro del email.
- **Creencias en juego:** #6 y #2 de `product/overview.md`, las dos de la guía.

**Límites.** Diez conversaciones no miden frecuencia: dicen cómo pasa y por qué, no cuánto. Todas salen de opt-ins autoseleccionados. La firmografía por licencias no se verificó (las empresas tienen 650 a 2.000 empleados; la oportunidad apunta a cuentas de 100 a 1.000 licencias). La guía pregunta por la última vez que algo terminó hecho distinto de lo acordado, lo que presupone que ocurrió: los 10 relatan un caso concreto, pero eso no permite estimar su frecuencia. Las transcripciones citan una guía (`2026-09-23-2030-colaboracion-en-vivo-fuera-de-teams.md`) que no está en `product/interview-guides/`.

## Cuánto se repite cada insight

| Entrevistado (canal) | Q1 del survey | 1 · Decisión perdida | 2 · Resumen de IA | 3 · Pizarra nativa | 4 · Uno maneja, el resto dicta | 5 · Sin acceso al tablero |
|---|---|---|---|---|---|---|
| Tomás Aguirre (panel) | En todas | ● | | ● | ● | ● |
| Andrés Quintero (panel) | En ninguna | ● | | | ● | |
| Lucía Fernández (email) | En ninguna | ● | ● | ● | ● | |
| Javier Molina (panel) | Más de la mitad | ● | ● | ● | ● | ● |
| Martina Rojas (panel) | Más de la mitad | ● | ● | | ● | |
| Diego Paredes (email) | Aprox. la mitad | ● | ● | | ● | |
| Sofía Martínez (panel) | Más de la mitad | ● | | ● | | ● |
| Paula Benítez (email) | En ninguna | ● | ● | | | |
| Valeria Castro (email) | Menos de la mitad | ● | ● | | ● | ● |
| Ricardo Salinas (panel) | En ninguna | ● | | ● | | |
| **Total** | | **10 de 10** | **6 de 10** | **5 de 10** | **7 de 10** | **4 de 10** |

## 1. Lo que falla es el cierre de la reunión: 10 de 10 tuvieron una decisión que se ejecutó distinta y 7 de 10 la reconstruyen a mano después

Cada uno relata un caso concreto en que lo decidido se perdió o se entendió distinto, sea cual sea la herramienta (Miro, Jira, Excel, Confluence o solo hablado). En 8 de los 10 el costo fue de días a semanas: un release movido, dos semanas de trabajo sobre una decisión que se había descartado, un escalamiento de cliente parado 4 días, un fin de semana de guardia. Las causas se repiten: la decisión queda en un sitio y el lector mira en otro (Javier, Martina, Diego, Sofía), nadie asume ser el dueño (Andrés, Lucía, Ricardo) o el «por qué» no se escribe (Martina). Siete de los diez dedican entre 10 y 60 minutos por reunión a reconstruirlo (Tomás 20 min, Andrés 30 o más, Lucía 30, Javier 30, Diego 20, Valeria cerca de 1 hora, Paula 10 revisando el resumen de IA) y tres dicen expresamente que nadie más lo hace (Tomás, Javier, Valeria). Implica que la necesidad más fuerte no es una pizarra mejor: es cerrar la reunión con decisión, responsable, fecha y motivo, visible donde trabaja quien la ejecuta. Es la oportunidad que el enmarcado dejó como «adyacente» y que el survey ya empujaba (23% de lo más difícil en Q11).

> Evidence: "En la reunión se acordó, con fecha. En el recap quedó como "se habló de la API de geocercas". El equipo de México leyó el recap, no el hilo, y entendió que no era prioridad. Entregaron dos semanas tarde. Nosotros tuvimos que mover una release entera." — Javier Molina
> Evidence: "Lo que sí me serviría es algo que cierre la reunión con lo decidido y el por qué, y que eso quede en el ticket. Eso no lo tengo." — Martina Rojas
> Evidence: "Yo pensé que el arquitecto iba a hacer el ADR y él pensó que yo lo iba a mandar por correo." — Ricardo Salinas

## 2. El resumen de IA de Teams lo probaron 6 de 10 y ninguno lo usa tal cual: no distingue lo decidido de lo hablado

Las seis personas que lo usaron o lo probaron le ponen la misma objeción, con cuatro variantes: resume la conversación, no las decisiones (Martina, Javier); no dice quién se comprometió a qué (Lucía); no ve lo que pasó en la herramienta externa, ni qué número o filtro se miraba (Valeria, Diego); y en el peor caso marca como decisión algo que era solo una idea (Paula). Ese último error costó una semana de dos desarrolladores. Las respuestas: Paula revisa el resumen antes de enviarlo (10 min por reunión), Javier lo reescribe (30 min), Martina lo dejó, Diego lo usa para recordar de qué se habló, Lucía para poner al día a quien no vino, y Valeria lo miró y no le sirvió. Implica que en este flujo un resumen que inventa decisiones es más dañino que uno que omite, y que el requisito mínimo es separar decisión, responsable, fecha y motivo, con las salvedades a la vista. Coincide con el survey: en Q9, 12 de 26 respuestas que ponían el recap como registro agregaron una salvedad.

> Evidence: "marca como decisión cosas que eran solo ideas. Alguien dice "podríamos pasar el release al 20" y en el resumen aparece "se decidió pasar el release al 20"." — Paula Benítez
> Evidence: "Me resumió la conversación, no las decisiones." — Martina Rojas
> Evidence: "Pero no me dice quién se comprometió a qué." — Lucía Fernández

## 3. La pizarra nativa se abandona por lenta, sin votación y, sobre todo, porque se pierde lo hecho; Miro se queda porque el tablero tiene dirección fija e historia

Cinco de diez la probaron en sus reuniones y tuvieron un problema. Tres motivos: es lenta con 11 a 14 personas (Tomás, Javier, Sofía, Ricardo); no permite votar ni agrupar y no tiene plantillas (Tomás, Javier, Lucía, Ricardo); y queda atada al chat de esa reunión, de modo que al cambiar la serie o hacer otra convocatoria no se encuentra (Tomás, Lucía; Sofía tampoco supo dónde había quedado, y las notas de reunión sufren lo mismo en el caso de Paula). Quienes más lo destacan son Tomás, para quien perder los acuerdos fue lo que cerró la puerta, y Lucía, para quien es «la parte que más rabia me da» y hoy saca una captura y la pega en Confluence. Los dos usuarios intensivos de Miro (Tomás, Javier) lo describen al revés: un tablero que se reutiliza (uno por trimestre en Tomás; el mismo desde hace tres años en Javier), con un frame nuevo por sesión, para ver qué se acordó y qué se arrastra. Implica que un tablero nativo tiene que persistir, tener un enlace estable e independiente de la reunión y guardar la historia; votar y rendir con 12 o más editores son condiciones necesarias, pero ninguna sustituye eso. El survey da la misma señal: 43% la usó y la dejó, 67% de quienes la probaron.

> Evidence: "A las dos semanas, para la retro siguiente, fui a buscarla y no estaba. Quedó colgada del chat de esa reunión, y justo en el medio se había recreado la serie de la reunión, porque cambiamos el horario. […] Perdí los acuerdos, así de simple." — Tomás Aguirre
> Evidence: "Esa continuidad es la razón por la que estamos en Miro." — Tomás Aguirre
> Evidence: "No tenía forma de votar. Plantillas, ninguna que sirviera. Y con catorce personas se arrastraba: iba lento, las notas se solapaban." — Javier Molina

## 4. En muchas reuniones una persona maneja y el resto dicta o señala, y eso genera errores, no solo pérdida de tiempo

Siete de diez describen el mismo patrón: solo quien maneja puede tocar y los demás dictan («"la de abajo", "no, la otra"») o mandan su aporte por chat. Ocurre sobre todo al compartir pantalla de una herramienta existente (Jira, Excel, Power BI, Figma: Tomás, Andrés, Martina, Diego, Valeria) y también en tableros cuando alguien no puede editar (Lucía, Javier). El costo son minutos cada vez, y a veces un error: Andrés cerró el ticket equivocado y el cliente recibió la notificación de cierre; en la revisión de métricas de Diego, cada uno tenía un filtro distinto y discutieron 10 a 15 minutos sobre números que no eran los mismos. En las reuniones sobre herramientas corporativas con inicio de sesión único no hay problema de acceso (Martina: «cero fricción»; Diego: «en un minuto ya están todos»), y la definición de Q1 («no cuenta si solo miraron una pantalla compartida») las deja fuera: Andrés respondió «En ninguna» y tiene esta fricción «en cada reunión, varias veces». Implica que parte de la oportunidad está en reuniones que el survey clasificó como «no trabajan afuera»: hace falta poder señalar y que todos vean lo mismo sobre el contenido compartido.

> Evidence: "Hace como un mes y medio cerré un ticket que no era. Me dijeron "ese ciérralo", yo lo marqué cerrado, y era el de la fila de al lado. Al cliente le llegó la notificación de cierre y el caso seguía abierto." — Andrés Quintero
> Evidence: "uno decía "las ventas bajaron ocho por ciento" y otro "no, a mí me sale que subieron". Y estábamos hablando de números distintos sin darnos cuenta." — Diego Paredes
> Evidence: "manejo yo y el resto dicta: "súbele la prioridad a esa", "esa ponle tres puntos", "esa asígnamela"." — Martina Rojas

## 5. El acceso a un tablero del equipo es un problema de identidad y licencia, y lo que pesa es la voz que se pierde, no los minutos

Cuatro de diez (Tomás, Javier, Valeria, Sofía) tuvieron a alguien sin poder editar: invitados sin licencia (3 de 11 en el equipo de Tomás), otra instancia de Miro por filial (Lyon en el caso de Javier), cuentas personales de Google que FigJam no reconoce (Valeria) y falta de permiso en Confluence (Sofía). Cuesta 5 a 10 minutos al inicio, pero el daño mayor es quién queda mirando: una persona de soporte de Valeria no logró entrar, no habló, y su objeción a una decisión clave (sacar la reprogramación por WhatsApp) apareció una semana después, cuando ya se estaba trabajando en eso. En Martina, un desarrollador escribió su desacuerdo por privado después de la reunión, y Sofía sospecha que quienes no hablaron no estaban de acuerdo («Rodrigo dijo "va" pero con cara de que no»). Implica medir el acceso por quién puede editar y opinar, no por minutos hasta entrar; los tableros propios de un equipo chocan con licencias e identidades que las herramientas corporativas con inicio de sesión único (Jira, Power BI) no tienen.

> Evidence: "Una objeción importante, y yo ni me enteré en la reunión." — Valeria Castro
> Evidence: "En casi todas hay alguien mirando desde afuera, y esa gente no opina. Eso me preocupa más que los minutos." — Valeria Castro
> Evidence: "la filial de Francia tiene otra instancia de Miro, otra licencia, y el tablero es de la de España." — Javier Molina

## Lo que matiza estos hallazgos

- **La herramienta no es el problema para 4 de 10.** Sofía («la herramienta no es el problema […] Lo que nos falla es cómo se cierra la reunión»), Diego («es disciplina»), Martina («no veo para qué querría otra herramienta») y Paula («no es que no nos dejen. Es que no lo necesito»). Refuerza el insight 1: la demanda está en el cierre, no en sumar una herramienta.
- **La reunión grande no es donde se decide.** Paula («las decisiones de verdad se toman en reuniones chicas, de tres o cuatro») y Ricardo («con dieciséis personas no se puede decidir nada») deciden aparte. El problema de registro se mueve entonces a la reunión chica y al pasaje entre ambas.
- **Trabajar afuera es menos frecuente de lo que sugiere el survey.** Cinco de diez usan un tablero o documento externo para crear en conjunto, pero con cadencia trimestral (planning), quincenal (retro) o mensual (kickoff), no en una de cada tres reuniones. Tomás lo corrigió: «creo que en la encuesta puse que salgo de Teams en todas las reuniones. No es así. […] Exageré un poco». Lo que sí es frecuente, semanal, es compartir pantalla sobre una herramienta existente (insight 4).
- **Un caso donde lo nativo sí funciona.** Paula usa las notas de reunión y el resumen de IA sin problema en un review informativo de 14 personas; su fallo es de otro orden (las notas no siguen a la serie cuando se reprograma, y el resumen mezcla ideas con decisiones). Lucía, en cambio, no puede usar nada externo: compliance lo prohíbe y aprobar una herramienta lleva meses. Ambos cubren el contraste que el enmarcado pedía.
- **No todo es la reunión.** Ricardo carga 27 horas semanales de reuniones y Andrés dice que la suya dura 1,5 horas y debería durar 40 minutos: para dos de diez el problema es el volumen.

## Qué dice esto del survey

Al cotejar las respuestas del survey de los 10 con lo que contaron: Q1 es consistente con la entrevista en 8, con una corrección explícita (Tomás, «En todas») y un caso no verificable (Javier, «Más de la mitad»); y el tiempo de entrada (Q6) coincide en los 6 casos donde lo cuantificaron. Ambas dudas están en el panel, que ya declaraba más intensidad que el email (69% vs. 47% en aproximadamente la mitad o más). Es una señal débil, de 2 casos, y solo justifica una hipótesis: el panel puede sobreestimar la frecuencia. Además, Valeria respondió que conocía la Whiteboard y en la entrevista dijo que ni sabía que existía.

## Lo que las entrevistas no cubrieron

- **El tiempo semanal de consolidación** (pregunta 1.4 de la guía) no se preguntó. Con lo que cuentan, en 6 de 10 se puede estimar: solo Paula llega a cerca de 1 hora por semana (10 min × casi todas sus reuniones, estimación mía a partir de sus datos) y Andrés a 30 minutos o más. Tomás, Diego, Javier y Valeria quedan entre 2 y 20 minutos semanales. Lo que se sostiene es 10 a 60 minutos por reunión, no ≥1 h por semana.
- **Quién paga la herramienta y qué dijo IT** (preguntas 2.4 y 2.5) no aparecen. Javier dice que Miro está contratado por la empresa y Tomás que sus miembros tienen licencia: en ningún caso se ve gasto por fuera del contrato.
- **Frecuencia y tamaño de cada patrón:** para eso sirve el survey, no estas 10 conversaciones.

## Preguntas abiertas para más entrevistas

1. ¿Cuánto suma por semana el trabajo de reconstruir lo decidido, medido sobre una semana real y no sobre una reunión?
2. ¿Quién debería ser el dueño de cerrar la reunión, y qué pasa en los equipos donde alguien sí lo hace bien (Sofía, con su sección «Decisiones»)?
3. ¿Qué hace el equipo de Lucía donde nada externo es posible, y qué pide de lo nativo?
4. Referidos que nombraron como contraste: reuniones que se resuelven solo hablando (Carla, Fernanda, Mariana), por Slack (el manager de Colombia de Martina) y quienes viven en Miro (Gonzalo, Daniela).

## Contraste con las creencias del overview (propuesta, pendiente de aprobación)

- **#2 [product] [value]** (recurren a herramientas externas porque lo nativo no cubre, no por desconocimiento): **respaldada para la Whiteboard, con matices.** Tres de los cuatro que probaron la Whiteboard la dejaron por capacidad y persistencia (Tomás, Javier, Sofía); Valeria no sabía que existía. Además, Andrés no conocía las notas, Ricardo no sabía que se pueden meter otras herramientas en la reunión y Diego nunca usó Loop. Coincide con la propuesta desde el survey (`weakened`, aún sin guardar). Con fuente real, el estado más justo para el conjunto es `weakened`; no propongo `confirmed`.
  - Línea propuesta: `— weakened by product/insights/2026-09-29-2105-entrevistas-conductores-trabajo-en-vivo-fuera-de-teams.md (2026-09-29)`
- **#6 [opportunity: trabajo-en-vivo-fuera-de-teams] [value]** (≥1 de cada 3 reuniones sale afuera, con ≥1 h/semana de consolidación): **propongo `weakened`.** La consolidación de 10 a 60 minutos por reunión aparece en 7 de 10, pero por semana solo 1 de los 6 estimables llega a 1 hora. Sobre la frecuencia, el trabajo de co-creación externo es quincenal o trimestral en cinco casos, y Tomás corrigió su «En todas». Lo que sí es frecuente es la pantalla compartida sobre una herramienta existente.
  - Línea propuesta: `— weakened by product/insights/2026-09-29-2105-entrevistas-conductores-trabajo-en-vivo-fuera-de-teams.md (2026-09-29)`
- **#5 [opportunity] [viability]** (shadow IT): **no evaluable.** No se preguntó por el pago ni por IT. Solo dos señales indirectas: Miro contratado por la empresa (Javier) y prohibido por compliance (Lucía).
- **#1, #3, #4:** no las tocan. Solo #3 asoma en dos casos (Ricardo, Andrés) sin evidencia sobre baja de plan.

**Siguiente paso:** las entrevistas empujan a reenmarcar la oportunidad hacia el cierre de decisiones (insights 1 y 2) antes del punto de decisión del 20/11; con 10 entrevistas reales más el survey ya alcanza para `/derive-personas` si quieres ir por ese lado.
