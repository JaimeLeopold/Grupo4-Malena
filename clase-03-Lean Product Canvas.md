# Lean Product Canvas — SeñaSegura

> Este canvas contiene hipótesis. La evidencia surgirá de observar y experimentar.

---

## Paso 1 — Revisión de la evidencia de Clase 2

| Elemento | Respuesta del equipo |
|---|---|
| Problema priorizado en Clase 2 | Inseguridad transaccional (miedo a estafas y a recibir réplicas) al comprar indumentaria importada a revendedores informales. |
| Evidencia que lo respalda | Comportamiento observable en grupos de Facebook ("Legit Check Arg"), foros de moda y comentarios de Instagram donde se exigen fotos de etiquetas, costuras y tickets antes de pagar. |
| Contradicciones encontradas | Los usuarios buscan el mercado informal para ahorrar dinero, pero exigen el mismo nivel de garantías que el retail oficial. |
| Supuestos que permanecen | Que mostrar el ticket de compra original elimina la desconfianza — **todavía no validado**; el role-play sugiere que el miedo real podría ser financiero (perder la seña) y no solo la autenticidad de la prenda. |
| Cambios realizados al problema | Se pasó de "miedo a las réplicas" a un problema más amplio: "inseguridad por falta de pruebas de origen y reputación del vendedor", y luego, tras el role-play, se identificó un posible sub-problema no explorado: el miedo a transferir dinero por adelantado. |
| Usuarios entrevistados | Pendiente: el plan de Clase 2 definió 4 entrevistas mínimas (guion real ya diseñado); **marcar como no ejecutadas todavía si el equipo aún no las realizó**. |
| Comportamientos observados | Revisión de seguidores/comentarios del vendedor, pedido de fotos de etiquetas y costuras, pedido de medidas en centímetros, consulta en foros de verificación antes de pagar. |
| Alternativas actuales | Subir fotos a foros para validación de terceros, pagar de más en tienda oficial, pedirle a conocidos que viajan que traigan la prenda. |

**Nota del equipo:** como las entrevistas reales de Clase 2 todavía no están confirmadas como completas en el material recibido, todo el contenido de este canvas que dependa de ellas se marca explícitamente como **Supuesto** hasta que se registre evidencia real.

---

## 1. Problema de negocio

Los estudiantes universitarios argentinos que compran indumentaria de marca a revendedores informales (como nuestro propio equipo) tienen dificultad para confiar en la autenticidad del producto y en la seriedad del vendedor al momento de pagar una seña por adelantado, lo que genera abandono de compra, ciclos de venta muy largos y pérdida de ventas para quienes revendemos.

Lo sabemos por el comportamiento repetido y observable en grupos como "Legit Check Arg" y en comentarios de Instagram, donde los compradores exigen múltiples pruebas antes de comprometerse a pagar.

Todavía necesitamos comprobar si el freno principal es el miedo a recibir una réplica o el miedo a perder el dinero transferido por adelantado a un desconocido — esto surgió como contradicción no resuelta en el role-play de personas sintéticas de Clase 2.

*(Redacciones alternativas consideradas por el equipo, según el prompt sugerido de la guía: una centrada en el usuario, una centrada en el impacto del negocio y esta versión integrada, que fue la elegida por conectar ambas partes sin proponer todavía una solución.)*

---

## 2. Resultados de negocio

- Reducir el **tiempo del ciclo de venta** (desde el primer contacto hasta el pago de la seña), desde *pendiente de medir* hasta reducirlo significativamente en 8 semanas.
- Aumentar la **tasa de conversión de seña** (comprador que confirma y transfiere el adelanto sobre el total de conversaciones iniciadas), desde *pendiente de medir* hasta un objetivo a definir tras el experimento mínimo.
- Reducir el **abandono de compra en la etapa de pago** (usuarios que preguntan, piden pruebas y luego desaparecen), desde *pendiente de medir* hasta *pendiente de definir*.

*(No se define línea de base porque el equipo todavía no cuenta con datos propios de ventas; se marca como pendiente de medir según indica la guía.)*

---

## 3. Usuarios y clientes

| Rol | Definición | Fuente |
|---|---|---|
| **Usuario** | Estudiante argentino que busca comprar ropa de marca importada a un revendedor informal (por ejemplo, en Instagram). | Evidencia de Clase 2. |
| **Cliente** | El mismo comprador (es quien paga la seña y el saldo). | Evidencia de Clase 2. |
| **Decisor** | El propio comprador decide si transfiere o abandona. | Interpretación del equipo — pendiente de confirmar en entrevistas. |
| **Influenciador** | Comunidades de verificación ("Legit Check Arg"), amigos que ya compraron antes, comentarios públicos en las publicaciones. | Evidencia de Clase 2. |
| **Rol pendiente** | El revendedor (nuestro propio rol) podría convertirse en cliente si la solución se ofrece como herramienta paga para vendedores; **pendiente de investigación**, no fue objeto de las entrevistas de Clase 2. |

