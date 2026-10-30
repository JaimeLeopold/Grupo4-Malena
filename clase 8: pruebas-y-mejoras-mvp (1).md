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

Cada persona se identifica como U1, U2, etc., sin datos personales. Una prueba entre compañeros fuera del segmento sirve para detectar dificultades de uso, no demuestra demanda, disposición a pagar ni valor real.

| ID | Perfil/segmento | Versión | Intentó | Completó | Sin ayuda | Valor/unidad o no medido | Dificultad y ayuda |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Interna (equipo) | Equipo, no cuenta como participante | v1.0 | n/a | n/a | n/a | No medido | Ver "Aprendizaje e iteración". Excluida de las métricas. |
| U1 | Por completar | v1.1 | Por completar | Por completar | Por completar | Por completar | Por completar |
| U2 | Por completar | v1.1 | Por completar | Por completar | Por completar | Por completar | Por completar |
| U3 | Por completar | v1.1 | Por completar | Por completar | Por completar | Por completar | Por completar |
| U4 | Por completar | v1.1 | Por completar | Por completar | Por completar | Por completar | Por completar |
| U5 | Por completar | v1.1 | Por completar | Por completar | Por completar | Por completar | Por completar |

**Resultados de la ronda 1 con personas (v1.1):** no medido, todavía no hubo participantes humanos. El experimento de Clase 5/6 tampoco dejó visitas ni clics registrados.

**Guion para la prueba (3 roles: facilita, observa, registra):**
1. Explicar el contexto y leer la consigna. No indicar pasos.
2. Dejar que la persona intente sin indicaciones. Anotar dudas, errores y abandonos, y cualquier ayuda dada.
3. Al terminar preguntar: ¿qué esperabas encontrar? ¿qué te confundió? ¿qué te faltó para decidir?
4. Registrar si pertenece al segmento y si usó el comparador con su propia prenda.

## Aprendizaje e iteración

- **Hechos observados** (prueba interna del equipo en clase, v1.0; no son participantes humanos):
  1. En la prenda #3 (sin medidas) no quedaba claro por qué no se podía avanzar.
  2. En el formulario de seña de las prendas #1 y #2 faltaba capturar si la persona se quedaba con dudas que requerirían mandar un mensaje (la métrica de valor de Clase 6).
  3. El formulario no aclaraba que la reserva es manual y sin cobro automático.
- **Posibles causas (a comprobar):** la ficha incompleta no explica qué dato falta; el formulario no estaba pensado para medir el valor ni para fijar expectativas sobre el cobro.
- **Prioridad elegida y justificación:** el bloqueo sin explicación de la prenda #3 y la falta de medición de valor, porque impiden completar la tarea y medir si la ficha evita el ida y vuelta de mensajes. Quedó fuera de esta iteración cualquier función sin relación con lo observado (pasarela de pago, login, carrito).
- **Pedido a la IA y decisión del equipo** (devolución dada a la IA): *"Elegí la prenda #3 (sin medidas) y busqué el botón de señar. Esperaba ver el motivo del bloqueo, pero no explicaba qué dato faltaba. Además, al presionar 'Separar con seña' en la prenda #1, necesitamos que el formulario aclare que es una reserva manual sin cobro automático e incluya una pregunta para registrar si el usuario necesita o no pedir más datos por mensaje."*
- **Cambio realizado y verificación técnica:** se agregó la alerta roja de bloqueo por falta de datos en la prenda #3, la validación numérica en el comparador de medidas y el campo selector en el formulario de reserva. Se volvió a probar el recorrido en los 3 casos y funcionó sin errores. **Verificación técnica y del equipo únicamente: sigue pendiente comprobar con personas que estos cambios mejoran el uso.**
- **Nota:** esta iteración se hizo a partir de una prueba interna. La dificultad priorizada de la ronda con personas se elegirá con los registros reales de U1–U5 y, si no aparece una dificultad relevante, se justificará mantener la versión y pasar a una prueba más exigente o en contexto real.

## Comparación

| Métrica | Antes (n y resultado) | Después (n y resultado) | Interpretación y límites |
| --- | --- | --- | --- |
| Éxito | No medido (sin participantes humanos en v1.0) | Pendiente: ronda 1 con v1.1 | Sin datos no hay comparación. La segunda ronda debería hacerse con personas nuevas del mismo perfil y la misma consigna. |
| Autonomía | No medido | Pendiente | Si se repiten participantes, aclarar que ya conocen el recorrido. |
| Valor (proxy) | No medido | Pendiente | Fake Door: mide intención, no pago real. Comparación exploratoria, no prueba causalidad. |

Al comparar, registrar cambios de contexto, perfil, dispositivo o instrucciones, y reportar por separado los abandonos.

## Próximo paso

- **Incertidumbre pendiente:** si la Ficha de Prenda Verificada logra que al menos el 15% de los visitantes únicos haga clic en "Separar con seña" sin pedir información extra por mensaje, y si esas personas completarían luego una transferencia real.
- **Acción más barata, responsable y momento:** activar GitHub Pages y pegar el enlace arriba; probad con 3 a 5 estudiantes del segmento con el guion de arriba y difundid el enlace 5 días a entre 30 y 50 estudiantes, sin cambiar la hipótesis ni el umbral. Volcad las visitas, los clics y las reservas reales en `registro-experimento.md`. Responsable: [completar]. Momento: [completar].
- **Qué observar y qué decisión tomar según el resultado:**
  - Si se alcanza el 15% y la mayoría completa sin ayuda: probar la reserva con transferencia real coordinada a mano.
  - Si no se alcanza: identificar la dificultad más frecuente en los registros, elegir un cambio pequeño, pedirlo a la IA, implementarlo y repetir con personas nuevas.
  - Si faltan datos: seguir probando antes de decidir.
