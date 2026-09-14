# Clase 2 — Descubrimiento de problemas asistido por IA

## Estacionamiento de soluciones

_(Ninguna idea de producto, app o funcionalidad fue estacionada durante el proceso. Si surge una durante las entrevistas reales, anotarla acá y volver a investigar el problema.)_

---

## 1. Territorio de investigación

- **Dominio:** Reventa y comercio internacional de ropa.
  - ¿El dominio es suficientemente concreto para investigar? Sí.
- **Usuario inicial:** Estudiantes argentinos que quieren comprar ropa de marca.
  - ¿Podemos reconocer al usuario que describimos? Sí.
- **Contexto:** Debido a los altos aranceles en Argentina (por ejemplo, para marcas como Zara), sale más económico comprar en España y revender en Argentina.
  - ¿El contexto representa una situación real? Sí.
- **Supuestos iniciales:**
  - La volatilidad del tipo de cambio dificulta calcular el margen de ganancia real al momento de vender.
  - Coordinar los puntos de entrega físicos con los vendedores consume tiempo durante el semestre académico.
  - ¿Marcamos nuestros supuestos como supuestos? Sí.
- **Límites / Fuera de alcance:** Restricciones arancelarias, tipo de cambio. Tampoco se estudian aspectos legales o fiscales relacionados con la reventa.
  - ¿Definimos qué no investigaremos? Sí.

---

## 2. Research secundario

### 2.1 Problemas potenciales (research original del equipo)

| Problema potencial | Usuario | Contexto | Evidencia | Fuente | Hecho, interpretación o supuesto | Preguntas pendientes |
|---|---|---|---|---|---|---|
| **Desconfianza ante posibles réplicas** | Estudiante argentino que busca ropa de marca. | Al contactar a revendedores informales o estudiantes de intercambio por Instagram para comprar. | Compradores exigiendo fotos de etiquetas interiores, tickets de compra de origen (ej. España) y detalles de costuras. | Grupos de Facebook ("Legit Check Arg") y foros de moda. | **Hecho** (el comportamiento de verificación existe y es observable). | ¿Qué elementos específicos generan confianza inmediata en un vendedor particular? |
| **Imposibilidad de pagar en cuotas sin recargos altos** | Estudiante argentino sin gran liquidez en efectivo. | Al intentar comprar una prenda importada a un revendedor independiente que prioriza el efectivo o transferencias. | Quejas frecuentes en comentarios sobre la falta de financiamiento o el recargo abusivo al querer usar tarjeta de crédito. | Comentarios en publicaciones de showrooms en Instagram. | **Interpretación** (asumimos que la falta de cuotas frena muchas ventas de alto valor). | ¿Cuánto recargo están dispuestos a asumir con tal de poder financiar una prenda exclusiva? |
| **Riesgo al no poder probarse la ropa ni devolverla** | Estudiante argentino interesado en indumentaria importada. | Al comprar mercadería traída del exterior a un particular, sabiendo que no hay políticas de cambio o devolución. | Consultas constantes sobre las medidas exactas en centímetros de las prendas (ej. ancho de hombros) por miedo a equivocarse de talle. | Interacciones en Facebook Marketplace y mensajes directos. | **Supuesto** (creemos que el miedo a equivocarse de talle es una fricción principal para no concretar la compra). | ¿Prefieren arriesgarse con el talle para ahorrar dinero o prefieren ir a la tienda oficial aunque sea más caro? |
| **Falta de confianza en el vendedor** | Estudiante argentino. | Compra a una persona particular que encuentra en Instagram u otra plataforma. | Los compradores suelen revisar comentarios, seguidores, publicaciones y experiencias anteriores. | Instagram, Facebook, Reddit | **Hecho:** los compradores buscan referencias antes de comprar. **Supuesto:** la falta de información sobre el vendedor puede generar desconfianza. | ¿Qué señales hacen que un comprador considere fiable a un vendedor? |
| **Dificultad para comprobar el estado de la prenda** | Estudiante argentino. | Compra mediante fotos y mensajes sin poder ver físicamente el producto. | Las publicaciones pueden mostrar un número limitado de fotografías. | Instagram, Facebook, Mercado Libre | **Hecho:** el comprador recibe información principalmente mediante imágenes. **Supuesto:** las fotos pueden no ser suficientes para evaluar el producto. | ¿Qué información o fotografías necesita el comprador antes de comprar? |
| **Dificultad para coordinar la entrega** | Estudiante argentino. | La compra requiere acordar un lugar y horario con el vendedor. | Los compradores y vendedores deben coordinarse mediante mensajes. | Instagram, WhatsApp, Facebook | **Hecho:** la entrega requiere coordinación. **Interpretación:** esto puede generar inconvenientes de tiempo. | ¿Qué tipo de entrega resulta más cómoda para los estudiantes? |

### 2.2 Problemas potenciales (research complementario — fuentes oficiales AR)

