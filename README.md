# Java-banking-system


API REST compacta diseñada para la gestión transaccional y el repaso de conceptos avanzados de backend en Java utilizando una arquitectura tradicional por capas.

## Estructura del Proyecto (N-Tier Architecture)
* **Presentación (Controllers):** Exposición de endpoints REST y validación de datos de entrada.
* **Negocio (Services):** Orquestación de la lógica financiera y gestión de transacciones (`@Transactional`).
* **Datos (Repositories):** Persistencia y acceso a datos mediante Spring Data JPA.

## Aspectos Técnicos a Repasar
1. **Aislamiento Transaccional:** Garantía de operaciones ACID en transferencias de fondos.
2. **Concurrencia:** Prevención de condiciones de carrera mediante bloqueos en la base de datos.
3. **Manejo de Excepciones:** Centralización de errores financieros (ej. saldos insuficientes) con respuestas HTTP semánticas.
