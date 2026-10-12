# T1 · abrir-como-app: hoja de captura

**Prueba:** `product/tests/2026-10-12-1830-trabajo-en-vivo-fuera-de-teams.md`, T1
**Creencia (#8):** abierto como app en la reunión, quienes hoy miran la pantalla de otro editan u opinan sin cuenta ni licencia adicional, incluidos invitados, usuarios de otra instancia y cuentas personales.
**Quién la completa:** tech. **Plazo:** hasta 3 días hábiles, a confirmar con tech.
**Participantes:** ninguno. Las cuentas de cada escenario las crea tech en el tenant de prueba. Provenance de los resultados: `real` (medición técnica, no de usuarios).

## Datos de la corrida

| Campo | Valor |
|---|---|
| Fecha | |
| Quién ejecutó | |
| Tenant de prueba de Teams | |
| Herramienta de tablero (sin inicio de sesión único) | |
| Versión de la app de Teams de esa herramienta | |
| Herramienta de control (con inicio de sesión único corporativo) | |
| Versión de la app de Teams del control | |

## Cómo se ejecuta cada escenario

1. Abrir una reunión de Teams con el anfitrión (cuenta interna con licencia plena de la herramienta).
2. El anfitrión abre la herramienta **como app dentro de la reunión**.
3. Entrar a la reunión con la cuenta del escenario y, sin ayuda previa, intentar **editar** (cambiar o agregar un elemento) y **comentar**.
4. Registrar abajo qué pasó, incluidos los pasos extra que la herramienta exigió.

## Escenarios en la herramienta de tablero

| Escenario | Cuenta usada (describir) | ¿Edita? (sí/no) | ¿Comenta? (sí/no) | Pasos extra exigidos (ninguno / crear cuenta / pedir licencia / otro: cuál) | ¿Pasa? | Nota libre |
|---|---|---|---|---|---|---|
| (a) Usuario interno sin licencia de la herramienta | | | | | | |
| (b) Invitado externo a la organización | | | | | | |
| (c) Usuario de otra instancia de la herramienta | | | | | | |
| (d) Usuario con cuenta personal (por ejemplo, Google) | | | | | | |

**Un escenario pasa solo si** edita o comenta (al menos una de las dos es "sí") **y** los pasos extra son "ninguno". Si pidió crear cuenta, pedir licencia u otro paso, no pasa, aunque después haya podido editar.

## Control en la herramienta con inicio de sesión único

| Escenario | Cuenta usada (describir) | ¿Edita? (sí/no) | ¿Comenta? (sí/no) | Pasos extra exigidos | ¿Pasa? | Nota libre |
|---|---|---|---|---|---|---|
| Participante interno con inicio de sesión único corporativo | | | | | | |

El control pasa si edita o comenta con pasos extra "ninguno".

## Lectura del resultado (se completa al terminar)

| Medida | Valor |
|---|---|
| Escenarios que pasan en la herramienta de tablero (de 4) | |
| ¿Pasa el control? (sí/no) | |

Umbral fijado en el diseño, sin cambios: **≥3 de 4 escenarios y control correcto**.
