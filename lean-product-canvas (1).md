# Lean Product Canvas — SeñaSegura

> Este canvas contiene hipótesis. La evidencia surgirá de observar y experimentar.

## 1. Problema de negocio

Cuando un comprador y un revendedor informal de indumentaria importada negocian por Instagram, la falta de garantías sobre el pago adelantado (seña) genera desconfianza mutua: el comprador teme pagar y no recibir el producto esperado, y el vendedor teme enviar la prenda sin haber cobrado. Esto provoca abandono de la compra, ciclos de negociación desgastantes o ventas que no se concretan.

**Evidencia:** entrevistas reales (Sofía, Tomás, Valentina) muestran que el mayor esfuerzo del comprador ocurre *antes* de pagar, buscando y contrastando información para reducir incertidumbre; fuentes oficiales (UFECI, BA-CSIRT, La Nación) documentan el crecimiento de estafas en compraventa por Instagram en Argentina.

**Supuesto:** que el vendedor experimenta el mismo nivel de desconfianza que el comprador (no entrevistamos a ningún vendedor todavía).

## 2. Resultados de negocio

- Reducir el % de negociaciones de compra-venta que se abandonan por falta de confianza, desde *pendiente de medir* hasta *pendiente de definir* en 3 meses de operación.
- Aumentar el % de transacciones que se concretan con seña pagada por adelantado, desde *pendiente de medir* hasta *pendiente de definir*.
- Reducir el tiempo promedio entre primer contacto y pago, desde *pendiente de medir* hasta *pendiente de definir*.

## 3. Usuarios y clientes

| Rol | Descripción | Fuente |
|---|---|---|
| Usuario comprador | Estudiante universitario argentino que compra indumentaria importada por Instagram/DM | Evidencia (3 entrevistas) |
| Usuario vendedor | Revendedor informal (frecuentemente también estudiante) que trae ropa de España | Supuesto — sin entrevistas propias todavía |
| Cliente | Pendiente de investigación: podría ser comprador, vendedor o ambos, según modelo de comisión | Supuesto |
| Decisor | Ambas partes deben aceptar usar la herramienta para que la transacción ocurra | Supuesto |
| Influenciador | Comunidades tipo "Legit Check Arg" que validan autenticidad | Evidencia (Clase 2) |

## 4. Necesidades y resultados del usuario

- **Comprador:** Cuando quiero comprar una prenda importada a un revendedor desconocido por Instagram, quiero tener garantías de que si pago la seña voy a recibir el producto tal como se describió, para decidir sin miedo a perder mi dinero.
- **Vendedor (supuesto):** Cuando negocio la venta de una prenda con un comprador desconocido, quiero tener garantías de que voy a cobrar si entrego el producto, para no arriesgarme a enviarlo sin cobrar.

## 5. Ideas de solución

### Alternativa 1 — Información/decisión: Sello de confianza digital
Checklist guiado (bot de WhatsApp/Instagram) que estructura la evidencia que hoy se pide de forma desordenada (ticket, medidas, video). Tecnología central: chatbot + almacenamiento de evidencia. Riesgo: no resuelve el riesgo financiero de la seña, solo la duda sobre el producto.

### Alternativa 2 — Coordinación/transacción: SeñaSegura (seleccionada)
Plataforma que retiene la seña (escrow) hasta que el comprador confirma la recepción conforme, integrada a una pasarela de pago existente (ej. Mercado Pago). Tecnología central: integración de pagos + lógica de retención/liberación. Datos necesarios: monto, comprobante de entrega, confirmación del comprador. Riesgo principal: exposición regulatoria por retener fondos de terceros. Prototipo inicial: flujo simulado en notebook o app no-code (Bubble/Glide) con pagos ficticios.

### Alternativa 3 — Automatización/inteligencia: Verificador de autenticidad con IA
Asistente que analiza fotos de prenda/ticket para detectar inconsistencias antes del pago. Riesgo: precisión limitada sin dataset de fraudes reales; alto costo de entrenamiento.

- **Estado:** idea no validada.
- **Dependencia secundaria:** integración con procesador de pagos externo (no es infraestructura física, es una dependencia técnica de terceros).

## 6. Hipótesis principales

