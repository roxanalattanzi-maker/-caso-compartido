---
opportunity: trabajo-en-vivo-fuera-de-teams
status: testing-several
chosen: abrir-como-app, pizarra-persistente
tests: product/tests/2026-10-12-1830-trabajo-en-vivo-fuera-de-teams.md
---

# Soluciones para: El trabajo conjunto de las reuniones se hace fuera de Teams

## Qué dice la evidencia ahora
- **#6 [value]** está `weakened` (entrevistas `real`): la co-creación externa es quincenal o trimestral en 5 de 10, no en 1 de cada 3 reuniones; la consolidación es de 10 a 60 min **por reunión**, y solo 1 de 6 estimables llega a ≥1 h/semana. El survey la deja prometedora, no confirmada (87% trabajó afuera alguna vez; 61% en aproximadamente la mitad o más; autoseleccionados, sin separar cuentas medianas). No está `contradicted`.
- **#2 [value]** está `weakened`: se sostiene para Whiteboard (92% la conoce, 67% de quienes la probaron la dejó), no para notas (31% no las conocía) ni para apps en la reunión (40% no sabía que existen).
- **#5 [viability]** sigue sin evidencia propia. El research (`secondary`) apoya "IT quiere consolidar" pero el gasto por fuera es chico (3,7%); en las entrevistas Miro lo contrata la empresa. El cruce de datos propios de la agenda (vencía el 9/10) y la ronda con IT no figuran en `product/`.
- Dos problemas con un mismo síntoma: el 64% trabaja en herramientas donde el trabajo ya vive (72% preexistía) y el 36% usa tableros nuevos (82% se crea para la reunión). La fricción de entrada se concentra en tableros nuevos y en reuniones con externos.
- Límites: entrevistas a Leads de SaaS de 650 a 2.000 empleados (licencias sin verificar); personas sintéticas.

## Baseline: lo que hacen hoy
Pegan el enlace de Miro, Docs o Jira en el chat (54%, survey n=187) o comparten pantalla mientras una persona maneja y el resto dicta o señala (7 de 10 entrevistas, `real`; 52% de las reuniones tiene a alguien mirando la pantalla de otro, Q7 n=178). Trabajan en la herramienta externa y después reconstruyen a mano lo decidido (10 a 60 min por reunión en 7 de 10; ~2 h/semana en Valeria, `synthetic`). Fuentes: `product/insights/2026-09-29-2050-encuesta-colaboracion-en-vivo-fuera-de-teams.md`, `product/insights/2026-09-29-2105-entrevistas-conductores-trabajo-en-vivo-fuera-de-teams.md`, `product/personas/valeria-quiroga.md`.

## Alternativas
### A1. Pizarra nativa persistente (`pizarra-persistente`)
La idea que llegó como pedido ("herramientas colaborativas integradas en la reunión"), hecha concreta: un tablero nativo con votar, agrupar y plantillas, que rinde con 12 o más editores y tiene un enlace estable que sobrevive a la serie de la reunión y guarda historial. Ataca el abandono de Whiteboard. Para Valeria Quiroga (primaria). Reemplaza a Miro, FigJam o Mural para sesiones de co-creación. Mecanismo: reemplazar la herramienta externa.

### A2. Sugerencia al pegar un enlace: abrir como app (`abrir-como-app`)
Cuando alguien pega en el chat de la reunión un enlace de Miro, Docs o Jira, Teams ofrece abrirlo como app dentro de la reunión: todos ven lo mismo, entran con su identidad corporativa y pueden señalar o editar. Es lo mínimo que podría funcionar y un cambio en una herramienta que ya usan. Ataca el 40% que no sabía que las apps existen, el 8% que las abre así y "uno maneja, el resto dicta". Para Valeria (primaria) y Norma Benítez (terciaria, que no abre links por miedo a crear cuenta). Reemplaza el enlace en el chat más la pantalla compartida. Mecanismo: hacer menos doloroso el workaround.

