> ⚠️ **EJEMPLO FICTICIO PARA PRACTICAR.** Todos los participantes, tiempos y resultados de este documento son inventados y **no proceden de pruebas reales**. No presentarlo como evidencia. El documento con datos reales es `pruebas-y-mejoras-mvp.md`.

# Clase 8 · Pruebas y mejoras del MVP (ejemplo con datos ficticios)

- **Equipo, fecha, usuario y problema:** [nombres del equipo] · 30/10/2026 · estudiante universitario argentino que compra ropa importada a un revendedor por Instagram. No tiene medidas exactas en cm, fotos del estado real ni referencias del vendedor, y abandona si tardan en responder. Base real: encuesta de Clase 4 (n=18), 50% de abandonos por causas operativas previas al pago.
- **MVP: acceso y versiones:** `index.html` en GitHub Pages [enlace]. v1.0 (Clase 7), v1.1 (con alerta de bloqueo, validación del comparador y selector de valor), v1.2 (ficticia: con guía de medición en el comparador).
- **Tarea, inicio, finalización y cierre:** *"Quieres comprarte una chaqueta o unos vaqueros importados de Zara ahorrando dinero respecto a la tienda. Entra en el enlace, revisa las prendas y fíjate si con la información en pantalla te basta para reservar una con seña, o qué harías."* Inicio: abre el enlace. Éxito: llega a la confirmación con código de reserva. Cierre: éxito, abandono o límite de 10 minutos.
- **Qué cuenta como ayuda:** cualquier indicación del equipo sobre qué hacer o cómo interpretar la pantalla, y toda respuesta a dudas sobre el producto durante la tarea.
- **Funcional / manual / simulado:** funcionan las 3 fichas, el comparador, el formulario con validación y los contadores. Son manuales o simulados los datos de demostración y el cobro de la seña (Fake Door, coordinación manual por WhatsApp). Fuera de alcance: pasarela de pago, login, carrito.

## Plan de medición
| Métrica | Fórmula/unidad | Fuente y momento | Criterio exploratorio | Decisión |
| --- | --- | --- | --- | --- |
| Éxito | Completan / intentan | Observación durante la prueba | ≥ 4 de 5 | Qué bloquea el recorrido |
| Autonomía | Completan sin ayuda / intentan | Registro de ayuda del observador | ≥ 4 de 5 | Qué textos o interacciones mejorar |
| Valor (proxy) | Llegan a la reserva sin pedir información adicional por mensaje / intentan | Selector del formulario | ≥ 15% de visitantes en la difusión; en la prueba presencial se informa "X de 5" | Si pasar a transferencia real |

Limitación: el valor es un proxy (Fake Door), mide intención de reservar, no pago real.

## Registro de pruebas — DATOS FICTICIOS
| ID | Perfil/segmento | Versión | Intentó | Completó | Sin ayuda | Valor/unidad | Dificultad y ayuda |
| --- | --- | --- | --- | --- | --- | --- | --- |
| U1 | Segmento | v1.1 | Sí | Sí | No | Pidió más info | No supo qué medir de su prenda; ayuda del equipo |
| U2 | Segmento | v1.1 | Sí | Sí | Sí | No pidió más info | Sin dificultad |
| U3 | Segmento | v1.1 | Sí | No | No | Abandonó | No entendió el comparador; abandonó a los 7 min |
| U4 | Fuera del segmento | v1.1 | Sí | Sí | No | Pidió más info | Dudó sobre el sello de vendedor alumno; ayuda del equipo |
| U5 | Segmento | v1.1 | Sí | Sí | Sí | No pidió más info | Sin dificultad |

**Ronda 1 (v1.1, n=5, ficticia):** éxito 4 de 5; autonomía 2 de 5; valor 2 de 5 (abandono de U3 incluido).

## Aprendizaje e iteración
- **Hechos (ficticios):** 3 de 5 dudaron sobre cómo medir su propia prenda para el comparador; 1 de 5 no entendió el sello.
- **Posible causa:** el comparador no explica qué medida tomar ni dónde.
- **Prioridad y justificación:** el comparador, porque bloqueó a U3, requirió ayuda en U1 y afecta la autonomía y el valor. Frecuencia 3 de 5, esfuerzo bajo.
- **Pedido a la IA y decisión:** *"Nuestro usuario es un estudiante que quiere decidir una compra sin dudas de talle. Probamos la v1.1 con 5 personas. Observamos que 3 de 5 no sabían qué medir de su prenda. Elegimos esta dificultad porque bloquea la tarea y la autonomía. Propón hasta tres cambios pequeños."* El equipo elige un texto breve con ejemplo de dónde medir (ancho de pecho en plano).
- **Cambio y verificación técnica:** v1.2 con guía de medición; se probó el recorrido principal y un caso de error. Pendiente de comprobar con personas.

## Comparación (ficticia)
| Métrica | Antes (v1.1, n=5) | Después (v1.2, n=5 nuevos) | Interpretación y límites |
| --- | --- | --- | --- |
| Éxito | 4 de 5 | 5 de 5 | Muestra pequeña; no prueba causalidad |
| Autonomía | 2 de 5 | 4 de 5 | Mejora exploratoria; mismo perfil |
| Valor | 2 de 5 | 3 de 5 | Proxy; falta prueba con transferencia real |

## Próximo paso
- **Incertidumbre:** si completarían una transferencia real.
- **Acción más barata:** coordinar a mano 3 reservas reales por WhatsApp y registrar cuántas se pagan en 48 h. Responsable y momento: [completar].
- **Decisión según resultado:** si se paga en 2 de 3, probar un flujo de pago asistido; si no, revisar confianza y precio.
