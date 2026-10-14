---
status: revised (tras la crítica de 2026-10-13-2150)
slug: seguir-trabajo-en-vivo
journey-persona: norma-benitez (terciaria)
primary-persona: valeria-quiroga (primaria, quien conduce)
critique: product/insights/2026-10-13-2150-critique-seguir-trabajo-en-vivo.md
opportunity: adyacente, sin enmarcar (declarado: se saltó /frame-opportunity)
solutions explored: no (declared)
solutions tested: no (declared)
---

# Seguir el trabajo en vivo

## Problem
En las reuniones de más de 5 personas, el trabajo se hace sobre una pantalla o un tablero que maneja una sola persona. Los demás miran, dictan ("la de abajo", "no, la otra") o no logran entrar. Cuando eso pasa, el grupo trabaja sobre cosas distintas y las voces que no pueden tocar nada se pierden o llegan tarde. Además, quien se desconecta un rato después no sabe qué se decidió ni qué le tocó. Ahora importa porque CollabCon es en ≈5 meses y estas reuniones son el caso diario de las cuentas medianas.

Dos situaciones distintas con un mismo síntoma ("estoy en la reunión pero no puedo seguirla"):

- **Quien mira y no puede participar.** En el 52% de las reuniones hay al menos un participante mirando la pantalla de otro (survey Q7, n=178), y 48% aun sin externos. 7 de 10 conductores entrevistados describen "uno maneja, el resto dicta"; 4 de 10 tuvieron a alguien sin poder editar por licencia, instancia o cuenta.
- **Quien se pierde el hilo.** Solo hay evidencia indirecta: 10 de 10 entrevistas relatan una decisión que se ejecutó distinta de lo acordado, y el resumen de IA no distingue lo decidido de lo hablado (6 de 10). La necesidad de Norma ("después no sabe qué le tocó hacer") viene de la persona, que es sintética.

> Evidence: "Una objeción importante, y yo ni me enteré en la reunión." — Valeria Castro, `product/insights/2026-09-29-2105-entrevistas-conductores-trabajo-en-vivo-fuera-de-teams.md` (real)
> Evidence: "Me dijeron "ese ciérralo", yo lo marqué cerrado, y era el de la fila de al lado. Al cliente le llegó la notificación de cierre y el caso seguía abierto." — Andrés Quintero, ídem (real)
> Evidence: "uno decía "las ventas bajaron ocho por ciento" y otro "no, a mí me sale que subieron". Y estábamos hablando de números distintos sin darnos cuenta." — Diego Paredes, ídem (real)
> Evidence: "Lo que sí me serviría es algo que cierre la reunión con lo decidido y el por qué, y que eso quede en el ticket." — Martina Rojas, ídem (real)

Límites de la evidencia: diez entrevistas autoseleccionadas a Leads de SaaS de 650 a 2.000 empleados, con licencias sin verificar. Quien no pudo participar aparece solo contado por otro (la conductora) y nunca en primera persona. Ninguna entrevista fue a una persona como Norma.

## Who it's for
- **Valeria Quiroga** (primaria): la conductora que pega el enlace o comparte pantalla y necesita que su equipo opine en el momento, no una semana después. Responde por lo que queda decidido y por lo que se toca en su reunión, por eso decide quién puede editar.
- **Norma Benítez** (terciaria, protagonista del recorrido): la mayoría silenciosa que participa pero no convoca. Si en la reunión mandan un link a Miro o a un Doc, no sabe si debe crear una cuenta y no lo abre. Es sintética: su perfil no está contrastado con personas reales.

## User journey
Desde el punto de vista de Norma. Los pasos con (supuesto) no tienen evidencia real y quedan registrados como supuestos.

1. **Trigger** — Norma entra desde el link de Outlook a una reunión de área de más de 5 personas, a la que asiste sin hablar mucho (persona).
2. Quien conduce pega el enlace de un tablero, documento o ticket en el chat, o comparte pantalla (insight 4 de entrevistas; 54% pega el enlace en el chat, survey).
3. Norma no sabe si tiene que crear una cuenta y no abre el enlace; queda mirando la pantalla de otro (persona, supuesto; caso real parecido: la persona de soporte de Valeria Castro, que no pudo entrar).
4. Si algo no es lo que ve, lo dicta o lo calla ("la de abajo", "no, la otra"). Si no habla, su objeción aparece después, o nunca (real, en terceros).
5. **Valor 1** — El contenido se abre dentro de la reunión, con su identidad corporativa y sin cuenta ni licencia adicional. Norma ve lo mismo que quien maneja y puede señalar o comentar sin pedir permiso (supuesto).
6. Al cerrar la reunión, quien conduce confirma la lista y Norma la recibe por el chat o el correo: lo decidido separado de lo hablado, con responsable y fecha, y sabe qué le toca (supuesto).
7. **Outcome** — Participa en el momento, no queda en evidencia por no saber usar una herramienta y no le pregunta a una compañera qué se decidió.

## Critical user stories

### Ver lo mismo que quien maneja
As Norma Benítez, I want ver en la reunión el mismo contenido que quien lo maneja, en el mismo estado, so that no discuto sobre algo distinto de lo que ven los demás.

