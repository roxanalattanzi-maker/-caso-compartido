---
opportunity: trabajo-en-vivo-fuera-de-teams
solutions: product/solutions/2026-10-12-1821-trabajo-en-vivo-fuera-de-teams.md
status: designed
---

# Pruebas de solución para: El trabajo conjunto de las reuniones se hace fuera de Teams

## Por qué testear
Están en prueba **A2** (`abrir-como-app`) y **A1** (`pizarra-persistente`). El dolor está evidenciado en las dos: 4 de 10 entrevistas con bloqueos de acceso, 7 de 10 con "uno maneja, el resto dicta" y el 67% de quienes probaron Whiteboard la dejó (survey, n=136). Lo que no está evidenciado es que estas soluciones lo relieven, porque nadie reaccionó a ellas. Lo más cercano es que el 72% de quienes ya usan apps en la reunión las sigue usando (Q10, n=67), que no prueba el efecto del aviso ni que el acceso se resuelva. Cada prueba apunta a la creencia que mata la alternativa. Orden: T1 primero, porque es barata y puede descartar A2 antes de gastar sesiones; T2 solo si T1 no descarta; T3 puede correr en paralelo.

**Límites de los tres diseños.** Los participantes de T2 y T3 salen del pool de opt-in del survey: autoseleccionados, con firmografía sin verificar. Se filtra por tamaño de cuenta al reclutar, pero no se garantiza. Una prueba con prototipo tiene efecto de demanda, por eso la señal es un compromiso concreto y no una opinión.

## T1. abrir-como-app: acceso sin licencia adicional
- **Test status:** ready
- **Belief under test:** `[feature: abrir-como-app] [feasibility]` abierto como app, quienes hoy miran la pantalla de otro editan u opinan sin cuenta ni licencia adicional, incluidos invitados, otra instancia y cuentas personales. *(pendiente de registro en `product/overview.md`)*
- **Risk:** [feasibility]
- **Test type:** technical-test
- **What we do:** Tech abre en un tenant de prueba una reunión de Teams con la herramienta abierta **como app** y comprueba, para cada escenario sacado de las entrevistas, si el participante puede editar o comentar sin crear cuenta ni pedir licencia: (a) usuario interno sin licencia de la herramienta (3 de 11 en el equipo de Tomás); (b) invitado externo a la organización (23% de las reuniones tiene externos); (c) usuario de otra instancia de la herramienta (el caso de Lyon, Javier); (d) usuario con cuenta personal (el caso de FigJam, Valeria Castro). Se prueba en una herramienta de tablero sin inicio de sesión único (Miro, la de más evidencia) y, como control, en una herramienta con inicio de sesión único corporativo (Jira o equivalente). Qué apps tienen hoy app de Teams lo confirma tech.
- **With whom:** Tech. Sin participantes externos: 4 escenarios en la herramienta de tablero y 1 de control con inicio de sesión único.
- **Material needed:** una hoja de captura con la grilla escenario × herramienta (puede editar o comentar: sí/no; pasos extra: crear cuenta, pedir licencia, otro; nota libre). Queda fuera todo lo que no sea el acceso: sin diseño del aviso, sin rendimiento.
- **Material:** `product/tests/materials/t1-abrir-como-app/hoja-de-captura.md`
- **Duration:** máximo 3 días hábiles de tech, a confirmar con tech.
- **Signal and threshold:** número de escenarios (de 4) en que el participante edita o comenta sin crear cuenta ni pedir licencia, en la herramienta de tablero; y si el control con inicio de sesión único funciona. Umbral: **≥3 de 4** y control correcto.
- **Decision rule:** continue si ≥3 de 4 escenarios funcionan y el control funciona · change si <3 de 4 pero el control funciona (A2 se reduce a herramientas con inicio de sesión único; sigue con su propio test de valor) · discard si el control falla (los participantes no pueden editar ni comentar abierto como app).
- **Expected provenance:** real (medición técnica, no de usuarios)
- **Next step if it passes:** T2.

