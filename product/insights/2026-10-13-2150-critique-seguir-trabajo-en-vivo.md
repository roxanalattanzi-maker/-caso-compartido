---
date: 2026-10-13
source: synthetic
document: product/specs/2026-10-13-2125-seguir-trabajo-en-vivo.md
panel: valeria-quiroga, norma-benitez
---

# Crítica del spec "Seguir el trabajo en vivo"

**Panel:** 2 personas sintéticas: 1 primaria (Valeria Quiroga) y 1 terciaria (Norma Benítez). Sin voz negativa: el spec toca permisos de edición y alcance, y no tiene a nadie que diga "esto no es para mí". Ver límites al final.

**Procedencia:** todo lo de este archivo es `synthetic`. Ninguna cita es de una persona real y no cuenta como evidencia de que el spec funcione.

---

### Valeria Quiroga — Team Lead de Operaciones Comerciales · primaria

**Overall rating:** 3/5

**Strengths:**
- Reconoce el dolor de la historia 1: "uno maneja y el resto dicta" es lo que pasa en mis revisiones de ventas, y me pasó discutir números distintos porque cada uno tenía otro filtro.
- Que el contenido se abra dentro de la reunión sin que nadie cree una cuenta me ahorra explicar el acceso al principio, que es donde se me van los primeros minutos.
- Me gusta la historia 4. Si la reunión termina con decisión, responsable y fecha, me ahorra buena parte de mis 2 horas semanales reconstruyendo minutas.

**Concerns:**
- **Más gente tocando, más accidentes.** Si todos pueden editar el ticket o la planilla, alguien va a cerrar el que no es. El spec dice quién puede editar, pero no dice quién decide eso. Yo convoco; yo respondo por lo que quede.
- **La historia que más me sirve es la más floja.** La lista de decisiones no dice quién la arma ni de dónde sale. Si es el resumen de IA, igual lo tengo que revisar, y entonces no me ahorra nada. Y si marca como decisión algo que era una idea, es peor que no tener nada.
- **Si falla una vez frente al equipo, no la vuelvo a usar.** Los criterios no hablan de rendimiento ni de qué pasa con 12 o más personas. La pizarra se me trabó con 8 y nunca más la intenté.
- **No reemplaza nada que yo use.** Seguiría pegando el link de Miro o Notion; esto solo cambia cómo lo veo. No veo a qué le gana en mi día a día, salvo en las reuniones donde hay gente que mira.
- Falta mi parte: el spec está contado desde Norma, y yo conduzco. No dice qué veo yo cuando alguien mira y no participa.

**Suggestions:**
- Que quien conduce decida quién puede editar, con "señalar y comentar" como valor por defecto, y que las ediciones se puedan deshacer o se vean quién las hizo.
- Definir de dónde sale la lista de decisiones: yo la confirmo antes de que se envíe, o la armo marcando durante la reunión. Una decisión sin responsable o sin fecha debería frenarme, no pasar.
- Agregar un criterio de rendimiento con la cantidad de gente de mis reuniones reales (10 a 15).
- Darme una vista de quién está mirando sin participar. Eso sí lo usaría.

Si solo anda la parte de "ver lo mismo", la tomo. Si me traen la lista de decisiones bien hecha, la peleo. Hoy el spec promete las dos y define una.

---

### Norma Benítez — Analista administrativa de cuentas a pagar · terciaria

**Overall rating:** 3/5

**Strengths:**
- Que no me pidan crear una cuenta. Hoy cuando mandan un link no sé si tengo que registrarme y termino sin abrirlo. Si se abre dentro de la reunión, con mi usuario de siempre, ya no tengo que decidir nada.
- Ver lo mismo que ve el que maneja. Me desconecto cuando no sigo lo que están mirando, y ahí no hay vuelta.
- La lista al final de "qué se decidió y qué me toca". Eso es lo que le pido a una compañera después de casi todas las reuniones largas.

