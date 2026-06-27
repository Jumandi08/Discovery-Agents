# Personas y Stakeholders — Facturación electrónica

```mermaid
flowchart LR
  classDef src    fill:#E2EAF3,stroke:#1A4E8A,color:#0E1A26;
  classDef pri    fill:#E3F1E8,stroke:#2E7D52,color:#0E1A26;
  classDef pain   fill:#F6E3BC,stroke:#9A6605,color:#0E1A26;
  classDef stake  fill:#EDE7F6,stroke:#5E35B1,color:#0E1A26;

  E1[entrevista-01-comerciante.md]:::src   --> CM[C. Comerciante]:::pri
  E2[entrevista-02-renovaciones.md]:::src  --> PG[Proveedor / Gestor]:::pri
  E3[entrevista-03-onboarding.md]:::src    --> PG

  CM --> D1[errores-tecnicos-ininteligibles]:::pain
  CM --> D2[bloqueo-en-punto-de-venta]:::pain
  CM --> D3[firma-vencida-sin-aviso]:::pain
  CM --> D4[soporte-lento-sin-resolucion]:::pain
  CM --> D5[miedo-a-multas]:::pain

  PG --> D6[seguimiento-manual-firmas]:::pain
  PG --> D7[renovacion-reactiva]:::pain
  PG --> D8[costos-renovacion-urgente]:::pain
  PG --> D9[alta-manual-costosa]:::pain
  PG --> D10[soporte-repetitivo]:::pain
  PG --> D11[cuello-botella-personal]:::pain

  ST[Ente tributario]:::stake
```

> **Clave de color:** verde = primera mano · morado = stakeholder sin entrevista directa.

---

## Personas

### C. (comerciante) — comerciante obligado a facturación electrónica

- **Contexto:** pequeño comerciante con baja familiaridad tecnológica, migrado forzosamente a la facturación electrónica por mandato del ente tributario; opera en punto de venta con cliente presente.
- **Objetivo principal:** cobrar y emitir facturas sin necesidad de entender la tecnología subyacente ni depender de terceros para resolver problemas.
- **Dolores:**
  - Mensajes de error técnicos e incomprensibles bloquean la emisión de facturas en plena venta. `(entrevista-01-comerciante.md)`
  - No puede entregar la factura al cliente que ya pagó cuando el sistema falla. `(entrevista-01-comerciante.md)`
  - La firma electrónica venció sin aviso previo; estuvo varios días sin poder facturar, perdiendo ventas. `(entrevista-01-comerciante.md)`
  - El soporte telefónico tiene esperas largas y no resuelve de forma inmediata. `(entrevista-01-comerciante.md)`
  - Busca ayuda en familiares o YouTube, pero los recursos no aplican a su sistema concreto. `(entrevista-01-comerciante.md)`
  - Vive con estrés y miedo constante a ser multado por no poder emitir facturas. `(entrevista-01-comerciante.md)`
- **Respaldo:** `primera mano` — `entrevista-01-comerciante.md`

---

### Proveedor / Gestor — proveedor de facturación electrónica y firmas (gestor)

- **Contexto:** emprendedor que vende y administra servicios de facturación electrónica y firmas digitales para una cartera de múltiples comerciantes PYME; opera hoy con Excel, WhatsApp y trabajo completamente manual.
- **Objetivo principal:** escalar la cartera de clientes sin que su tiempo personal sea el cuello de botella.
- **Dolores:**
  - Controla vencimientos de firmas en Excel, WhatsApp o de memoria; no tiene alertas automáticas. `(entrevista-02-renovaciones.md)`
  - Se entera del vencimiento cuando el cliente ya está bloqueado y enojado. `(entrevista-02-renovaciones.md)`
  - Las renovaciones de último minuto generan recargos evitables y dañan la relación con el cliente. `(entrevista-02-renovaciones.md)`
  - El alta de cada cliente nuevo es completamente manual, consume horas y no reutiliza nada del proceso anterior. `(entrevista-03-onboarding.md)`
  - Las mismas 5–6 preguntas de soporte se repiten; responde copiando y pegando el mismo instructivo. `(entrevista-03-onboarding.md)`
  - Es el cuello de botella de su negocio: más clientes significan más horas personales, no crecimiento real. `(entrevista-03-onboarding.md)`
- **Respaldo:** `primera mano` — `entrevista-02-renovaciones.md`, `entrevista-03-onboarding.md`

---

## Stakeholders

### Ente tributario (SRI / DIAN / SUNAT según el país)

- **Interés en el sistema:** garantizar el cumplimiento de la obligación de facturación electrónica; es quien impone plazos, sanciones y la exigencia de la firma electrónica vigente.
- **Fuente:** `entrevista-01-comerciante.md` (mencionado como mandante de la migración obligatoria y fuente del riesgo de multas).

> Nota: no existe entrevista directa al ente tributario. Su rol es regulatorio y contextual; no es usuario del sistema pero define restricciones críticas de negocio.
