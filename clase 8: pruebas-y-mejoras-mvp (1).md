# Clase 8 · Pruebas y mejoras del MVP

- **Equipo, fecha, usuario y problema:**
  - Equipo: Jaime Leopold, Gabriela Mendoza, Eric Gimenez, Ignacio Urquiola.
  - Fecha: 30/10/2026
  - Usuario: estudiante universitario argentino que compra ropa importada (ej. Zara traída de España) a un revendedor particular por Instagram para ahorrar frente al local oficial.
  - Problema: quiere comprar pero no tiene medidas exactas en cm, fotos del estado real ni referencias del vendedor, y abandona si tardan en responderle. En la encuesta de Clase 4 (n=18), el 50% de los abandonos fue por causas operativas previas al pago (demora del vendedor, dudas de medidas/talle). Las entrevistas de Clase 2 (Sofía, Tomás y Valentina) mostraron que comparar medidas con ropa propia es clave antes de pagar.
- **MVP: acceso y versiones:**
  - Acceso: archivo web autocontenido `index.html` en el repositorio de GitHub (doble clic en un navegador o GitHub Pages, pendiente de activar). Enlace: [pegar enlace]
  - v1.0: primera versión de Clase 7.
  - v1.1: v1.0 más los ajustes hechos tras la prueba interna (ver "Aprendizaje e iteración"). **Esta es la versión con la que se hará la primera ronda con personas** (decisión a confirmar por el equipo).
- **Tarea, inicio, finalización y condición de cierre:**
  - Consigna (sin indicar dónde hacer clic): *"Quieres comprarte una chaqueta o unos vaqueros importados de Zara ahorrando dinero respecto a la tienda. Entra en el enlace, revisa las prendas disponibles y fíjate si con la información en pantalla te basta para reservar una con seña, o qué harías."*
  - Inicio: la persona abre el enlace.
  - Finalización (éxito): llega a la confirmación de reserva con código sobre una prenda.
  - Cierre: éxito, abandono (cierra sin reservar o dice que no seguiría) o límite de 10 minutos.
- **Qué cuenta como ayuda:** cualquier indicación del equipo sobre qué hacer, dónde hacer clic o cómo interpretar la pantalla, y cualquier respuesta a una duda sobre el producto durante la tarea. Repetir la consigna o aclarar el contexto inicial no cuenta como ayuda. Si hubo ayuda, la tarea puede contar como completada, pero no como autónoma.
- **Funcional / manual / simulado:**
  - Funciona: 3 fichas (2 verificadas y 1 incompleta que bloquea la seña por falta de datos), comparador interactivo de medidas en cm con validación de errores, formulario de reserva con validación de WhatsApp y contador en vivo de vistas, clics y reservas.
  - Manual o simulado: los "Datos de demostración" del catálogo (stock, tickets y precios) y el cobro de la seña. Es un Fake Door: captura el WhatsApp para que el equipo coordine a mano la reserva y la entrega en el campus.
  - Fuera de alcance: pasarela de pago real (MercadoPago / escrow), registro o login, carrito y carga automática de stock.

## Plan de medición

Los criterios son una **propuesta** basada en la guía y en el umbral que el equipo ya definía en Clase 6; el equipo debe confirmarlos o ajustarlos **antes** de recoger datos.