Acceptance criteria:
- [ ] Cuando alguien abre un tablero, documento o ticket en la reunión, todos los participantes lo ven en el mismo estado (filtros y selección incluidos).
- [ ] Si quien maneja cambia un filtro o la selección, los demás lo ven cambiar sin pedirlo.
- [ ] Un participante puede mirar sin que su vista cambie la de los demás (modo "solo ver").
- [ ] Si el contenido no admite una vista compartida, la reunión lo dice (mensaje visible) en lugar de mostrar algo distinto en silencio.
- [ ] Caso borde: un participante que entra tarde ve el estado actual y no el de cuando empezó.

Traces to: insight 4 de las entrevistas (Diego, Andrés, Martina) y survey Q7.

### Señalar y opinar sin manejar
As Norma Benítez, I want señalar o comentar sobre lo que se está viendo sin tener que dictárselo a otra persona y sin quedar expuesta, so that mi aporte llega en el momento.

Acceptance criteria:
- [ ] Cualquier participante puede marcar un elemento (cursor o resalte) visible para todos, sin editar el contenido.
- [ ] El primer aporte puede dirigirse solo a quien conduce, sin que lo vea el resto; el participante elige si lo hace visible para todos.
- [ ] Las opciones de señalar y comentar aparecen cuando el participante intenta tocar el contenido; no hay un modo que elegir antes.
- [ ] Un comentario hecho en la reunión queda atado a ese elemento y se ve después de terminada.
- [ ] Quien no tiene permiso de edición ve un mensaje en palabras comunes de qué sí puede hacer y a quién pedir permiso, no un error.
- [ ] Caso borde: tres personas señalan a la vez; las marcas se distinguen y no se pisan.

Traces to: insights 4 y 5 de las entrevistas (Valeria Castro, Martina Rojas). El aporte sin nombre y las opciones que aparecen al tocar vienen de la crítica del panel (sintética), no de evidencia real.

### Decidir quién puede editar
As Valeria Quiroga, I want decidir quién puede editar el contenido compartido en mi reunión, so that más gente participando no produce un cambio equivocado.

Acceptance criteria:
- [ ] Por defecto, todos los participantes pueden mirar y comentar; editar lo habilita quien conduce, para todos o para personas puntuales.
- [ ] Cada edición muestra quién la hizo y se puede deshacer durante la reunión.
- [ ] Con 10 a 15 participantes mirando y 3 editando a la vez, el contenido compartido sigue respondiendo sin que nadie vea un estado distinto. *(Umbral de tiempo de respuesta a definir con Tech.)*
- [ ] Quien conduce ve cuántos participantes están mirando sin interactuar. *(Ver nombres es una decisión abierta: choca con la exposición de quien participa.)*
- [ ] Caso borde: si quien conduce sale de la reunión, el permiso pasa a otro organizador o vuelve al valor por defecto, y se avisa.

Traces to: insight 4 de las entrevistas (Andrés Quintero, ticket cerrado por error) y crítica del panel (sintética). El umbral de rendimiento y la vista de quién mira son supuestos.

### Entrar sin crear cuenta
As Norma Benítez, I want abrir lo que comparten sin crear una cuenta ni pedir una licencia, so that no quedo afuera por no saber qué hacer.

Acceptance criteria:
- [ ] Un usuario interno sin licencia de la herramienta señala o comenta sin pasos extra.
- [ ] Un invitado externo a la organización accede con el mismo resultado, o ve un mensaje que dice qué no puede hacer y por qué.
- [ ] Un usuario de otra instancia o con cuenta personal accede con el mismo resultado, o ve ese mismo mensaje.
- [ ] En ningún caso aparece un pedido de crear cuenta o de pagar licencia dentro de la reunión.
- [ ] Caso borde: la herramienta externa rechaza la identidad; el participante ve el mensaje en menos de 5 segundos y puede seguir viendo.

Traces to: insight 5 de las entrevistas (4 de 10: Tomás, Javier, Valeria Castro, Sofía) y survey Q6 y Q8 (con externos, 64% tarda 5 minutos o más en entrar).

### Saber qué se decidió y qué me toca
As Norma Benítez, I want recibir al terminar la reunión lo decidido, quién lo hace y para cuándo, so that no tengo que preguntarle a una compañera qué me tocó.

Acceptance criteria:
- [ ] Al cerrar la reunión, quien conduce revisa y confirma la lista (decisión, responsable, fecha y motivo) antes de que se envíe; nada se envía sin esa confirmación.
- [ ] La lista llega a cada participante por el chat de la reunión, y también por correo si lo tiene activado; no depende de que la busque en un lugar de Teams.
- [ ] Lo hablado pero no decidido aparece aparte y marcado como tal, nunca como decisión.
- [ ] Cada decisión sin responsable o sin fecha se marca como "incompleta" y frena la confirmación hasta que quien conduce la acepta así.
- [ ] Quien se desconectó durante la reunión recibe la misma lista.
- [ ] Caso borde: una reunión sin decisiones envía "no se registraron decisiones" y no una lista vacía.