### A5. Tablero de terceros licenciado dentro del plan (`tablero-tercero-en-plan`)
Un acuerdo con un proveedor (Miro, por ejemplo) para incluir su tablero en el plan M365, con integración de primera clase en la reunión. Para Marcelo Ferreyra (secundaria) y Valeria. Ataca el gasto duplicado, el shadow IT y los problemas de licencia e instancia; podría anclar el salto a Max como hace Zoom con sus pizarras. Reemplaza la licencia que cada área paga por fuera. Mecanismo: comprar o aliarse en vez de construir.

## Comparación
| Alternativa | Desirable | Feasible | Viable | Creencia más riesgosa |
|---|---|---|---|---|
| A1 | mixed — pain evidenced, relief not tested. 67% de quienes probaron Whiteboard la dejó (survey, n=136); votar es la actividad #1 afuera (39%); 5 de 10 entrevistados lo mencionan (real). Solo 36% usa pizarras y la co-creación es quincenal o trimestral | to check with tech — Whiteboard se traba con 8 o más editores (research, secondary); 5 meses hasta CollabCon | mixed — Zoom ancla su tier en pizarras ilimitadas (secondary); sin dato propio que una pizarra retenga cuentas; #1 y #5 abiertas | Conductores que hoy co-crean en Miro, Mural o FigJam y tienen historial ahí usarían un tablero nativo para su próxima sesión de co-creación aunque implique dejar ese historial |
| A2 | mixed — pain evidenced, relief not tested; el más cercano a strong. 40% no sabía que existen las apps; 8% las abre así (survey, n=187); 72% de quienes las probaron las sigue usando (Q10, n=67, survey, sustituto cercano); "uno maneja, el resto dicta" en 7 de 10 (real). La sugerencia en sí no fue probada | to check with tech — las apps de terceros en reuniones ya existen (research, secondary) | mixed — sube el uso de lo ya pagado (Marcelo, synthetic); no ancla Max ni elimina gasto en Miro | Abierto como app, quienes hoy miran la pantalla de otro pueden editar u opinar sin cuenta ni licencia adicional (4 de 10 entrevistas con bloqueo de licencia, instancia o identidad, real) |
| A5 | mixed — pain evidenced, relief not tested. Problemas de licencia e instancia reales (4 de 10, real); "que nos paguen Miro" viene de personas synthetic | to check with tech — y un acuerdo comercial que ningún artefacto cubre; 5 meses es poco para negociar | unknown — depende de #5; señales débiles en contra: gasto por fuera 3,7% (secondary), Miro contratado por la empresa en 2 casos reales | #5 [viability]: en ≥1 de cada 3 cuentas medianas esas herramientas se pagan fuera del contrato y IT quiere eliminarlas |

Ninguna celda es strong: nadie reaccionó todavía a estas soluciones concretas.

## Decisión
Elegidas para testear en paralelo, por el usuario el 2026-10-12: **A2 y A1**. Coincide con la recomendación, así que no hay entrada en `product/corrections.md`. Razones de la recomendación: atacan poblaciones distintas (64% trabaja en herramientas existentes, 36% crea tableros nuevos); A2 es la prueba más barata y con evidencia más cercana; la creencia clave de A1 (migrar desde Miro) se puede refutar con un prototipo mostrado antes de invertir en rendimiento. A5 queda en pausa hasta resolver #5. Cambiarían la recomendación: Miro-users que dicen que no migrarían (cae A1), una app que no resuelve licencia o instancia (cae A2), un cruce de datos propios que asocie shadow IT con bajas (sube A5).

## A testear
Diseñado en `product/tests/2026-10-12-1830-trabajo-en-vivo-fuera-de-teams.md`.
- **A2** — "Abierto como app, quienes hoy miran la pantalla de otro pueden editar u opinar sin cuenta ni licencia adicional" (T1, technical-test): si es falsa, la sugerencia no relieva el acceso, que es lo que dejó a gente sin voz en 4 de 10 entrevistas. Después, T2 (prototype-shown) sobre si aceptan el aviso.
- **A1** — "Conductores que hoy co-crean en Miro, Mural o FigJam con historial ahí usarían un tablero nativo para su próxima sesión de co-creación" (T3, prototype-shown): si es falsa, ni votar ni rendir con 12 o más editores alcanzan, porque Miro se queda por continuidad. El rendimiento con 12 o más editores va a tech, no a esta prueba.