**Concerns:**
- **Que aparezca mi nombre.** Si marco algo y todos ven "Norma" ahí, quedo expuesta. Yo casi no hablo en las reuniones grandes, y menos si no estoy segura de si lo que veo es lo correcto. Tengo miedo de tocar algo y romperlo.
- **Una cosa más que aprender.** Cada cambio de pantalla me desorienta semanas. "Modo solo ver", "señalar", "comentar": no sé cuál tengo que usar, y si me equivoco frente a todos, mejor no hago nada.
- **¿Dónde está la lista?** Cuando me comparten algo "en el canal", al día siguiente no lo encuentro. Si la lista queda en un lugar de Teams que no conozco, no la voy a ver. No uso las notas de reunión ni busco cosas ahí.
- **Los errores.** "Caso borde: el participante ve el mensaje en 5 segundos". Si el mensaje dice algo técnico, yo lo leo como "rompí algo".

**Suggestions:**
- Que la lista me llegue sola, por el chat o por correo, que es donde ya miro, sin tener que ir a buscarla.
- Que pueda hacerle una pregunta al conductor sin que se vea para todos, o que el aporte pueda ser anónimo al principio.
- Que no haya nada nuevo que elegir: que el contenido se abra y yo vea lo mismo, y que lo de señalar o comentar aparezca recién cuando intento tocar.
- Mensajes cortos y en palabras comunes: "Podés mirar y comentar. Para editar, pedile permiso a Valeria".

No pido cosas nuevas; pido que sea más simple. Si esto me deja ver lo mismo que los demás y me manda lo que me toca, lo agradezco. Si me suma botones, me va a costar.

---

## Síntesis del panel (como investigadora, no en personaje)

### Puntos de acuerdo
1. **Las dos quieren control antes que más libertad.** Valeria quiere decidir quién edita para evitar accidentes; Norma quiere no tener que decidir nada frente a todos. En los dos casos el valor por defecto importa más que la capacidad.
2. **La lista de decisiones es lo más valioso y lo menos definido.** Las dos la señalan como lo que más les sirve; ninguna confía en que salga bien sola. Valeria pide validarla; Norma pide que le llegue donde ya mira.
3. **Ninguna pide una herramienta nueva.** Las dos quieren que esto sea parte de lo que ya hacen, sin vocabulario ni pasos nuevos.

### Conflictos (decisiones de diseño)
- **Visibilidad de quién mira.** Valeria quiere ver quién está mirando sin participar; Norma no quiere que se vea su nombre cuando marca. Decisión: ¿la conductora ve nombres, ve solo cantidad o ve que alguien lleva rato sin interactuar? Esto toca la privacidad de participantes.
- **Control del conductor vs. autonomía del participante.** Si el conductor decide quién edita (pedido de Valeria), Norma depende de que se lo permitan, y "pedile permiso" en voz alta es justo lo que le cuesta.
- **Riqueza vs. simplicidad.** Valeria evalúa por lo que hace; Norma, por lo que no cambia. El mismo modo "señalar, comentar, editar" sirve a una y complica a la otra.

### Los 2 o 3 cambios de mayor impacto
1. **Agregar al spec un rol de control y valores por defecto.** El conductor decide quién edita; por defecto, "mirar y comentar". Sumar criterios de deshacer o de ver quién hizo una edición, y un criterio de rendimiento con 10 a 15 personas. Es lo que más reduce el riesgo para Valeria y lo que menos le exige a Norma.
2. **Definir la lista de decisiones o sacarla a otro spec.** Falta decir quién la arma, quién la confirma y por dónde llega. Además es la oportunidad adyacente del cierre de decisiones, donde la evidencia real es más fuerte (10 de 10 entrevistas). Mezclarla con "seguir en vivo" diluye las dos. Si se queda, que llegue por chat o correo y que lo no decidido se marque aparte.
3. **Bajar la exposición de quien participa.** Dejar que el primer aporte sea sin nombre o dirigido al conductor, y que "señalar y comentar" aparezca cuando se intenta tocar. Esto responde a la preocupación de Norma sin quitar nada de lo que pide Valeria.

### Para el spec
- El spec llama a Valeria "secundaria", pero su archivo de persona dice `primaria`. Conviene alinear uno de los dos.
- Faltan en los criterios: rendimiento con 10 a 15 personas, deshacer ediciones y cómo se decide quién edita.
- La historia 4 y el supuesto #13 siguen sin evidencia real. Esta crítica no los respalda: Valeria y Norma son sintéticas.

### Límites de la crítica
Dos personas sintéticas. Faltan Marcelo (secundaria, firma la renovación) y una voz negativa (Tomás), que diría hasta dónde este spec se acerca a un territorio que ya cubren Miro o Notion. El panel mide qué les preocupa, no qué harían.
