# Economía del producto — SeñaSegura

- **Fecha, moneda y período:** 19/10/2026 · pesos argentinos (ARS) · por operación (prenda reservada, pagada y entregada en el campus).
- **Usuario, valor y evidencia disponible:** estudiante universitario que compra ropa importada a revendedores por Instagram. Valor: decidir la compra sin dudas de calce ni de confiabilidad del vendedor (Ficha de Prenda Verificada + reserva con seña). Evidencia: encuesta Clase 4 (n=18, 50 % de abandonos por demora o dudas de talle), entrevistas Clase 2 y ronda ficticia de Clase 8 (v1.2: éxito 5 de 5, autonomía 4 de 5, valor proxy 3 de 5). **No hay evidencia de pago:** el cobro de la seña es un Fake Door.
- **Quién pagaría/financiaría y por qué (hipótesis):** el **revendedor alumno**, con una comisión por venta concretada, porque la ficha le ahorra mensajes repetidos y reduce abandonos antes del pago. El comprador usa y recibe valor, pero no paga en esta hipótesis (ya busca ahorrar respecto del shopping). Que alguien haya reservado en el MVP no demuestra que el vendedor pagaría.
- **Unidad económica:** una operación concretada (seña cobrada + prenda entregada). El ingreso propio es la comisión, **no** el precio de la prenda.

## Números iniciales
| Concepto | Importe y unidad | Observado / referencia / estimación / pendiente | Fuente o motivo |
| --- | --- | --- | --- |
| Precio de la prenda (base de la comisión) | $60.000 por operación | Estimación | Supuesto del equipo para una campera/jean importado; los precios del MVP son datos de demostración. Rango a verificar con revendedores. |
| Ingreso por unidad | $3.000 por operación (5 % de $60.000) | Estimación | Porcentaje elegido por el equipo; sin evidencia de disposición a pagar. |
| Trabajo manual: verificar ficha (medidas, fotos, ticket) | 10 min por operación | Estimación | Medir en plano y cargar datos de una prenda. |
| Trabajo manual: coordinar por WhatsApp y entregar en campus | 15 min por operación | Estimación | Coordinación de reserva, transferencia y encuentro. |
| Valor horario del equipo | $5.000 / hora | Estimación | Hoy trabajamos gratis; se usa para valuar el esfuerzo de sostener la operación, no es un desembolso actual. |
| Comisión de medio de pago | Pendiente | Pendiente | Hoy la seña sería por transferencia; si se usa una pasarela, falta consultar su tarifa vigente. |
| Costos fijos por período | $0 de desembolso mensual | Observado (plan actual) | GitHub Pages gratuito para el prototipo; no garantiza operación gratuita a mayor escala. |
| Inversión inicial | Horas del equipo para construir el MVP (Clases 7–8) | Pendiente de cuantificar | No hubo desembolso de dinero; no se suma a la contribución. |

## Resultado y escenario
- **Contribución por unidad:** ingreso − costo variable = $3.000 − (25 min × $5.000/h ≈ $2.083) = **≈ $917 por operación**.
- **Escenarios (cambia solo el tiempo manual por operación):**

| Concepto | Base estimada (25 min) | Escenario exigente (45 min) |
| --- | --- | --- |
| Ingreso | $3.000 | $3.000 |
| Costo variable (trabajo manual) | ≈ $2.083 | $3.750 |
| Contribución | ≈ $917 | ≈ −$750 |

- **Qué significa y qué no demuestra:** con atención 100 % manual, el margen por operación es chico y se vuelve negativo si cada venta lleva más de ~36 minutos (punto de equilibrio: $3.000 ÷ $5.000/h). Antes de escalar habría que reducir tiempo (por ejemplo, que el vendedor cargue sus propias medidas con la guía de la v1.2). Estos números no demuestran que haya vendedores dispuestos a pagar 5 %, ni cubren costos fijos futuros.

## Primeros clientes
- **Canal, costo y esfuerzo previstos:** contacto directo con revendedores que ya venden en grupos de Instagram/WhatsApp de la facultad, y difusión del enlace del MVP a estudiantes en esos mismos grupos. Sin gasto publicitario, pero con esfuerzo comercial: estimamos unas 2 horas del equipo para contactar a 5 revendedores (estimación).
- **CAC / repago:** **pendiente.** Con cero vendedores pagadores no se puede calcular. A averiguar: horas reales invertidas por vendedor que acepta y paga.

## Supuesto por comprobar
- **Supuesto elegido:** los revendedores alumnos aceptan pagar una comisión del 5 % por venta concretada a través de SeñaSegura.
- **Prueba, con quién, acción observable y registro:** ofrecer a 5 revendedores del campus publicar 1 prenda con Ficha Verificada pagando la comisión solo si se vende. Acción observable: (1) aceptan y envían los datos de la prenda; (2) tras la venta, transfieren la comisión. Se combina con la prueba ya planificada en Clase 8 (3 reservas reales por WhatsApp), donde además se registran los minutos reales por operación. Registro: planilla manual del equipo (vendedor, aceptó sí/no, prenda, precio, vendió sí/no, pagó comisión sí/no, minutos invertidos).
- **Qué no demostraría:** que el 5 % sea el precio óptimo ni que se sostenga con más volumen; un "sí, me interesa" sin transferencia no cuenta como pago.
- **Criterio previo y decisión:** si al menos 3 de 5 aceptan **y** al menos 1 paga efectivamente la comisión, mantenemos al vendedor como pagador y medimos tiempo con más operaciones. Si aceptan pero nadie paga, probamos un cargo fijo por publicación o un fee al comprador. Si menos de 3 aceptan, revisamos quién paga antes de seguir construyendo.
- **Responsable y fecha:**  Eric, Gabriela, Jaime e Ignacio a 23/10/2026.