Traces to: insights 1 y 2 de las entrevistas (10 de 10 con decisión mal ejecutada; 6 de 10 con resumen de IA que mezcla ideas con decisiones) y survey Q9 (24% sin registro). La necesidad de Norma proviene de la persona (sintética); quién confirma y por dónde llega viene de la crítica del panel (sintética).

*Nota de alcance:* esta historia coincide con la oportunidad adyacente "reuniones sin cierre de decisiones y responsables" (A3 `cierre-asistido`, en pausa), donde la evidencia real es más fuerte. Queda aquí para el piloto de este spec; si crece, se separa en su propio spec.

## Hypothesis
We believe los participantes que hoy miran la pantalla de otro o no logran entrar a la herramienta compartida van a señalar, comentar o editar durante la reunión cuando el contenido se abre para todos dentro de Teams con su identidad corporativa, porque hoy el costo de participar (dictar, crear una cuenta, pedir licencia) es mayor que el de callar.
We're wrong if en reuniones reales de más de 5 personas con una sesión asistida, **menos de la mitad** de los participantes que habían mirado sin tocar nada (de acuerdo con el facilitador o con el conductor) hacen al menos una marca, comentario o edición durante la reunión, o si **uno de cada cuatro** necesita ayuda o abandona por el acceso. *(Umbrales propuestos; a confirmar con el equipo.)*

## Tested before spec
Riskiest belief not tested (declared). Este spec no descendió de una exploración ni de un test.

Relación con A2 `abrir-como-app`, que sí tiene pruebas diseñadas en `product/tests/2026-10-12-1830-trabajo-en-vivo-fuera-de-teams.md` (T1, T2 y T3 sin correr hasta hoy):
- T1 (technical-test, acceso sin licencia adicional) cubre solo la historia "Entrar sin crear cuenta" para herramientas de tablero y una con inicio de sesión único. No hay resultado todavía.
- T2 (prototype-shown, aceptación del aviso) mide si el conductor acepta abrir como app. No cubre a quien mira.
- T3 corresponde a A1 `pizarra-persistente` y no aplica a este spec.
- Las historias "Ver lo mismo", "Señalar y opinar", "Decidir quién puede editar" y "Saber qué se decidió" no están cubiertas por ningún test.
- La revisión posterior a la crítica sumó el control del conductor, el aporte sin nombre y la confirmación de la lista. Son comportamientos que ningún test de A2 incluyó; el T2 mide solo si el conductor acepta el aviso.

## Assumptions
Ya registradas en `product/overview.md`:
- [feature: abrir-como-app] [value] #7 — los conductores que hoy pegan el enlace de una herramienta externa en el chat la abren como app cuando se les sugiere, en lugar de compartir pantalla.
- [feature: abrir-como-app] [feasibility] #8 — abierto como app, quienes hoy miran la pantalla de otro editan u opinan sin cuenta ni licencia adicional, incluidos invitados, otra instancia y cuentas personales.
- [product] [value] #2 — recurren a herramientas externas porque las nativas no cubren la necesidad, no por desconocimiento (`weakened`).

Nuevas, propuestas para el registro (pendientes de tu aprobación):
- [feature: seguir-trabajo-en-vivo] [value] quien mira sin poder tocar no opina durante la reunión y su objeción llega tarde o nunca. *(Evidencia real solo contada por otro: Valeria Castro, Martina Rojas; ninguna en primera persona.)*
- [feature: seguir-trabajo-en-vivo] [usability] los participantes de baja alfabetización técnica (Norma) señalan o comentan sin ayuda ni capacitación cuando el contenido se abre en la reunión.
- [feature: seguir-trabajo-en-vivo] [feasibility] el contenido de herramientas de terceros puede mostrarse a todos en el mismo estado (filtros y selección) y admitir marcas de participantes sin permiso de edición. — owner: Tech
- [feature: seguir-trabajo-en-vivo] [value] quien se pierde parte de una reunión usa la lista de decisiones con responsable y fecha en lugar de preguntarle a un compañero. *(Sin evidencia real; viene de la persona Norma.)*
- [feature: seguir-trabajo-en-vivo] [value] quienes conducen quieren ver quién está mirando sin poder participar. *(Sin evidencia: surge de la frase de Valeria Castro "En casi todas hay alguien mirando desde afuera".)*
- [feature: seguir-trabajo-en-vivo] [viability] mejorar la participación de quien hoy mira sube la retención en la renovación de cuentas medianas. *(Sin dato propio; hereda #5 y #1.)*

Agregadas por la crítica del panel, pendientes de tu aprobación para el registro (sintéticas):
- [feature: seguir-trabajo-en-vivo] [usability] quienes conducen eligen quién edita y confirman la lista de decisiones sin que les agregue trabajo respecto de lo que hacen hoy (Valeria: 2 h/semana reconstruyendo minutas).
- [feature: seguir-trabajo-en-vivo] [feasibility] el contenido compartido sigue respondiendo con 10 a 15 participantes y 3 editando a la vez. — owner: Tech
- [feature: seguir-trabajo-en-vivo] [usability] un primer aporte dirigido solo al conductor, o sin nombre, hace que participantes como Norma participen más que con la marca visible para todos.