### Hipótesis de problema
Creemos que compradores y vendedores de este circuito abandonan o retrasan ventas por falta de garantías mutuas sobre el pago adelantado.
Lo sabremos si al menos el 50% de los encuestados/entrevistados confirma haber abandonado o postergado una compra/venta por este motivo.

### Hipótesis de valor
Creemos que un mecanismo que retiene la seña hasta confirmar la entrega (SeñaSegura) aumentará la disposición de ambas partes a concretar la transacción.
Lo sabremos si al menos el 40% de los encuestados declara que usaría el servicio si estuviera disponible.

### Hipótesis de comportamiento
Creemos que compradores y vendedores estarán dispuestos a dejar de usar transferencia directa y adoptar un intermediario externo para gestionar el pago.
Lo sabremos si al menos el 20% de los visitantes de una landing/fake door deja su contacto para sumarse a una lista de espera.

### Hipótesis de factibilidad
Creemos que podemos simular un flujo de retención y liberación de fondos usando una pasarela de pago existente, sin necesitar licencia financiera propia para el prototipo.
Lo sabremos si logramos armar una simulación funcional (pago → retención → confirmación → liberación) con datos de ejemplo.

## 7. Lo más importante por aprender

| Hipótesis | Incertidumbre 1–5 | Impacto 1–5 | Prioridad | Justificación |
|---|---:|---:|---:|---|
| Problema | 2 | 5 | Media | Ya hay evidencia fuerte de Clase 2 |
| Valor | 4 | 5 | **Alta** | No sabemos si pagarían/usarían un tercero |
| Comportamiento | 5 | 5 | **Alta** | Cambiar el hábito de transferencia directa es incierto |
| Factibilidad | 3 | 4 | Media | Existen pasarelas de pago, pero la retención regulatoria es incierta |

**Pregunta priorizada:**
¿Los compradores y vendedores de indumentaria importada estarían dispuestos a usar un tercero de confianza que retenga la seña, en lugar de transferir el dinero directamente?

## 8. Experimento mínimo

- **Hipótesis que prueba:** Comportamiento (disposición a usar un intermediario de confianza para la seña).
- **Objetivo:** Medir intención real de uso, no solo opinión declarada.
- **Tipo de experimento:** Landing page tipo *fake door* + encuesta corta.
- **Herramienta:** Google Forms + landing simple (Carrd o Notion).
- **Participantes:** mínimo 15 compradores y 5 revendedores del entorno universitario.
- **Duración:** 5 días.
- **Tarea:** completar la encuesta y, si les interesa, dejar contacto para "anotarse a la lista de espera" de SeñaSegura.
- **Datos necesarios:** respuestas de encuesta y tasa de registro en la lista de espera (sin datos sensibles).
- **Métrica:** % de visitantes que dejan su contacto en la lista de espera.
- **Criterio de éxito:** 20% o más de conversión a lista de espera.
- **Criterio de fracaso:** menos del 10% de conversión.
- **Aprendizaje esperado:** si existe intención de uso real (comportamiento) más allá de la simpatía declarada por la idea.
- **Limitaciones:** intención declarada ≠ pago real; muestra pequeña y sesgada al entorno universitario propio del equipo.

---

## Pre-mortem — SeñaSegura

*Imaginamos que, seis meses después de lanzarse, la propuesta fracasó.*