| Problema potencial | Usuario | Contexto | Evidencia | Fuente | Hecho, interpretación o supuesto | Preguntas pendientes |
|---|---|---|---|---|---|---|
| **Estafas por productos que nunca llegan tras el pago** | Compradores por Instagram en Argentina | Pago por adelantado a un vendedor desconocido | UFECI reportó un aumento de casos de compradores que pagan y nunca reciben el producto (dic 2024–ene 2025); caso documentado de vendedor que cobró y desapareció | [El Independiente](https://www.elindependiente.com.ar/pagina.php?id=362932), [Diario de Cuyo](https://diariodecuyo.com.ar/policiales/Detuvieron-a-un-bailarin-de-Tini-acusado-de-realizar-estafas-reiteradas-20230104-0004.html) | Hecho general (existencia del fraude); interpretación aplicarlo al nicho de ropa importada | ¿Qué % de estas estafas ocurre en indumentaria vs. otros rubros? |
| **Dificultad para distinguir vendedores falsos de reales** | Compradores en Instagram | Antes de contactar/pagar a un perfil desconocido | Más del 50% de fraudes reportados a BA-CSIRT en 2024 vinculados a Instagram; señales de alerta (seguidores comprados, imágenes robadas, cambios de usuario) | [Buenos Aires Ciudad](https://buenosaires.gob.ar/noticias/vas-comprar-por-instagram-cuidado-con-las-estafas), [Ámbito](https://www.ambito.com/tecnologia/tiendas-falsas-instagram-como-detectar-una-las-estafas-que-crece-argentina-n6172376) | Hecho | ¿Los estudiantes aplican estas verificaciones o confían más por ser conocidos del entorno universitario? |
| **Dificultad para reclamar/recuperar dinero tras estafa** | Compradores estafados | Pago por transferencia bancaria directa | Reclamo debe hacerse directo al banco del vendedor; denuncias de fraude en compraventa pasaron de 603 a 5200/año | [La Nación](https://www.lanacion.com.ar/economia/negocios/compras-por-redes-sociales-las-estafas-crecieron-casi-nueve-veces-en-un-ano-y-ponen-en-alerta-a-los-nid07022022/) | Hecho (dato de 2022, no desagregado por rubro) | ¿Existe dato más reciente y específico? |
| **Mercado de servicios de verificación de autenticidad** | Compradores/revendedores de indumentaria de marca (mercado global) | Antes de comprar reventa sin poder probar la prenda | Foros de expertos voluntarios y servicios pagos (10–30 €) de autenticación; apps con IA que analizan costuras y etiquetas | [Limited Resell](https://limitedresell.com/es/blog/post/como-evitar-productos-falsificados-en-el-mercado-de-reventa-una-guia-de-autenticacion/), [Legit Check App](https://play.google.com/store/apps/details/Legit_Check?id=com.legitcheck&hl=es_US) | Hecho (mercado global); supuesto que aplique igual al circuito España-Argentina | ¿Los estudiantes conocen/usan este tipo de servicios o resuelven todo de forma informal? |
| **Confianza limitada en los propios servicios de autenticación pagos** | Usuarios que ya pagaron por verificación externa | Al usar un servicio de terceros para autenticar | Reseñas reportan veredictos de autenticidad incorrectos pese a errores evidentes en la prenda | [Trustpilot](https://ca.trustpilot.com/review/legitcheck.app) | Interpretación (reseñas individuales, no patrón comprobado) | ¿Los estudiantes argentinos usan o descartan estos servicios? |

### 2.3 Fuentes consultadas

- [Nombre de la fuente](URL): grupos de Facebook ("Legit Check Arg"), foros de moda, comentarios en Instagram, Facebook Marketplace, mensajes directos (sin URL específica registrada por el equipo).
- [UFECI vía El Independiente](https://www.elindependiente.com.ar/pagina.php?id=362932): aumento de estafas por productos que nunca llegan (Instagram, dic 2024–ene 2025).
- [Diario de Cuyo](https://diariodecuyo.com.ar/policiales/Detuvieron-a-un-bailarin-de-Tini-acusado-de-realizar-estafas-reiteradas-20230104-0004.html): caso real de estafa por venta en Instagram con transferencia previa.
- [Buenos Aires Ciudad – BA-CSIRT](https://buenosaires.gob.ar/noticias/vas-comprar-por-instagram-cuidado-con-las-estafas): más del 50% de fraudes reportados vinculados a Instagram.
- [Ámbito Financiero](https://www.ambito.com/tecnologia/tiendas-falsas-instagram-como-detectar-una-las-estafas-que-crece-argentina-n6172376): señales para detectar tiendas falsas en Instagram.
- [La Nación](https://www.lanacion.com.ar/economia/negocios/compras-por-redes-sociales-las-estafas-crecieron-casi-nueve-veces-en-un-ano-y-ponen-en-alerta-a-los-nid07022022/): dificultad de reclamo cuando el pago es por transferencia bancaria.
- [Limited Resell](https://limitedresell.com/es/blog/post/como-evitar-productos-falsificados-en-el-mercado-de-reventa-una-guia-de-autenticacion/): mercado de servicios de autenticación de indumentaria/sneakers.
- [Legit Check – Google Play](https://play.google.com/store/apps/details/Legit_Check?id=com.legitcheck&hl=es_US): app de verificación de autenticidad con IA.
- [Trustpilot – Legit Check By Ch](https://ca.trustpilot.com/review/legitcheck.app): reseñas sobre fallos en servicios de autenticación pagos.

### 2.4 Dudas y contradicciones

- Ninguna fuente encontrada habla específicamente del circuito "estudiante trae ropa de España para revender en Argentina"; toda la evidencia complementaria es del problema más amplio (estafas en reventa por redes sociales en general).
- Las fuentes oficiales (UFECI, BA-CSIRT, La Nación) ponen el foco en el **riesgo de la transferencia irreversible**, más que en el miedo a recibir una réplica. Esto contradice el énfasis inicial del equipo, que había puesto el foco principal en el miedo a la réplica.
- Contradicción identificada en las fuentes: los usuarios buscan comprar en el mercado secundario (revendedores) para conseguir precios más bajos que en los shoppings de Argentina, pero al mismo tiempo exigen el mismo nivel de certidumbre y garantías que ofrece el retail oficial.

---

## 3. Fichas de problemas

### Problema A1: Desconfianza en la autenticidad del producto (miedo a la réplica)

| Campo | Respuesta |
|---|---|
| Problema observado | Miedo a pagar por una prenda de marca y recibir una falsificación. |
| Usuario | Estudiante argentino que compra ropa importada a un revendedor informal. |
| Contexto | Al recibir fotos del producto antes de la entrega, sin poder verlo ni tocarlo. |
| Progreso buscado | Adquirir una prenda genuina a menor precio que en tienda oficial. |
| Fricción observada | Imposibilidad de verificar la autenticidad a distancia. |
| Consecuencia | Desgaste de tiempo pidiendo pruebas (fotos de etiquetas, costuras, ticket) o abandono de la compra. |
| Evidencia | Grupos de Facebook y foros de moda pidiendo pruebas de autenticidad; mercado global de servicios de "legit check" con apps de IA y tarifas de 10–30 €. |
| Fuentes | Grupos de Facebook ("Legit Check Arg"), foros de moda, Limited Resell, Google Play. |
| Frecuencia aparente | Frecuente en el research original; sin confirmación en fuentes oficiales argentinas. |
| Comportamiento observable | Pide fotos específicas (etiquetas, costuras, código de artículo); sube imágenes a foros para validación externa. |
| Alternativas actuales | Validadores comunitarios (grupos de FB) o pagar el precio completo en tienda oficial. |
| Acceso a usuarios | Sí, a través de redes sociales, foros o el propio entorno de estudiantes. |
| Supuestos | Que el miedo a la réplica, por sí solo, es suficiente para frenar una compra. |
| Evidencia faltante | Ningún caso documentado de un comprador argentino que haya recibido efectivamente una réplica en este circuito específico. |

### Problema A2: Desconfianza en la transacción (miedo a la estafa financiera / pago sin recibir nada)

| Campo | Respuesta |
|---|---|
| Problema observado | Miedo a transferir dinero por adelantado a un vendedor desconocido y no recibir el producto. |
| Usuario | Estudiante argentino que compra ropa importada a un revendedor informal por Instagram u otra red. |
| Contexto | Al momento de tener que pagar una seña o el total antes de ver la prenda en persona. |
| Progreso buscado | Concretar la compra sin arriesgar la pérdida total del dinero. |
| Fricción observada | El pago se hace por transferencia bancaria directa, sin mecanismo de reversión ni garantía. |
| Consecuencia | Pérdida irrecuperable del dinero si el vendedor no entrega; trámite de denuncia largo y de baja efectividad. |
| Evidencia | UFECI reportó aumento de casos de compradores que pagan y nunca reciben el producto (dic 2024–ene 2025); BA-CSIRT: más del 50% de fraudes reportados en 2024 vinculados a Instagram; La Nación: denuncias de fraude en compraventa pasaron de 603 a 5200 casos/año; caso judicial documentado de un vendedor que cobró y desapareció. |
| Fuentes | UFECI, BA-CSIRT (Gobierno de la Ciudad), La Nación, Diario de Cuyo. |
| Frecuencia aparente | Alta a nivel país (según fuentes oficiales); sin dato específico del nicho de ropa importada. |
| Comportamiento observable | Ansiedad al momento de transferir; revisión de seguidores y comentarios del vendedor antes de pagar. |
| Alternativas actuales | Pedir entrega presencial antes del pago total, pedir referencias de conocidos, o desistir de la compra. |
| Acceso a usuarios | Sí, en el mismo entorno universitario. |
| Supuestos | Que este patrón general de fraude en Instagram se traslada igual al nicho específico de ropa importada de estudiantes. |
| Evidencia faltante | Ningún dato desagregado por rubro (ropa vs. otros productos) ni por edad del comprador; dato de denuncias más reciente que 2022. |

### Problema B: Riesgo de talla sin posibilidad de prueba o devolución

| Campo | Respuesta |
|---|---|
| Problema observado | Miedo a equivocarse de talla al comprar sin poder probarse la prenda previamente. |
| Usuario | Joven argentino interesado en indumentaria importada de reventa. |
| Contexto | Al comprar ropa traída del exterior a un particular, sin probadores ni políticas de cambio o devolución. |
| Progreso buscado | Adquirir una prenda que le quede bien sin arriesgarse a perder el dinero. |
| Fricción observada | Imposibilidad física de probarse la ropa y dificultad de hacer una devolución a un particular. |
| Consecuencia | No concreta la compra por aversión al riesgo, o tarda de más haciendo preguntas adicionales. |
| Evidencia | Consultas constantes y reiteradas sobre las medidas exactas en centímetros de las prendas. |
| Fuentes | Mensajes directos (DMs) y consultas públicas en Facebook, Marketplace e Instagram. |
| Frecuencia aparente | Frecuente, especialmente en prendas de calce específico (pantalones, calzado, camperas). |
| Comportamiento observable | Pide medidas en centímetros o va a medirse modelos similares a tiendas oficiales. |
| Alternativas actuales | Comprar un talle más grande por las dudas, o directamente no comprar. |
| Acceso a usuarios | Sí, fácilmente contactables en redes. |
| Supuestos | Que el miedo a equivocarse de talla es una fricción tan fuerte como el miedo a las réplicas. |
| Evidencia faltante | Validar si una tabla de medidas precisas por prenda es suficiente para comprar sin probarse. |

### Problema C: Falta de financiamiento accesible (cuotas sin interés)

| Campo | Respuesta |
|---|---|
| Problema observado | Imposibilidad de pagar precios altos en un solo pago. |
| Usuario | Estudiante argentino sin gran liquidez mensual en efectivo. |
| Contexto | Al momento de concretar el pago de una prenda de alto valor a un revendedor. |
| Progreso buscado | Financiar la compra sin comprometer todo el presupuesto mensual de una sola vez. |
| Fricción observada | Los revendedores priorizan efectivo/transferencia; el pago con tarjeta traslada intereses altos al comprador. |
| Consecuencia | La venta se cae en la instancia final de pago al conocer los recargos por tarjeta de crédito. |
| Evidencia | Preguntas constantes sobre métodos de pago y quejas cuando se informa el precio final financiado. |
| Fuentes | Comentarios en publicaciones y mensajes directos en showrooms de Instagram. |
| Frecuencia aparente | Muy frecuente, especialmente en la segunda quincena del mes o en productos exclusivos. |
| Comportamiento observable | Consulta opciones de financiamiento y abandona el carrito al calcular el interés final. |
| Alternativas actuales | Ahorra en moneda extranjera hasta pagar en efectivo, pide dinero prestado o desiste de la compra. |
| Acceso a usuarios | Sí, en el mismo entorno universitario. |
| Supuestos | Que la falta de cuotas reduce el mercado potencial a más de la mitad de los interesados reales. |
| Evidencia faltante | Qué porcentaje de recargo máximo estarían dispuestos a asumir por pagar en 3 cuotas. |

---

## 4. Limpieza y agrupación

- **Agrupaciones sugeridas por la IA (ronda 1):**
  - Agrupación A (Confianza y Autenticidad): combinaba "Desconfianza ante posibles réplicas", "Falta de confianza en el vendedor" y "Dificultad para comprobar el estado de la prenda".
  - Agrupación B (Aversión a la pérdida por error de talla): "Riesgo al no poder probarse la ropa ni devolverla".
  - Agrupación C (Barrera de liquidez): "Imposibilidad de pagar en cuotas sin recargos altos".
  - Solución disfrazada detectada: "Dificultad para coordinar la entrega" — descartada como problema central.

- **Decisión formal del equipo (tras el research complementario):** se separa definitivamente la Agrupación A en dos problemas independientes, **A1** (miedo a la réplica) y **A2** (miedo a la estafa financiera), en lugar de tratarlos como una sola barrera de "confianza".

- **Motivo de la separación:** la evidencia complementaria mostró que A1 y A2 tienen respaldo documental de calidad muy distinta. A2 está respaldado por fuentes oficiales de fraude (UFECI, BA-CSIRT, La Nación); A1 solo está respaldado por comportamiento observado en foros y por un mercado global de autenticación (Francia, sneakers), sin ningún caso argentino documentado. Evaluarlos juntos generaba una falsa sensación de solidez.

- **Problemas mantenidos separados:** riesgo de talle (Problema B) y falta de cuotas (Problema C), como problemas secundarios para futuras iteraciones.

- **Problema descartado:** "Dificultad para coordinar la entrega" — señalado como síntoma de un proceso logístico deficiente, no como necesidad fundamental del usuario.

- **Contradicciones y datos faltantes:**
  - Los usuarios buscan el mercado informal por precio, pero exigen las mismas garantías que el retail oficial.
  - No se sabe qué peso tiene la falta de cuotas frente al miedo a una réplica o a una estafa financiera.
  - No se ha confirmado si mostrar el ticket de compra europeo es realmente suficiente para generar confianza suficiente como para pagar una seña por adelantado.
  - Ninguna fuente oficial de fraude menciona réplicas como parte del patrón de estafa en Instagram — todas describen "pagué y no recibí nada", lo cual respalda más a A2 que a A1.

---

## 5. Evaluaciones ICE individuales

### Ignacio Urquiola

| Problema | Impact | Confidence | Ease | ICE | Justificación |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Problema A (Inseguridad/Estafas, combinado) | 9 | 8 | 9 | 6.48 | Sin confianza no hay venta; es el bloqueador principal. |
| Problema B (Talla) | 7 | 6 | 9 | 3.78 | Es real, pero mandando medidas exactas se mitiga bastante. |
| Problema C (Cuotas) | 8 | 5 | 9 | 3.60 | El público objetivo ya sabe que debe juntar el dinero de antemano. |

### Gabriela Mendoza

| Problema | Impact | Confidence | Ease | ICE | Justificación |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Problema A (Inseguridad/Estafas, combinado) | 8 | 7 | 9 | 5.04 | Grave, pero el ticket de compra europeo lo soluciona casi de inmediato. |
| Problema B (Talla) | 9 | 7 | 8 | 5.04 | Gravísimo; mucha gente no compra sin probarse. |
| Problema C (Cuotas) | 7 | 6 | 8 | 3.36 | La reventa entre particulares siempre fue al contado. |

### Jaime Leopold

| Problema | Impact | Confidence | Ease | ICE | Justificación |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Problema A (Inseguridad/Estafas, combinado) | 9 | 6 | 9 | 4.86 | Depende de la marca; con Zara hay más confianza que con lujo. |
| Problema B (Talla) | 6 | 6 | 9 | 3.24 | Con la moda oversize, errarle un poco ya no es tan grave. |
| Problema C (Cuotas) | 9 | 7 | 9 | 5.67 | Las cuotas destrabarían muchísimas ventas para un estudiante. |

### Eric Giménez

| Problema | Impact | Confidence | Ease | ICE | Justificación |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Problema A (Inseguridad/Estafas, combinado) | 8 | 8 | 8 | 5.12 | Es lo que más se lee en los foros. |
| Problema B (Talla) | 8 | 5 | 9 | 3.60 | Afecta más a ciertas prendas específicas. |
| Problema C (Cuotas) | 7 | 6 | 9 | 3.78 | El que busca revendedores ya está mentalizado a transferir. |

---

## 6. Evaluación ICE con IA

### 6.1 Primera ronda (problema A combinado)

| Problema | Impact | Confidence | Ease | ICE |
| :--- | :---: | :---: | :---: | :---: |
| Problema A (Inseguridad/Estafas, combinado) | 8 | 7 | 9 | 5.04 |
| Problema B (Talle sin prueba) | 7 | 6 | 9 | 3.78 |
| Problema C (Falta de Cuotas) | 6 | 4 | 9 | 2.16 |

### 6.2 Segunda ronda (con evidencia complementaria, A todavía combinado)

| Problema | Impact | Confidence | Ease | ICE |
| :--- | :---: | :---: | :---: | :---: |
| Problema A (Inseguridad/Estafas) | 8 | 6 | 9 | 4.32 |
| Problema B (Talle sin prueba) | 7 | 6 | 9 | 3.78 |
| Problema C (Falta de Cuotas) | 6 | 4 | 9 | 2.16 |

### 6.3 Tercera ronda — evaluación final tras separar A1 y A2

**Problema A1: Desconfianza en la autenticidad del producto (miedo a la réplica)**
- Impact (7): genera fricción y desgaste de tiempo, pero no hay evidencia de pérdida total de dinero.
  - *Inferencia:* que este riesgo se percibe como grave sin haber sufrido nunca el daño real.
  - *Falta:* ningún caso documentado de un comprador argentino que haya recibido una réplica en este circuito.
- Confidence (6): señales consistentes de comportamiento, pero ninguna fuente oficial argentina menciona réplicas como patrón de estafa.
  - *Falta:* fuente argentina que confirme réplicas como motivo de fraude en este nicho.
- Ease (9): acceso directo e inmediato a estudiantes del entorno universitario.
- **ICE:** (7 × 6 × 9) / 100 = **3.78**

**Problema A2: Desconfianza en la transacción (miedo a la estafa financiera)**
- Impact (9): el daño es total e irreversible (pérdida completa del dinero transferido).
  - *Inferencia:* que este patrón general de Instagram se traslada igual al nicho de indumentaria importada.
  - *Falta:* ningún dato desagregado por rubro (ropa vs. otros productos).
- Confidence (7): evidencia diversa y de fuentes oficiales (fiscalía, gobierno, medios).
  - *Falta:* dato de denuncias más reciente que 2022; ninguna fuente segmenta por edad o tipo de producto.
- Ease (9): mismo acceso directo al segmento.
- **ICE:** (9 × 7 × 9) / 100 = **5.67**

**Problemas B y C:** sin evidencia complementaria nueva; se mantienen los puntajes de la ronda 2 (ICE 3.78 y 2.16 respectivamente).

### Tabla comparativa final

| Problema | Impact | Confidence | Ease | ICE | Incertidumbre principal |
|---|:---:|:---:|:---:|:---:|---|
| **A1 — Miedo a la réplica (producto)** | 7 | 6 | 9 | **3.78** | Sin evidencia argentina específica; solo evidencia global |
| **A2 — Miedo a la estafa financiera (transacción)** | 9 | 7 | 9 | **5.67** | Evidencia oficial fuerte pero no segmentada por rubro ni edad |
| **B — Riesgo de talle** | 7 | 6 | 9 | 3.78 | Sin datos de tasa real de abandono por esta causa |
| **C — Falta de cuotas** | 6 | 4 | 9 | 2.16 | Evidencia mayormente indirecta |

### Advertencias de la IA sobre información faltante

- No se encontró ninguna fuente que documente estafas específicamente en el circuito de reventa de indumentaria importada por estudiantes.
- No hay datos que indiquen si el comprador de este nicho teme más a la réplica (A1) o a la estafa financiera (A2); solo hay evidencia de que A2 está mejor documentado a nivel país.
- No se sabe si los estudiantes conocen o usan servicios de autenticación tipo "Legit Check", o si resuelven todo de forma informal.
- El dato de denuncias de fraude en compraventa (La Nación) es de 2022; falta una cifra más reciente.
- Ninguna fuente oficial consultada segmenta los fraudes por rubro ni por edad del comprador.
- La IA no eligió un problema ganador: A2 obtuvo el ICE más alto de todos los evaluados, pero esto no prueba que sea "el problema correcto" — solo que tiene mejor respaldo documental hasta este punto.

---

## 7. Comparación de evaluaciones humano-IA

- **Principales coincidencias:** tanto el equipo como la IA coinciden en que el Impacto del problema de confianza/estafa es alto (8-9) y en que la Facilidad de acceso a usuarios es máxima (9) en todos los problemas evaluados.
- **Principales diferencias:** algunos integrantes puntuaron la Confianza con un 8, asumiendo que los reclamos en foros equivalen a ventas caídas. La IA fue más cautelosa (6-7), y al separar A1 de A2 mostró que la confianza combinada (6) escondía una asimetría: A2 solo, con evidencia oficial, merecería un 7; A1 solo, sin evidencia argentina, se queda en 6.
- **Puntajes modificados y motivo:** se ajustó el Confidence del problema de confianza consolidado a 7 en la ronda 1, y luego se dividió el problema en A1 (Confidence 6) y A2 (Confidence 7) en la ronda 3, tras aceptar que mezclarlos generaba una falsa sensación de solidez.
- **Inferencias o errores detectados en la IA:** la IA inicialmente confiaba en que mostrar el ticket de compra resolvía la desconfianza; el research complementario mostró que las fuentes oficiales de fraude no mencionan el ticket como mitigador, lo cual corrige ese sesgo.
- **Incertidumbres que permanecen:** si el verdadero freno es la réplica, la estafa financiera, o ninguna de las dos y en realidad es otro factor (precio, liquidez, talle); si mostrar el ticket y coordinar entrega en la universidad reduce el miedo a estafa financiera.

> **La IA es un segundo evaluador, no un árbitro.**

---

## 8. Crítica del problema finalista

**Problema evaluado:** A2 — Desconfianza en la transacción / miedo a la estafa financiera (pago sin recibir nada). ICE 5.67, finalista tras la separación de la Agrupación A.

- **Debilidades encontradas:**
  - El Impact (9) y la Confidence (7) se apoyan casi enteramente en fuentes oficiales de fraude en Instagram **en general**, no en ningún caso documentado del circuito específico "estudiante revende ropa traída de España". Es una extrapolación, no evidencia directa del nicho.
  - Ninguna fuente segmenta los fraudes por rubro (ropa vs. electrónica, entradas, etc.) ni por edad del comprador, por lo que no sabemos si los estudiantes universitarios están tan expuestos como el usuario promedio de Instagram que describen esas estadísticas.
  - El dato más citado (La Nación, denuncias de 603 a 5200 casos/año) es de 2022; no hay confirmación de que la tendencia se haya mantenido igual en 2025-2026.
  - Ease sigue siendo 9 en los cuatro problemas evaluados (A1, A2, B y C), por lo que no diferencia nada entre ellos. Esto obliga a preguntarse si A2 quedó primero solo porque Impact y Confidence se inflaron con evidencia general, no porque haya una razón específica del nicho para priorizarlo sobre B o C.

- **Explicaciones alternativas:**
  - El monto de dinero en juego podría ser el verdadero factor decisivo (a mayor precio, mayor parálisis), independientemente de si el miedo se nombra como "estafa" o como cualquier otra excusa.
  - Los estudiantes podrían evitar este riesgo simplemente pagando siempre contra entrega, en cuyo caso el "miedo a la estafa" existiría como preocupación abstracta pero no como barrera real que frene transacciones.
  - Podría ser un problema genérico de "comprar por redes sociales a un desconocido" que no tiene nada de particular en el circuito de ropa importada, y que por lo tanto no amerita ser el foco de este proyecto específico.

- **Evidencia que podría refutarlo:**
  - Si en las entrevistas los estudiantes dicen que nunca pagan por adelantado y por eso nunca sintieron este riesgo como bloqueante, eso refutaría que A2 sea una barrera real en este nicho, aunque el miedo exista en abstracto.
  - Si describen que resuelven esto con acuerdos informales dentro del propio círculo universitario (conocidos, recomendaciones boca a boca) sin necesidad de ningún mecanismo adicional, esto debilitaría el Impact y la Confidence asignados.
  - Si el motivo real de no comprar termina siendo otro (precio, talle, falta de stock) y la desconfianza aparece solo como excusa secundaria, eso también refutaría la priorización actual.

- **Respuesta del equipo:**
  - _(Pendiente de completar por el equipo tras discutirlo.)_

---

## 9. Decisión humana

> **Pendiente de actualizar.** La decisión original (ver versión anterior del archivo) había priorizado el problema de "Confianza y Autenticidad" combinado. Tras la separación en A1/A2 y la nueva evaluación ICE (A2 = 5.67, el puntaje más alto de los cuatro problemas), el equipo debe decidir formalmente:
> - Si prioriza A2 en solitario,
> - Si prefiere seguir investigando A1 y A2 juntos en las mismas entrevistas para no perder de vista ninguno de los dos miedos,
> - O si, tras la crítica del Paso 8, prefiere mantener dos finalistas hasta tener evidencia real.

Plantilla a completar:

```text
Priorizamos este problema porque:

El criterio ICE más sólido es:

El criterio ICE más incierto es:

La evidencia más fuerte que tenemos es:

La principal debilidad de nuestra elección es:

Podríamos estar equivocados si:

La próxima evidencia que necesitamos obtener es:
```

---

## 10. Problema priorizado

> **Pendiente de redacción final.** La redacción anterior del equipo (ver historial) describía el problema de "Confianza y Autenticidad" de forma combinada. Dado que ahora se distinguen A1 y A2 con evidencia y puntajes ICE distintos, se recomienda redactar el problema priorizado nuevamente una vez que el equipo complete la Decisión humana (sección 9), dejando explícita cuál de las dos incertidumbres (o ambas) se investigará primero.

### Puntaje ICE de referencia

- **A1 (réplica):** Impact 7, Confidence 6, Ease 9 → ICE 3.78
- **A2 (estafa financiera):** Impact 9, Confidence 7, Ease 9 → ICE 5.67

### Redacción final

_(Pendiente — completar tras la Decisión humana del Paso 9.)_

### Justificación

_(Pendiente.)_

---

## 11. Personas sintéticas y entrevistas

### Persona sintética 1: El "Legit Checker" Experto

- **Contexto:** Estudiante que consume frecuentemente indumentaria de marca y conoce la existencia de réplicas de altísima calidad en el mercado informal.
- **Objetivo o progreso buscado:** Conseguir indumentaria 100% original a menor precio que en el retail oficial, asegurando su autenticidad.
- **Comportamientos:** Pide de 3 a 5 fotos específicas (etiquetas interiores, costuras, código de artículo). Sube imágenes a foros o grupos de Facebook para que terceros las validen.
- **Frustraciones:** El desgaste de tiempo que le genera verificar cada compra y lidiar con vendedores que se ofenden al pedirles el ticket de origen.
- **Restricciones:** No concreta la transacción si falta una sola prueba visual o si el ticket de compra no coincide exactamente.
- **Alternativas actuales:** Utiliza validadores comunitarios (grupos de FB) o termina pagando el precio completo en la tienda oficial.
- **Evidencia que la respalda:** Actividad observable en grupos como "Legit Check Arg" y exigencia reiterada de fotos de etiquetas.
- **Supuestos incorporados:** Asumimos que su miedo principal es *la calidad del producto* (recibir una réplica) y no necesariamente que el vendedor desaparezca con la plata.
- **Preguntas para personas reales:** ¿Qué comprobante específico eliminaría por completo tu necesidad de consultar en un foro antes de comprar?

### Persona sintética 2: El Comprador Primerizo Temeroso

- **Contexto:** Estudiante con presupuesto ajustado que quiere comprar una prenda importada a un precio más accesible a través de Instagram.
- **Objetivo o progreso buscado:** Ahorrar dinero en su compra sin caer en una estafa virtual donde pierda sus ahorros.
- **Comportamientos:** Revisa compulsivamente la cantidad de seguidores del vendedor, lee todos los comentarios buscando quejas, y duda días antes de enviar el primer mensaje.
- **Frustraciones:** Siente mucha ansiedad al momento de tener que enviar una "seña" o pago por adelantado a un CBU desconocido.
- **Restricciones:** No sabe cómo distinguir una prenda original de una réplica por foto. Su presupuesto no le permite asumir riesgos.
- **Alternativas actuales:** Le pide a conocidos que viajan al exterior que le traigan la ropa, o directamente abandona la compra.
- **Evidencia que la respalda:** Compradores revisando comentarios y experiencias; parálisis por análisis y carritos abandonados.
- **Supuestos incorporados:** Asumimos que su miedo principal es *la estafa financiera* (transferir y ser bloqueado), más que el hecho de que la prenda sea una réplica.
- **Preguntas para personas reales:** Si el vendedor te propone entregar en un lugar público y seguro, ¿cambia tu disposición a transferir una seña?

### Aprendizajes del role-play

- **Nuevas hipótesis:** El usuario valora mucho su tiempo; la fricción de pedir fotos y esperar validaciones externas es tan alta que a veces anula el beneficio de pagar menos, llevándolo a abandonar la compra informal.
- **Contradicciones detectadas:** El usuario busca el mercado informal para ahorrar, pero exige el mismo nivel de garantías y seguridad que el retail oficial.
- **Afirmaciones sin respaldo:** Asumimos que "los vendedores se ofenden" cuando se les piden pruebas, pero solo tenemos la perspectiva del comprador.
- **Respuestas que deben validarse:** Necesitamos descubrir en qué momento exacto de la interacción (el punto de quiebre) el usuario decide definitivamente abandonar la compra.

### Guion de entrevista real

> **Nota importante:** dado el research complementario, se recomienda que las preguntas 3-6 distingan explícitamente entre el miedo a la réplica (producto) y el miedo a la estafa financiera (transacción), en lugar de tratarlos como una sola inquietud.

1. Contame sobre la última vez que le compraste, o intentaste comprarle, ropa importada a un revendedor por Instagram u otra red social.
2. ¿Cómo fue el paso a paso desde que viste la prenda publicada hasta que tomaste la decisión de avanzar o frenar la compra?
3. En ese momento, antes de confirmar, ¿cuál fue tu principal duda o preocupación: la originalidad de la prenda, la seguridad de transferir el dinero, u otra cosa?
4. ¿Qué hiciste exactamente para intentar resolver esa duda por tu cuenta?
5. ¿Qué le pediste o qué le preguntaste al vendedor en esa ocasión?
6. ¿Qué información o respuesta te dio el vendedor? ¿Cómo te hizo sentir eso?
7. ¿Cómo acordaron manejar el tema del pago y la entrega esa vez?
8. Recordando el momento exacto en el que tenías que hacer la transferencia o pagar, ¿qué pasó por tu cabeza?
9. Si al final decidiste no comprar, ¿qué terminaste haciendo para conseguir ropa de ese estilo?

### Plan de entrevistas

| Decisión | Definición del equipo |
| :--- | :--- |
| **Perfil de entrevistados** | Estudiantes universitarios argentinos que hayan comprado o intentado comprar ropa importada a revendedores en los últimos 6 meses. |
| **Cantidad mínima** | 4 personas (una por cada integrante del equipo). |
| **Forma de contacto** | Mensaje directo por WhatsApp o intercepción presencial en el patio y pasillos de la facultad. |
| **Responsable de entrevistar** | 2 integrantes asumirán el rol principal de conducción (rotativo). |
| **Responsable de registrar** | 2 integrantes tomarán notas en vivo y registrarán las citas textuales (rotativo). |
| **Evidencia que se recopilará** | Notas escritas, citas textuales sobre el momento de mayor fricción y validación de si el bloqueo principal es el miedo a la réplica (A1) o el miedo a la transferencia por adelantado (A2). |
| **Fecha límite** | Antes de la Clase 3. |

---

## 12. Revisar y entregar

### Lista de verificación

- [x] Territorio: dominio, usuario, contexto, supuestos y límites.
- [x] Entre 5 y 10 problemas potenciales (research original + complementario).
- [x] Fuentes originales y verificables.
- [x] Fichas completas de los problemas finalistas (A1, A2, B, C).
- [x] Agrupaciones sugeridas por la IA y decisiones del equipo.
- [x] Evaluaciones ICE individuales.
- [x] Evaluación ICE de la IA con justificaciones (3 rondas).
- [x] Comparación entre evaluaciones.
- [x] Crítica escéptica del problema finalista (A2).
- [ ] Decisión humana justificada — **pendiente de actualizar tras la separación A1/A2.**
- [ ] Redacción final del problema — **pendiente.**
- [x] Dos personas sintéticas.
- [x] Aprendizajes del role-play.
- [x] Guion y plan para entrevistar al menos a tres personas reales.
- [x] Supuestos pendientes y evidencia que podría refutarlos.

### Cierre del equipo

```text
El problema que decidimos investigar es:
La inseguridad transaccional que experimentan los estudiantes universitarios al intentar
comprar indumentaria importada a revendedores informales por redes sociales. Se identificaron
dos componentes con evidencia de peso distinto: el miedo a recibir una réplica (A1) y el miedo
a la estafa financiera al transferir dinero por adelantado (A2). Este último cuenta con mejor
respaldo documental (fuentes oficiales de fraude en Argentina).

La evidencia más fuerte que encontramos es:
Los reportes de UFECI y BA-CSIRT sobre el crecimiento de fraudes en Instagram en Argentina
(más del 50% de los casos reportados en 2024), y el comportamiento observable en grupos de
Facebook como "Legit Check Arg" exigiendo pruebas de autenticidad.

El supuesto más riesgoso es:
Asumir que demostrar que la prenda es original (mostrando el ticket de España) alcanza para
generar confianza suficiente, cuando la evidencia sugiere que el verdadero freno podría ser
el riesgo financiero de transferir dinero por adelantado a un desconocido, independientemente
de la autenticidad del producto.

La pregunta más importante para los usuarios reales es:
Recordando el momento exacto en el que tenías que hacer la transferencia o pagarle por
adelantado a un revendedor, ¿qué pasó por tu cabeza y cuál fue el factor definitivo que te
hizo avanzar o cancelar la compra: la duda sobre el producto o la duda sobre el vendedor/pago?
```

---

# Entregable para la Clase 3

## 1. Este archivo (`clase-02-descubrimiento.md`)

Completo, con las siguientes secciones marcadas explícitamente como pendientes de cerrar antes de la Clase 3:
- Sección 8 — Respuesta del equipo a la crítica del problema finalista.
- Sección 9 — Decisión humana (actualizar tras separar A1/A2).
- Sección 10 — Redacción final del problema priorizado.

## 2. Registro de entrevistas reales

> **Pendiente.** Todavía no se realizaron las entrevistas reales; deben completarse antes de la Clase 3 según el Plan de entrevistas (Sección 11). Usar el siguiente formato por cada entrevista:

```markdown
## Entrevista [NÚMERO]

- Fecha:
- Entrevistador/a:
- Perfil de la persona:
- Contexto de la conversación:

### Situaciones reales relatadas

- 

### Comportamientos y alternativas actuales

- 

### Consecuencias observadas

- 

### Frases relevantes

- 

### Contradicciones con nuestra hipótesis

- 

### Nuevos aprendizajes

- 

### Cambios que haríamos a la redacción del problema

- 
```

## 3. Hallazgos, contradicciones y cambios al problema inicial

> **Pendiente**, a completar una vez realizadas las tres entrevistas reales mínimas. Debe indicar explícitamente si la evidencia real confirmó que el freno principal es A1 (réplica), A2 (estafa financiera), ambos, o ninguno de los dos.