---

## 4. Necesidades y resultados del usuario

- Cuando tengo que transferir una seña a un revendedor que no conozco antes de recibir la prenda, quiero tener alguna garantía de que mi dinero está protegido, para animarme a concretar la compra sin miedo a perderlo. *(Supuesto — surge del role-play, no de entrevistas reales todavía.)*
- Cuando encuentro una prenda publicada por un revendedor, quiero confirmar rápido que es original y que el vendedor es serio, para no perder tiempo pidiendo pruebas manualmente en cada conversación. *(Evidencia: comportamiento observado en foros y comentarios de Clase 2.)*

Ambas frases describen progreso del usuario, no una herramienta específica, y siguen siendo válidas aunque cambie la solución elegida en la Caja 5.

---

## 5. Ideas de solución

Tres alternativas generadas siguiendo los tres enfoques de la guía (información/decisión, coordinación/transacción, automatización/inteligencia):

### Alternativa 1 — Perfil de confianza del vendedor (Información/decisión)
- Propuesta: perfil digital del revendedor con historial de ventas, fotos de tickets ya verificadas y reseñas centralizadas.
- Valor: reduce el tiempo de investigación manual en foros externos.
- Tecnología central: perfil web/app con reputación acumulada.
- Datos necesarios: historial de transacciones, reseñas, fotos subidas por el vendedor.
- Riesgo principal: requiere que haya suficiente volumen de vendedores activos para que el historial sea útil (problema de arranque en frío).
- Prototipo: página estática o Notion/Airtable público con perfil de ejemplo.

### Alternativa 2 — SeñaSegura: pago de la seña con liberación condicionada (Coordinación/transacción)
- Propuesta: un flujo de pago donde la seña queda retenida y se libera al vendedor solo cuando el comprador confirma la recepción de la prenda.
- Valor: ataca directamente el miedo a transferir dinero a un desconocido, sin depender de que la prenda "parezca" original.
- Tecnología central: checkout de pago (ej. Mercado Pago) con lógica de retención/confirmación manual en el MVP.
- Datos necesarios: monto de la seña, confirmación de entrega del comprador, datos de contacto de ambas partes.
- Riesgo principal: sin ser una plataforma registrada, retener fondos de terceros puede tener límites legales u operativos; en el MVP la "retención" tendría que simularse (ej. el equipo actúa como intermediario manual).
- Prototipo: landing + bot de WhatsApp que explica el flujo y linkea a un pago, sin automatizar todavía la liberación.

### Alternativa 3 — Verificador automático de autenticidad por foto (Automatización/inteligencia)
- Propuesta: un asistente que analiza las fotos de etiquetas, costuras y código de artículo que sube el vendedor y devuelve una probabilidad de autenticidad.
- Valor: reemplaza la validación manual en foros de "Legit Check" por una respuesta inmediata.
- Tecnología central: modelo de clasificación de imágenes o un asistente de IA que compara contra referencias públicas de la marca.
- Datos necesarios: banco de imágenes de productos originales por marca y modelo, fotos del vendedor.
- Riesgo principal: la exactitud del modelo es incierta y una falsa sensación de seguridad podría ser peor que no tener verificación (además no resuelve el miedo financiero detectado en el role-play).
- Prototipo: probar manualmente con un asistente de IA (prompt + fotos) antes de pensar en un modelo propio.

### Selección del equipo

```markdown
## 5. Ideas de solución

### SeñaSegura — pago de seña con liberación condicionada

- Propuesta: flujo digital donde la seña se retiene y se libera al vendedor
  solo cuando el comprador confirma haber recibido la prenda tal como fue
  publicada.
- Valor para el usuario: elimina el miedo a transferir dinero a un
  desconocido sin garantías, que el role-play de Clase 2 identificó como
  posible freno principal (todavía sin confirmar con entrevistas reales).
- Tecnología central: checkout de pago (Mercado Pago u otro) + bot/landing
  que gestiona la confirmación de entrega.
- Datos necesarios: monto de la seña, confirmación del comprador,
  seguimiento de la conversación.
- Riesgo principal: viabilidad legal/operativa de retener fondos de
  terceros sin ser una plataforma registrada.
- Prototipo inicial: landing + bot de WhatsApp simulando el flujo, con
  liberación manual gestionada por el equipo durante el experimento.
- Dependencias: cuenta de pago (Mercado Pago u otra), disponibilidad del
  equipo para mediar manualmente durante el MVP.
- Estado: idea no validada.
```