## T2. abrir-como-app: aceptación del aviso
- **Test status:** designed
- **Belief under test:** `[feature: abrir-como-app] [value]` los conductores que hoy pegan el enlace de una herramienta externa en el chat la abren como app en la reunión cuando se les sugiere, en lugar de compartir pantalla para que los demás dicten. *(pendiente de registro en `product/overview.md`)*
- **Risk:** [value]
- **Test type:** prototype-shown
- **What we do:** Sesión de 30 minutos con cada conductor. Trae el enlace de un artefacto de su última reunión grande (tablero, documento o ticket). Se le plantea la escena: "estás en la reunión y tenés que pasarle esto al grupo para trabajarlo; hacelo como lo harías hoy". Usa un prototipo clickeable de una reunión de Teams con chat. Cuando pega el enlace aparece el aviso "Abrir como app para todos". Se observa, sin guiarlo, si acepta el aviso, lo ignora o lo cierra y comparte pantalla. Al final se pide un compromiso: agendar en su calendario, durante la sesión, una reunión real de las próximas 2 semanas e invitar al facilitador para probar el aviso con el equipo.
- **With whom:** 8 conductores de reuniones de más de 5 personas, del pool de opt-in del survey (`product/insights/2026-09-29-2050-…`, 64 candidatos, 58 con contacto), excluyendo a los 10 ya entrevistados y a quienes administran M365. Se prioriza a quienes respondieron Q3 "enlace pegado en el chat". En el filtro se pregunta tamaño de la cuenta (100 a 1.000 licencias).
- **Material needed:** un prototipo clickeable de una reunión de Teams con chat, donde pegar un enlace dispara el aviso y aceptarlo muestra la herramienta abierta con otros cursores. Un guion de facilitación con la escena y la pregunta de compromiso. Una hoja de captura por participante: primer camino elegido (aviso, pantalla compartida, otro), si acepta el aviso sin ayuda (sí/no), dudas, y compromiso (fecha, nombre de la reunión, invitación enviada sí/no). Queda fuera: integración real, ajustes, IA, el cierre de decisiones.
- **Material:** *(lo agrega `/build-solution-test`)*
- **Duration:** sesiones en 1 semana.
- **Signal and threshold:** S1 = participantes que aceptan el aviso sin que el facilitador lo indique (de 8). S2 = participantes que agendan la reunión real durante la sesión (de 8). Umbral: S1 ≥6 y S2 ≥4.
- **Decision rule:** continue si S1 ≥6 y S2 ≥4 · discard si S1 ≤3 o S2 ≤1 · change en cualquier otro caso (se rediseña el momento o el texto del aviso y se vuelve a testear).
- **Expected provenance:** real
- **Next step if it passes:** Wizard of Oz en las reuniones reales agendadas: un facilitador abre la herramienta como app en la reunión, y se mide si los participantes que antes miraban editan u opinan.

## T3. pizarra-persistente: migrar desde Miro
- **Test status:** designed
- **Belief under test:** `[feature: pizarra-persistente] [value]` los conductores que hoy co-crean en Miro, Mural o FigJam con historial ahí usarían un tablero nativo con votar, agrupar, plantillas y enlace estable para su próxima sesión de co-creación. *(pendiente de registro en `product/overview.md`)*
- **Risk:** [value]
- **Test type:** prototype-shown
- **What we do:** Sesión de 30 minutos con cada conductor. Se le muestra un prototipo clickeable de un tablero nativo y hace una tarea real de su última sesión: priorizar una lista votando y agrupando con una plantilla. Se le enseña que el tablero tiene enlace propio, atado al equipo y no a la serie de la reunión. Se le dice de forma explícita que **no trae el historial de Miro**. Luego se le pregunta con qué herramienta haría su próxima sesión de co-creación y por qué. Al final se pide un compromiso: enviar durante la sesión una invitación de calendario a su equipo (≥3 personas, con fecha) para esa sesión, para hacerla en el tablero nativo.
- **With whom:** 8 conductores que usan Miro, Mural o FigJam, del mismo pool de opt-in (Q2 = herramienta tipo pizarra; Q4 "se siguió usando"), excluyendo a los 10 ya entrevistados y a IT. Mismo filtro de tamaño de cuenta que T2. No se repiten participantes de T2.
- **Material needed:** un prototipo clickeable de un tablero con votar, agrupar y una plantilla, y un enlace estable visible. Un guion que incluye la aclaración del historial y la pregunta de elección. Una hoja de captura por participante: herramienta que elegiría para la próxima sesión, motivo (continuidad o historial, votación, plantillas, acceso), si envía la invitación al equipo (sí/no, fecha, personas). Queda fuera: diagramación avanzada, importación del historial, rendimiento con 12 o más editores.
- **Material:** *(lo agrega `/build-solution-test`)*
- **Duration:** sesiones en 1 semana.
- **Signal and threshold:** S = participantes que envían durante la sesión la invitación a su equipo para su próxima sesión en el tablero nativo (de 8). Umbral: **≥4 de 8**.
- **Decision rule:** continue si S ≥4 · discard si S ≤1 · change si S es 2 o 3 (se ajusta la propuesta según el motivo más repetido y se vuelve a testear).
- **Expected provenance:** real
- **Next step if it passes:** Wizard of Oz con una sesión real de co-creación del equipo en un tablero operado a mano. El rendimiento con 12 o más editores va a tech antes de cualquier construcción.

## Resultados
*(lo agrega `/analyze-solution-tests`)*

## Decisión
*(lo agrega `/analyze-solution-tests`)*
