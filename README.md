# flowguard-mocks

Fixtures de demostración para FlowGuard: escenarios de pago aprobado, bloqueado, y fallo de investigación, usados por el frontend en modo mock, por las pruebas de contrato y por los ensayos de demo.

**Responsable principal:** Dev 4 (contratos compartidos, mocks, pruebas, documentación, QA).

## Alcance

Según [flowguard-docs/architecture.md § 3](https://github.com/FlowGuard-Hackathon/flowguard-docs/blob/main/architecture.md#3-estructura-del-repositorio):

```
mocks/
├── payment-approved.json
├── payment-blocked.json
└── investigation-failed.json
```

Cada fixture debe validar contra los esquemas Zod de `flowguard-src/contracts/` y contra los contratos documentados en [flowguard-docs/api-contracts.md](https://github.com/FlowGuard-Hackathon/flowguard-docs/blob/main/api-contracts.md) — un fixture nunca se presenta como una respuesta generada en vivo (ver [flowguard-docs/demo-script.md § 3](https://github.com/FlowGuard-Hackathon/flowguard-docs/blob/main/demo-script.md#3-plan-de-contingencia-de-la-demo)).

## Dependencias de otros repos

- `flowguard-src`: los esquemas contra los que estos fixtures deben validar.
- `flowguard-app`: los consume en modo mock (Bloque 1 de la implementación).

Este repo todavía no tiene fixtures; está preparado para que Dev 4 empiece a publicarlos siguiendo el Bloque 1 de [flowguard-docs/implementation-checklist.md](https://github.com/FlowGuard-Hackathon/flowguard-docs/blob/main/implementation-checklist.md).