## Propuesta de valor: A2 · Abrir como app (`abrir-como-app`)
- **Pain relieved:** quien conduce pega el enlace y los demás miran o dictan: "súbele la prioridad a esa", un ticket equivocado cerrado (Andrés), filtros distintos y 10 a 15 min discutiendo números que no eran los mismos (Diego), una objeción que llegó una semana tarde (Valeria Castro). 52% de las reuniones tiene a alguien mirando la pantalla de otro (survey Q7, n=178).
- **Gain created:** todos ven lo mismo dentro de la reunión, con su identidad corporativa, y quien no manejaba puede señalar o editar.
- **Replaces:** el enlace en el chat más la pantalla compartida. Se cambia porque cuesta un clic sin salir de la reunión, mientras el workaround cuesta errores y voces perdidas.
- **Deliberately does not:** crear tableros nuevos, reemplazar Miro, Docs o Jira, registrar decisiones ni negociar licencias de terceros.

## Propuesta de valor: A1 · Pizarra nativa persistente (`pizarra-persistente`)
- **Pain relieved:** Whiteboard se dejó por lenta con 11 a 14 personas, sin votar ni plantillas y porque "se pierde" lo hecho (Tomás, Javier, Lucía, Sofía, Ricardo; 67% de quienes la probaron, survey).
- **Gain created:** un tablero que vota, agrupa y rinde con 12 o más, con enlace estable atado al equipo y no a la serie, dentro del perímetro M365.
- **Replaces:** Miro, FigJam o Mural para sesiones de co-creación. Se cambia por no tener segunda herramienta, cuenta ni licencia, y porque algunas cuentas no pueden usar herramientas externas (Lucía, compliance, real).
- **Deliberately does not:** replicar todo Miro (diagramas avanzados), importar el historial existente en Miro, cerrar o registrar decisiones.

## Creencias
- [opportunity: trabajo-en-vivo-fuera-de-teams] [value] #6 — referenciada, ya registrada (`weakened`).
- [product] [value] #2 — referenciada, ya registrada (`weakened`).
- [feature: abrir-como-app] [value] — los conductores que hoy pegan el enlace de una herramienta externa en el chat la abren como app en la reunión cuando se les sugiere, en lugar de compartir pantalla para que los demás dicten. *(registrada en overview.md como #7)*
- [feature: abrir-como-app] [feasibility] — abierto como app, quienes hoy miran la pantalla de otro editan u opinan sin cuenta ni licencia adicional, incluidos invitados, otra instancia y cuentas personales. *(registrada en overview.md como #8)*
- [feature: pizarra-persistente] [value] — los conductores que hoy co-crean en Miro, Mural o FigJam con historial ahí usarían un tablero nativo con votar, agrupar, plantillas y enlace estable para su próxima sesión de co-creación. *(registrada en overview.md como #9)*

## Descartadas o en pausa
- **A3. Cierre asistido de decisiones** (`cierre-asistido`) — parked: pertenece a la oportunidad adyacente "reuniones sin cierre de decisiones y responsables", fuera de este enmarcado por decisión del usuario el 2026-10-12. Lo traería de vuelta un `/frame-opportunity` del cierre: es donde la evidencia pesa más (10 de 10 entrevistas con una decisión mal ejecutada; Q11 23%; el resumen de IA no distingue lo decidido de lo hablado, 12 de 26 con salvedad).
- **A4. Plantilla y ritual "Decisiones"** (`ritual-decisiones`) — parked, mismo motivo y misma condición. Es la alternativa no software de ese conjunto.
- **A5. Tablero de terceros licenciado en el plan** (`tablero-tercero-en-plan`) — parked: depende de #5, sin evidencia propia. Lo traería de vuelta el cruce de datos propios (shadow IT vs. baja o no renovación) más la ronda con IT.

## Resultado
Pendiente: lo agrega `/analyze-solution-tests`.
