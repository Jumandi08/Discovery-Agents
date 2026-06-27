# Requisitos candidatos — Facturación electrónica

---

## Funcionales

- **[R-01]** El sistema debe mostrar mensajes de error en lenguaje comprensible para el usuario no técnico, con pasos concretos para resolverlos.
  - Tipo: funcional
  - Origen: `entrevista-01-comerciante.md` · C. (comerciante)

- **[R-02]** El sistema debe alertar al comerciante con anticipación suficiente cuando su firma electrónica esté próxima a vencer, sin depender de que el usuario lo recuerde.
  - Tipo: funcional
  - Origen: `entrevista-01-comerciante.md` · C. (comerciante)

- **[R-03]** El sistema debe alertar automáticamente al Proveedor/Gestor cuando la firma de cualquier cliente de su cartera esté próxima a vencer, con tiempo suficiente para renovar sin urgencia ni recargo.
  - Tipo: funcional
  - Origen: `entrevista-02-renovaciones.md` · Proveedor / Gestor

- **[R-04]** El sistema debe ofrecer un tablero al Proveedor/Gestor que liste todos sus clientes con el estado de cada firma: al día / por vencer / vencida.
  - Tipo: funcional
  - Origen: `entrevista-02-renovaciones.md` · Proveedor / Gestor

- **[R-05]** El sistema debe permitir configurar el canal de alerta por cliente (al menos: email o WhatsApp).
  - Tipo: funcional
  - Origen: `entrevista-02-renovaciones.md` · Proveedor / Gestor

- **[R-06]** El sistema debe automatizar o guiar digitalmente el proceso de alta de un cliente nuevo, reduciendo la intervención manual del gestor en la recolección de documentos.
  - Tipo: funcional
  - Origen: `entrevista-03-onboarding.md` · Proveedor / Gestor

- **[R-07]** El sistema debe ofrecer una base de conocimiento o asistente de autoservicio que responda las preguntas de soporte más frecuentes sin requerir intervención del gestor.
  - Tipo: funcional
  - Origen: `entrevista-03-onboarding.md` · Proveedor / Gestor

---

## No funcionales

- **[R-08]** Las alertas deben entregarse con suficiente anticipación para que la renovación se complete antes del vencimiento; la latencia máxima de entrega desde el trigger es de 5 minutos.
  - Tipo: no funcional (disponibilidad / tiempo de respuesta)
  - Origen: `entrevista-02-renovaciones.md` · Proveedor / Gestor

- **[R-09]** El tablero de vencimientos debe ser accesible desde dispositivo móvil sin instalación de software adicional.
  - Tipo: no funcional (accesibilidad)
  - Origen: `entrevista-02-renovaciones.md` · Proveedor / Gestor (gestiona hoy desde WhatsApp/móvil)

- **[R-10]** El canal de soporte para el comerciante debe garantizar un tiempo de primera respuesta que no bloquee una venta en curso (p. ej., menos de 15 minutos en horario comercial).
  - Tipo: no funcional (tiempo de respuesta / experiencia de usuario)
  - Origen: `entrevista-01-comerciante.md` · C. (comerciante)