**Por qué se eligió esta y no las otras:** la Alternativa 1 no resuelve el miedo financiero detectado en el role-play (solo ataca la duda de autenticidad) y depende de tener muchos vendedores para ser útil. La Alternativa 3 tampoco resuelve el miedo financiero y su precisión es incierta. La Alternativa 2 ataca directamente la contradicción más riesgosa que dejó Clase 2: que el verdadero freno podría no ser la réplica sino la plata transferida sin garantías.

---

## 6. Hipótesis principales

### Hipótesis de problema

Creemos que los compradores abandonan la compra principalmente por miedo a transferir dinero por adelantado a un vendedor desconocido, más que por miedo a recibir una réplica.
Lo sabremos si, al preguntar directamente por el "momento de quiebre" en entrevistas o encuestas, la mayoría menciona el momento de la transferencia y no la revisión de fotos o etiquetas.

### Hipótesis de valor

Creemos que ofrecer una seña con liberación condicionada a la confirmación del comprador aumentará su disposición a pagar por adelantado.
Lo sabremos si, en la prueba, una proporción relevante de compradores prefiere este flujo frente a la transferencia directa tradicional.

### Hipótesis de comportamiento

Creemos que los compradores estarán dispuestos a completar un flujo de pago a través de un link o bot en lugar de una transferencia bancaria directa al vendedor.
Lo sabremos si una parte significativa de quienes reciben el link llega a iniciar el pago (no solo a leer la propuesta).

### Hipótesis de factibilidad

Creemos que podemos simular la retención y liberación de la seña de forma manual (sin infraestructura legal propia) durante el MVP, usando un checkout existente y coordinación directa del equipo.
Lo sabremos si logramos completar al menos un ciclo de compra de prueba de punta a punta sin errores de pago ni reclamos de ninguna de las dos partes.

---

## 7. Lo más importante por aprender

| Hipótesis | Incertidumbre 1–5 | Impacto 1–5 | Prioridad | Justificación |
|---|---:|---:|---:|---|
| Problema | 5 | 5 | 1 | Es una contradicción sin resolver desde Clase 2: no sabemos si el freno real es la réplica o el dinero. Si nos equivocamos acá, toda la solución apunta al problema incorrecto. |
| Valor | 3 | 4 | 2 | Depende directamente de la respuesta a la hipótesis de problema; no tiene sentido probarla antes. |
| Comportamiento | 3 | 3 | 3 | Importante, pero solo relevante si la hipótesis de valor se confirma primero. |
| Factibilidad | 4 | 3 | 4 | Riesgo real (retener fondos de terceros), pero solo vale la pena resolverlo si el problema y el valor ya están confirmados. |

### Caja 7

```text
¿Es el miedo a transferir dinero por adelantado a un desconocido —y no
el miedo a recibir una réplica— el verdadero motivo por el que los
compradores abandonan la compra antes de pagar la seña?
```

---

## 8. Experimento mínimo

- **Hipótesis que prueba:** Hipótesis de problema.
- **Objetivo:** determinar si el miedo financiero (transferir sin garantías) pesa más que el miedo a la réplica en el abandono de la compra.
- **Tipo de experimento:** encuesta dirigida + entrevistas cortas de seguimiento (no se construye ningún prototipo todavía, porque primero hay que confirmar cuál es el problema correcto).
- **Herramienta:** formulario digital (Google Forms) distribuido por WhatsApp/Instagram, más 2-3 entrevistas cortas de profundización usando el guion ya diseñado en Clase 2.
- **Participantes:** entre 15 y 20 estudiantes que compraron o intentaron comprar ropa importada a revendedores en los últimos 6 meses (distintos de los ya entrevistados en Clase 2, para no repetir sesgo de muestra).
- **Duración:** 5 días.
- **Tarea:** responder una pregunta de elección forzada sobre cuál fue el motivo principal de abandono en su último intento de compra frustrado, y ordenar sus miedos de mayor a menor.
- **Datos necesarios:** respuestas cuantitativas de la encuesta y comentarios cualitativos abiertos.
- **Métrica:** porcentaje de encuestados que señalan "miedo a transferir sin garantías" como motivo principal, frente al porcentaje que señala "miedo a la réplica".
- **Criterio de éxito:** si el 60% o más señala el miedo financiero como motivo principal, se confirma que la solución debe orientarse hacia un mecanismo de pago seguro (Alternativa 2) antes que hacia verificación de autenticidad.
- **Criterio de fracaso:** si el miedo a la réplica sigue siendo predominante (60% o más), o si el resultado queda empatado sin un patrón claro, se debe replantear la hipótesis de problema y reconsiderar si SeñaSegura es la solución correcta.
- **Aprendizaje esperado:** cuál de los dos miedos debe ser el foco real del MVP, antes de invertir en construir cualquier flujo de pago.
- **Limitaciones:** muestra pequeña y no representativa de todo el universo de compradores; sesgo de memoria al preguntar de forma retrospectiva; la encuesta mide intención/percepción declarada, no comportamiento real de pago, por lo que sus resultados solo sirven para decidir hacia dónde apuntar el siguiente experimento (no para validar la solución en sí).

