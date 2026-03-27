| ID | Riesgo | Impacto| Probabilidad | Nivel | Categoría | Mitigación |
| ----| ------ | ----- | -------------| -------| ---------- |  --------- |
| R1 | Permite comprar productos que no se encuentran en stock | 4 | 4 | 16 | Funcional | Validación de inventario en el checkout |
| R2 | No se agregan productos correctamente al carrito | 5 | 3 | 15 | Funcional | Pruebas de persistencia de sesión |
| R3 | Acceso no autorizado a cuentas por contraseñas débiles | 2 | 3 | 6 | Seguridad | Pruebas de autenticación y autorización, validación de políticas de contraseñas |
| R4 | Permite ingresar cantidades muy grandes en el checkout | 2 | 2 | 4 | Funcional | Validaciones de límite máximo en frontend y backend, pruebas de valores límite, pruebas de inputs inválidos |
| R5 | Falta de control de inventario | 5 | 4 | 20 | Funcional | Pruebas de consistencia de base de datos, simulación de ventas concurrentes |