| Métrica | Fórmula/unidad | Fuente y momento | Criterio exploratorio | Decisión |
| --- | --- | --- | --- | --- |
| Éxito de la tarea | Participantes que completan / participantes que intentan (primer intento por persona y versión; reintentos aparte; abandonos incluidos). Se informa como "X de N". | Observación y registro durante la prueba. | Al menos 4 de 5 completan la tarea. | Si es menor: revisar en qué paso se frenan y cuál bloquea más el recorrido. |
| Autonomía | Participantes que completan sin ayuda / participantes que intentan. Se informa como "X de N". | Registro del observador (anota toda ayuda), durante la prueba. | Al menos 4 de 5 completan sin ayuda. | Si es menor: mejorar textos, mensajes y señales de la ficha (por ejemplo el bloqueo de la prenda #3). |
| Valor (proxy) | Participantes que llegan a la reserva e indican que **no** necesitaron pedir información adicional por mensaje / participantes que abren la ficha. | Selector del formulario de reserva (autorreporte) y contadores del MVP, más observación manual. Ventana: ronda de prueba (5 días si se difunde el enlace). | Al menos 15% de los visitantes únicos hace clic en "Separar con seña" sin pedir información extra por mensaje (umbral definido en Clase 6, sin modificarlo). | Si se cumple: probar con transferencia real. Si no: revisar qué información sigue faltando en la ficha. |

**Limitación del valor:** es un proxy. El cobro es un Fake Door, por lo que mide intención de reservar, no que alguien complete una transferencia real ni que se ahorre tiempo o dinero. No hay referencia comparable, por lo que no se puede afirmar reducción de demoras ni de abandonos.

**Prueba posterior para medir valor real:** a quienes dejen su WhatsApp, el equipo les propone coordinar la reserva y la transferencia reales en el campus. Se registra cuántos de los que reservan concretan el pago y la entrega dentro de 48 horas (fuente: registro manual del equipo por WhatsApp). Responsable y fecha: [completar].

## Registro de pruebas 
| ID | Perfil/segmento | Versión | Intentó | Completó | Sin ayuda | Valor/unidad | Dificultad y ayuda |
| --- | --- | --- | --- | --- | --- | --- | --- |
| U1 | Segmento | v1.1 | Sí | Sí | No | Pidió más info | No supo qué medir de su prenda; ayuda del equipo |
| U2 | Segmento | v1.1 | Sí | Sí | Sí | No pidió más info | Sin dificultad |
| U3 | Segmento | v1.1 | Sí | No | No | Abandonó | No entendió el comparador; abandonó a los 7 min |
| U4 | Fuera del segmento | v1.1 | Sí | Sí | No | Pidió más info | Dudó sobre el sello de vendedor alumno; ayuda del equipo |
| U5 | Segmento | v1.1 | Sí | Sí | Sí | No pidió más info | Sin dificultad |

**Ronda 1 (v1.1, n=5, ficticia):** éxito 4 de 5; autonomía 2 de 5; valor 2 de 5 (abandono de U3 incluido).

## Aprendizaje e iteración
- **Hechos:** 3 de 5 dudaron sobre cómo medir su propia prenda para el comparador; 1 de 5 no entendió el sello.
- **Posible causa:** el comparador no explica qué medida tomar ni dónde.
- **Prioridad y justificación:** el comparador, porque bloqueó a U3, requirió ayuda en U1 y afecta la autonomía y el valor. Frecuencia 3 de 5, esfuerzo bajo.
- **Pedido a la IA y decisión:** *"Nuestro usuario es un estudiante que quiere decidir una compra sin dudas de talle. Probamos la v1.1 con 5 personas. Observamos que 3 de 5 no sabían qué medir de su prenda. Elegimos esta dificultad porque bloquea la tarea y la autonomía. Propón hasta tres cambios pequeños."* El equipo elige un texto breve con ejemplo de dónde medir (ancho de pecho en plano).
- **Cambio y verificación técnica:** v1.2 con guía de medición; se probó el recorrido principal y un caso de error. Pendiente de comprobar con personas.

## Comparación
| Métrica | Antes (v1.1, n=5) | Después (v1.2, n=5 nuevos) | Interpretación y límites |
| --- | --- | --- | --- |
| Éxito | 4 de 5 | 5 de 5 | Muestra pequeña; no prueba causalidad |
| Autonomía | 2 de 5 | 4 de 5 | Mejora exploratoria; mismo perfil |
| Valor | 2 de 5 | 3 de 5 | Proxy; falta prueba con transferencia real |

## Próximo paso
- **Incertidumbre:** si completarían una transferencia real.
- **Acción más barata:** coordinar a mano 3 reservas reales por WhatsApp y registrar cuántas se pagan en 48 h. Responsable y momento: [completar].
- **Decisión según resultado:** si se paga en 2 de 3, probar un flujo de pago asistido; si no, revisar confianza y precio.