---

## Pre-mortem

**Prompt usado:** el sugerido en la guía, pidiendo a la IA que actúe como crítico de producto digital e imagine el fracaso de la propuesta seis meses después.

| Causa | Supuesto que falló | Señal temprana | Experimento pequeño |
|---|---|---|---|
| Problema inexistente o mal definido | Que el freno principal es el dinero y no la réplica (o viceversa) | La encuesta del experimento mínimo queda empatada o contradice lo esperado | El experimento mínimo diseñado en la Caja 8 |
| Limitaciones tecnológicas/legales | Que se puede simular la retención de fondos sin ser una plataforma registrada | Mercado Pago u otro medio de pago rechaza o limita el flujo de retención manual | Prueba técnica simple con un pago de prueba entre dos cuentas del equipo |
| Baja adopción | Que un paso extra de "seña protegida" genera confianza y no fricción | Los compradores prefieren seguir transfiriendo directo "porque es más rápido" | Fake door: dos versiones de landing (con y sin SeñaSegura) midiendo clics en "continuar" |

**Riesgos seleccionados por el equipo (los tres más importantes):**
1. Que el problema esté mal definido (la Caja 7 ya lo pone como prioridad 1).
2. Que la retención de fondos no sea viable de simular de forma simple y confiable.
3. Que el paso adicional genere más fricción que confianza y los usuarios prefieran la transferencia directa de siempre.

**Verificación:** los tres riesgos confirman que la hipótesis priorizada en la Caja 7 (Problema) sigue siendo correcta: no tiene sentido resolver la factibilidad o la adopción de SeñaSegura si todavía no sabemos si el miedo financiero es realmente el freno principal.

---

## Cierre del equipo

```text
La solución digital que decidimos explorar es:
SeñaSegura, un flujo de pago de seña con liberación condicionada a la
confirmación de entrega del comprador.

La evidencia más fuerte que la respalda es:
El comportamiento observado en Clase 2 (exigencia constante de pruebas
antes de pagar) combinado con la contradicción detectada en el role-play:
el miedo a la estafa financiera podría pesar más que el miedo a la réplica.

El supuesto más riesgoso es:
Que los compradores confiarán en un flujo de pago intermediado por
nuestro propio equipo, sin infraestructura legal de retención de fondos,
tanto o más de lo que confiarían en pedir pruebas de autenticidad.

Lo más importante que necesitamos aprender es:
Si el freno real para pagar la seña es el miedo a la réplica o el miedo
a transferir dinero sin garantías a un desconocido.

El experimento que realizaremos es:
Una encuesta dirigida y entrevistas cortas de seguimiento a 15-20
estudiantes que compraron o intentaron comprar ropa importada, para
identificar cuál de los dos miedos predomina en el "momento de quiebre".

Abandonaremos o cambiaremos la propuesta si:
El miedo a la réplica resulta ser predominante (60% o más), lo que
indicaría que el foco debe estar en verificación de autenticidad
(Alternativa 1 o 3) y no en un mecanismo de pago seguro.
```

---

## Lista de verificación (Paso 13)

- [x] El problema de negocio utiliza evidencia de la Clase 2.
- [x] Los supuestos están diferenciados de los hechos.
- [ ] Los resultados de negocio son observables — **pendiente de línea de base real**, hoy son "pendiente de medir".
- [x] Los usuarios, clientes y decisores están diferenciados o marcados como pendientes.
- [x] Los resultados del usuario describen progreso, no herramientas.
- [x] Se generaron entre dos y tres soluciones digitales diferentes.
- [x] La solución seleccionada tiene tecnología en el centro.
- [x] Los datos y dependencias necesarios están identificados.
- [x] Existen hipótesis de problema, valor, comportamiento y factibilidad.
- [x] Una hipótesis fue priorizada por incertidumbre e impacto.
- [x] El pre-mortem cuestionó la propuesta.
- [x] El experimento prueba una hipótesis principal (Problema).
- [x] La métrica y el criterio de éxito fueron definidos antes de ejecutar.
- [x] Las limitaciones del experimento están documentadas.
- [ ] **Pendiente real del equipo:** confirmar que las entrevistas reales de Clase 2 efectivamente se realizaron; si no, todo este canvas debe tratarse como hipótesis de práctica, no como decisiones finales.

