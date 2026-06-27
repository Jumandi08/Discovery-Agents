# User Stories — Facturación electrónica

Alcance: MVP de seguimiento proactivo de vencimientos de firmas digitales.

---

- **[US-01]** Como Proveedor/Gestor, quiero ver el estado de vencimiento de todas las firmas de mi cartera en un solo tablero para identificar de un vistazo quién necesita renovación antes de que se bloquee.
  - Criterios de aceptación:
    - Dado que tengo clientes registrados, cuando abro el tablero, entonces veo cada cliente con su estado (al día / por vencer / vencida) y los días restantes.
    - Dado un cliente con firma vencida, cuando lo veo en el tablero, entonces aparece destacado con estado rojo.
  - Fuente: `entrevista-02-renovaciones.md`

- **[US-02]** Como Proveedor/Gestor, quiero recibir una alerta automática cuando la firma de un cliente esté a N días de vencer para renovarla con anticipación y evitar recargo.
  - Criterios de aceptación:
    - Dado un cliente cuya firma vence en N días (configurable), cuando se cumple ese plazo, entonces recibo una notificación por el canal configurado (email o WhatsApp).
    - Dado que recibí la alerta, cuando la abro, entonces veo el nombre del cliente, la fecha exacta de vencimiento y un acceso directo al proceso de renovación.
  - Fuente: `entrevista-02-renovaciones.md`

- **[US-03]** Como Proveedor/Gestor, quiero que mis clientes reciban una alerta directa de vencimiento para que colaboren en el proceso de renovación sin que yo tenga que perseguirlos.
  - Criterios de aceptación:
    - Dado un cliente con alerta habilitada, cuando su firma esté a N días de vencer, entonces él recibe una notificación por el canal configurado.
    - Dado que el cliente recibió la alerta, cuando responde o toma acción, entonces el sistema registra el estado como "en gestión".
  - Fuente: `entrevista-02-renovaciones.md`

- **[US-04]** Como Proveedor/Gestor, quiero registrar la fecha de vencimiento de la firma de un cliente nuevo para que el sistema lo incluya en el seguimiento automático desde el primer día.
  - Criterios de aceptación:
    - Dado que doy de alta un cliente, cuando ingreso su fecha de vencimiento de firma, entonces el sistema lo agrega al tablero y programa sus alertas.
    - Dado un campo de fecha vacío, cuando intento guardar, entonces el sistema me lo indica y no guarda hasta completarlo.
  - Fuente: `entrevista-03-onboarding.md`
