# Regla: Testing

- Todo cambio de comportamiento lleva test (TDD preferido: test primero).
- Un test prueba UNA cosa; el nombre describe el comportamiento esperado.
- Cubre caso feliz + caso borde + caso de error.
- No mockees lo que puedas probar de verdad; mockea solo I/O externo (red, disco).
- Los tests deben pasar localmente (`npm test`) antes de proponer un commit.
- Tests deterministas: nada de `sleep`, nada de dependencia de fecha/hora real.
