---
status: framed
segment: Team Leads y mandos medios que conducen reuniones de más de 5 personas en cuentas medianas de M365 (100–1.000 licencias)
personas: valeria-quiroga, norma-benitez, marcelo-ferreyra, tomas-lindqvist
---

# Oportunidad: El trabajo conjunto de las reuniones se hace fuera de Teams

En cuentas medianas, cuando una reunión de más de 5 personas tiene que producir algo en conjunto (planificar, priorizar, redactar), quien conduce saca ese trabajo a Miro, Notion, Google Docs o Jira, y lo producido queda fragmentado fuera de la reunión y del perímetro M365. Ahora, porque "el equipo ya usa otras herramientas" y "pagamos por funciones que no usamos" están entre los motivos de baja, y CollabCon llega en 5 meses.

## Segmento y personas
- **Valeria Quiroga** (primaria) — **lo sufre**: usa Miro porque Whiteboard se trabó con 8 editores; acciones dispersas entre chat, Notion y Jira; ~2 h/semana reconstruyendo minutas.
- **Norma Benítez** (terciaria) — **lo sufre de rebote**: no abre los links de Miro/Docs por no saber si debe crear cuenta; queda afuera del trabajo en vivo.
- **Marcelo Ferreyra** (secundaria) — **no lo sufre en la reunión**, pero paga su costo: tres áreas pagan Miro/Notion por fuera, datos de clientes fuera del perímetro, no puede justificar la licencia. Responde la creencia de viabilidad (firma la renovación).
- **Tomás Lindqvist** (negativa) — **no lo sufre**: usa Miro/Notion por elección y no tiene M365. Fuera de alcance; si su feedback justifica algo, es señal de alerta.
- **Falta:** ninguna. Útil como contraste (opcional): un conductor de cuenta mediana que *sí* usa Whiteboard/notas nativas.

## Señales
| Señal | Procedencia | Fuente |
|---|---|---|
| 29% de reuniones de más de 5 participantes comparte en el chat un enlace externo (Docs, Notion, Miro, Mural, FigJam, Jira) | real | product/overview.md — datos de uso |
| Whiteboard 5%, notas de reunión 8% de uso en reuniones | real | product/overview.md — datos de uso |
| 41% de las reuniones tiene más de 8 participantes | real | product/overview.md — datos de uso |
| 19% de quejas post-reunión: "colaboración durante la reunión" | survey (n no informado) | product/overview.md — encuestas post-reunión |
| Motivos de baja: #1 "pagamos por funciones que no usamos", #3 "el equipo ya usa otras herramientas" (sin especificar) | real | product/overview.md — motivos de baja/no renovación |
| 37% de organizaciones con Slack o Google Chat activo además | real | product/overview.md — datos de uso |
| Whiteboard se traba con 8 editores; se usa Miro vía link | synthetic | product/personas/valeria-quiroga.md |
| Shadow IT: áreas que pagan Miro/Notion con tarjeta corporativa | synthetic | product/personas/marcelo-ferreyra.md |
| Participantes que no abren el link externo | synthetic | product/personas/norma-benitez.md |

## Resultado de negocio
**Retención en la renovación** de cuentas medianas (reducir el 3,6% que baja de plan o no renueva). Se observan además, como métricas de la dirección: tasa de upgrade a Max e ingresos por licencia.

## Restricciones
- Presupuesto máximo: USD 5M.
- Los features se presentan en CollabCon, dentro de 5 meses (≈ fines de febrero 2027).
- Métricas de la dirección para el segmento: upgrade a Max, retención en la renovación, ingresos por licencia.
- Límites para cualquier solución: facilidad de uso, accesibilidad, compatibilidad con Microsoft 365, privacidad y seguridad corporativas, tiempo real, impacto mínimo en el rendimiento de la reunión.

## Creencias
Registro único: product/overview.md.
- #2 [product] [value] — recurren a herramientas externas porque las nativas no cubren la necesidad, no por desconocimiento. *Esta oportunidad depende de ella.*
- #1 [product] [viability] — el salto Premium→Max no está anclado a valor percibido. *Relacionada lateralmente.*
- #5 [opportunity: trabajo-en-vivo-fuera-de-teams] [viability] — shadow IT en cuentas medianas con reuniones con enlaces externos, que IT quiere eliminar, y mayor downgrade/no renovación en esas cuentas.
- #6 [opportunity: trabajo-en-vivo-fuera-de-teams] [value] — el trabajo conjunto sale a herramientas externas en ≥1 de cada 3 reuniones de más de 5 personas, con ≥1 h/semana de consolidación posterior.

## Agenda de investigación
| Creencia | Instrumento (del más barato al más caro) | Decisión que habilita | Para cuándo |
|---|---|---|---|
| #5 viability | 1) Datos propios: cruzar % de reuniones con enlaces externos por cuenta vs. downgrade/no renovación en cuentas medianas | Seguir o descartar la oportunidad como palanca de retención | 9 oct 2026 |
| #5 viability | 2) /research-market: gasto típico en Miro/Notion/Docs dentro de empresas M365 y tendencias de consolidación | Dimensionar el costo duplicado que IT recuperaría | 9 oct 2026 |
| #6 value + #2 | 3) /design-survey a conductores de cuentas medianas: frecuencia, horas de consolidación, motivo (no cubre vs. no conocía); con bloque de opt-in | Confirmar el problema y separar "no cubre" de "no conocía" | 30 oct 2026 |
| #5 viability | 3b) Preguntas del survey para IT: herramientas pagadas por fuera e intención de eliminarlas en la renovación | Sostener la viabilidad con compradores | 30 oct 2026 |
| #6 value | 4) /design-interview entre opt-ins, priorizando a quienes contradigan la creencia: qué hacen hoy y por qué | Pasar a /clarify-idea con un problema validado | 13 nov 2026 |
| — | Punto de decisión: ¿el problema se sostiene? | Sin esta decisión no hay margen de construcción antes de CollabCon | 20 nov 2026 |

## Ideas candidatas (no evaluadas)
- "Herramientas colaborativas integradas en la reunión" — la forma en que llegó el pedido.
- Oportunidades adyacentes (no enmarcadas aquí): reuniones sin cierre de decisiones y responsables; participantes que no pueden seguir el trabajo en vivo.
