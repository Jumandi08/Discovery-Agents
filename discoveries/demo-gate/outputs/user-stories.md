# User Stories — demo-gate

---

- **[US-01]** Como vendedor, quiero que el sistema de facturación complete el cobro sin errores mientras el cliente está presente, para no perder la venta en el momento decisivo.
  - Criterios de aceptación:
    - Dado que un cliente decide pagar, cuando el vendedor inicia el proceso de cobro, entonces el sistema lo completa sin interrupciones ni mensajes de error en al menos el 98 % de los intentos.
    - Dado que ocurre un error técnico, cuando el vendedor lo encuentra con el cliente enfrente, entonces el sistema no interrumpe indefinidamente la sesión — ofrece un camino de recuperación o reintento inmediato.
  - Fuente: `entrevista-vendedor-real.md`

- **[US-02]** Como vendedor, quiero entender qué falló y qué debo hacer a continuación cuando el sistema me muestra un error, para no quedarme paralizado frente al cliente.
  - Criterios de aceptación:
    - Dado que el sistema de facturación falla, cuando el error se muestra en pantalla, entonces el mensaje describe la causa en lenguaje no técnico y propone al menos una acción concreta (reintentar, contactar soporte, usar método alternativo).
    - Dado que el vendedor lee el mensaje de error, cuando sigue la acción sugerida, entonces puede completar o registrar la venta sin necesidad de llamar a soporte.
  - Fuente: `entrevista-vendedor-real.md`

- **[US-03]** Como vendedor, quiero poder contactar soporte técnico en menos de 5 minutos durante una venta activa, para resolver la falla antes de que el cliente se vaya.
  - Criterios de aceptación:
    - Dado que ocurre un fallo de facturación con un cliente presente, cuando el vendedor activa el canal de soporte de emergencia, entonces recibe atención o respuesta en 5 minutos o menos.
    - Dado que no hay agente disponible, cuando el vendedor solicita ayuda, entonces recibe al menos un procedimiento de emergencia documentado para continuar la venta manualmente.
  - Fuente: `entrevista-vendedor-real.md`