| Causa | Supuesto que falló | Señal temprana observable | Experimento pequeño para investigarlo |
|---|---|---|---|
| **Problema inexistente o poco relevante** | Que la desconfianza mutua (no solo del comprador) es realmente lo que frena las ventas | En entrevistas de seguimiento, los vendedores dicen que ellos nunca dudaron del comprador | Entrevistar a 3–5 revendedores reales (hoy solo hay evidencia del lado comprador) |
| **Falta de valor para el usuario** | Que retener la seña resuelve más desconfianza de la que genera fricción nueva (trámite extra, demora en cobrar) | Usuarios abandonan el flujo al ver que el vendedor no cobra hasta la confirmación | Prototipo navegable del flujo de pago con tarea cronometrada, medir abandono paso a paso |
| **Baja adopción o uso** | Que comprador y vendedor migrarán de la transferencia directa a un intermediario nuevo | Menos del 10% de conversión en la landing/fake door | El experimento mínimo ya diseñado (Caja 8) |
| **Datos insuficientes o de mala calidad** | Que se puede verificar "entrega conforme" de forma confiable a distancia | No hay forma consistente de que el comprador certifique digitalmente que la prenda llegó como se esperaba (fotos, video, etc. son manipulables) | Simulación tipo Wizard of Oz: un humano del equipo revisa manualmente "evidencias de entrega" de 10 casos ficticios y mide cuántos son ambiguos |
| **Limitaciones tecnológicas** | Que se puede integrar fácilmente con una pasarela de pago existente para retener/liberar fondos | Al investigar APIs de Mercado Pago u otras, no existe función nativa de "retención condicional" accesible sin cuenta empresarial/habilitación especial | Prueba técnica: intentar armar el flujo de retención en modo sandbox de una pasarela real |
| **Privacidad, seguridad o confianza** | Que los usuarios confiarán sus datos de pago a una plataforma nueva y desconocida (paradoja: para resolver desconfianza, pedimos más confianza) | En la encuesta, alta tasa de "no dejaría mis datos de pago a una app que no conozco" | Pregunta específica sobre esto en la encuesta de Clase 4, separada de la intención general de uso |
| **Dependencias institucionales / regulatorias** ⚠️ | Que se puede operar un esquema de retención de fondos de terceros (escrow) sin habilitación regulatoria como entidad de pago | Al consultar el marco normativo del BCRA/CNV sobre custodia de fondos de terceros, se descubre que requiere registro como Proveedor de Servicios de Pago (PSP) o similar, inviable para un proyecto estudiantil en el corto plazo | Investigación legal exploratoria (no simulación): consultar normativa vigente o a un profesor/abogado antes de seguir invirtiendo en esta alternativa |
| **Modelo de negocio** | Que existe disposición a pagar una comisión por el servicio (de comprador, vendedor, o ambos) | En la encuesta, nadie indica estar dispuesto a pagar una comisión adicional por seguridad | Pregunta directa de disposición a pagar en la encuesta de Clase 4 |

### Decisión del equipo (3 riesgos priorizados)

1. **Dependencias institucionales / regulatorias** — este es el riesgo que podría invalidar toda la Alternativa 2 (SeñaSegura) sin importar el resto, porque si retener fondos de terceros requiere una habilitación que el equipo no puede obtener en el marco de la materia, hay que pivotar la solución antes de seguir validando valor o comportamiento.
2. **Baja adopción o uso** — migrar el hábito de "transferencia directa" a un intermediario nuevo es una barrera de comportamiento fuerte, ya reflejada en la Caja 7 como la hipótesis de mayor incertidumbre e impacto.
3. **Datos insuficientes de calidad** — sin una forma confiable de verificar "entrega conforme", el mecanismo de liberación de fondos pierde sentido.

**Verificación de la hipótesis priorizada (Caja 7):** el pre-mortem confirma que la pregunta de comportamiento sigue siendo la más urgente, pero agrega que la pregunta regulatoria (factibilidad) debe investigarse en paralelo y no después, porque si el escrow es inviable legalmente, cambia directamente la Caja 5 (solución) antes de seguir invirtiendo en validar valor o comportamiento sobre una alternativa que quizás no se pueda operar.

---

## Cierre del equipo

La solución digital que decidimos explorar es: **SeñaSegura**, una plataforma de retención de seña (escrow) para transacciones entre comprador y vendedor informal de indumentaria importada.

La evidencia más fuerte que la respalda es: las entrevistas reales de Clase 2 (Sofía, Tomás, Valentina) y las fuentes oficiales sobre estafas en compraventa por Instagram (UFECI, BA-CSIRT, La Nación).

El supuesto más riesgoso es: que se puede operar legalmente un esquema de retención de fondos de terceros sin habilitación regulatoria como entidad de pago.

Lo más importante que necesitamos aprender es: si compradores y vendedores estarían dispuestos a usar un tercero de confianza para gestionar la seña, en lugar de transferir el dinero directamente.

El experimento que realizaremos es: una landing page tipo fake door + encuesta corta, midiendo conversión a lista de espera.

Abandonaremos o cambiaremos la propuesta si: la conversión a lista de espera es menor al 10%, o si la investigación regulatoria confirma que el esquema de retención de fondos no es operable dentro del marco de la materia.
