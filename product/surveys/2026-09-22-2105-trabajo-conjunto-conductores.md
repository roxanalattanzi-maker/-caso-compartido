---
opportunity: trabajo-en-vivo-fuera-de-teams
beliefs: "#6, #2"
audience: conductores
status: draft
---

# Survey: trabajo conjunto en reuniones — conductores

- **Objetivos de aprendizaje:**
  - **O1 (#6):** ¿En qué proporción de las reuniones de más de 5 personas el trabajo conjunto sale a una herramienta externa? ¿Cuánto tiempo semanal se dedica después a consolidar lo producido? → Define si el problema tiene tamaño suficiente para seguir con la oportunidad. El umbral de la creencia es ≥1 de cada 3 reuniones y ≥1 h/semana.
  - **O2 (#2):** Entre quienes sacan el trabajo afuera, ¿probaron las funciones nativas (notas de reunión/Loop, Whiteboard) y no alcanzaron, o no las conocían? → Define si la solución apunta a desempeño/capacidad (no alcanzan) o a descubrimiento/adopción (no las conocían).
- **Encuestados objetivo:** Team Leads y mandos medios que convocan o conducen reuniones de Teams de más de 5 personas, en organizaciones de 100 a 1.000 licencias M365 (segmento de la oportunidad; persona primaria: Valeria Quiroga).
- **Canal:** mail. La lista de envío se arma con datos propios: usuarios de cuentas de 100 a 1.000 licencias que organizaron al menos una reunión de más de 5 participantes en las últimas 2 semanas. Por eso no se pregunta el tamaño de la organización.
- **Identificador de cuenta:** el enlace de cada mail lleva un identificador de cuenta (parámetro oculto, no una pregunta). Sirve para cruzar las respuestas con el % de reuniones con enlaces externos y con el resultado de la renovación de esa cuenta. El mail de invitación tiene que avisar que las respuestas se asocian a la organización.
- **Registro del envío:** anotar la cantidad de mails enviados para poder informar la tasa de respuesta. Los que responden se seleccionan solos (sesgo de autoselección): probablemente responden más los que tienen el problema.
- **Filtro:** S1 confirma el rol (la lista sale de telemetría, pero puede haber organizadores que no conducen).
- **Duración estimada:** 9 preguntas + bloque de reclutamiento, ~5 min.
- **Límite conocido:** no hay trabajo cualitativo real previo. Las opciones de Q1, Q3 y Q6 salen de las personas sintéticas y del research de mercado. Por eso todas tienen "Otro" y hay una pregunta abierta, que sirve para detectar lo que falte.

## Filtro

S1. En las últimas 2 semanas, ¿cuántas reuniones de Teams con más de 5 participantes convocaste o condujiste vos? [opción única]
   - Ninguna
   - 1 o 2
   - 3 a 5
   - 6 a 10
   - Más de 10
   → descalificar si "Ninguna"
   > Objetivo: filtro de rol (conduce reuniones grandes); también es denominador de Q2

## Preguntas

Q1. Pensá en la **última** reunión de más de 5 personas que condujiste en la que el grupo tenía que producir algo en conjunto (planificar, priorizar, redactar, armar una lista de tareas). ¿Dónde se hizo ese trabajo? [opción múltiple]
   - Compartiendo pantalla: una persona editaba y el resto miraba
   - En el chat de la reunión
   - En las notas de la reunión de Teams o en un componente Loop
   - En Whiteboard de Teams
   - En un archivo de Word, Excel o PowerPoint que editaban varias personas a la vez
   - En una herramienta fuera de Microsoft 365 (Miro, Mural, FigJam, Notion, Google Docs, Jira u otra)
   - En esa reunión no se produjo nada en conjunto
   - Otro: ___
   > Objetivo: O1. Toma el último caso concreto, que se recuerda con menos sesgo que un promedio.

Q2. De las reuniones de más de 5 personas que condujiste en las últimas 2 semanas (las que contaste en S1), ¿en cuántas el trabajo conjunto se hizo en una herramienta fuera de Microsoft 365? [opción única]
   - En ninguna
   - En pocas (menos de 1 de cada 3)
   - En 1 de cada 3 o más, pero menos de la mitad
   - En la mitad o más, pero no en todas
   - En todas
   > Objetivo: O1. Contrasta directamente el umbral de #6 (≥1 de cada 3).

Q3. *(Mostrar si Q2 ≠ "En ninguna")* ¿Qué herramientas fuera de Microsoft 365 usaron en esas reuniones? [opción múltiple]
   - Miro
   - Mural
   - FigJam
   - Notion
   - Google Docs / Sheets / Slides
   - Jira
   - Trello o Asana
   - Otra: ___
   > Objetivo: O1. Además, cruza con lo que IT declara pagar por fuera (survey de IT).

Q4. En una semana típica, ¿cuánto tiempo dedicás después de las reuniones a juntar lo que se produjo? Por ejemplo, pasar acuerdos o tareas de un lugar a otro, armar la minuta o avisar a los responsables. [opción única]
   - Nada
   - Menos de 30 minutos
   - Entre 30 y 59 minutos
   - Entre 1 y 2 horas
   - Más de 2 horas
   > Objetivo: O1. Contrasta el umbral de #6 (≥1 h/semana).

Q5. Para cada función de Teams, ¿qué frase describe mejor tu experiencia? [matriz, opción única por fila]
   - Filas: Notas de la reunión / Loop · Whiteboard
   - Columnas: No sabía que existía · Sabía que existía, pero nunca la probé · La probé y dejé de usarla · La uso a veces · La uso habitualmente
   > Objetivo: O2. Separa "no conocía" de "probó y no alcanzó".

Q6. *(Mostrar si en Q5 marcó "nunca la probé" o "la probé y dejé de usarla" en alguna fila)* ¿Qué te llevó a no usarla o a dejar de usarla? [opción múltiple]
   - Se trabó o anduvo lenta con varias personas editando
   - A los participantes les costó entrar o editar
   - Le faltaba algo que sí tiene otra herramienta
   - El equipo ya trabajaba en otra herramienta
   - Lo que se producía no quedaba donde lo necesitaba después
   - No sabía cómo usarla durante la reunión
   - Preferí no arriesgarme a que fallara frente al equipo
   - No me acuerdo
   - Otro: ___
   > Objetivo: O2. Cuantifica motivos; el "por qué" en profundidad queda para las entrevistas.

Q7. ¿Qué es lo más difícil de lograr que una reunión de más de 5 personas termine con algo producido en conjunto? [abierta, no obligatoria]
   > Objetivo: O1/O2. Detecta motivos y comportamientos que las opciones cerradas no cubren.

Q8. ¿Cuál describe mejor tu rol? [opción única]
   - Team Lead / líder de equipo
   - Gerente o jefe de área
   - Director o superior
   - Colaborador/a que a veces conduce reuniones
   - Otro: ___
   > Objetivo: segmentación del análisis

## Filtro + opt-in (reclutamiento para entrevistas)

R1. ¿Trabajás en IT, sistemas o en la administración de Microsoft 365 de tu organización? [sí / no]
   → no es candidato si "sí" (ese perfil se entrevista por el survey de IT)

R2. ¿Aceptarías una conversación de 30 minutos sobre cómo trabajan en conjunto en tus reuniones? [sí / no]

R3. Si respondiste que sí, ¿cómo te contactamos? [abierta, opcional — solo si R2 = sí]
