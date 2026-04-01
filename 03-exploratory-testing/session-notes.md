# Sesión 1
## Charter
Explorar el proceso de compra
usando flujos completos e incompletos, datos válidos e inválidos y múltiples confirmaciones
para descubrir errores en la generación de órdenes, duplicaciones y fallos en validaciones.
## ÁREAS
JPetStore
OS: Windows 10
Plataforma: Web (Chrome versión 145.0.7632.160 64 bits)
Estrategia: Exploración y Análisis

## INICIO
01/04/2026 10:30 am
## TESTER
Vivian Sánchez
## DESGLOSE DE TAREAS
Duración: 30 minutos
Diseño y ejecución de pruebas: 25 minutos
Investigación y reporte de defectos: 2 minutos
Preparación de la sesión: 3 minutos

## ARCHIVOS DE DATOS

## NOTAS DE PRUEBA
Se revisó el flujo de ckeckout con el siguiente esquema de cobertura:
Dispositivos/ Navegadores: Chrome (Desktop)
Flujos principales:
Selección de productos
Agregar al carrito
Checkout
Confirmación de pago

Interfaz
Carrito de compra
Checkout

Datos
Direcciones
Datos de tarjeta ficticios
## LISTA DE RIESGOS 
Compra de productos que no se encuentran en stock
Inconsistencia de datos en el carrito
Errores no controlados que afectan la experiencia de utilización del sistema

## DEFECTOS (BUGS) 
BUG #1
Error no controlado al no ingresar info de credit card: En el checkout, cuando no se ingresa el dato de la tarjeta de crédito y se presiona continuar, se visualiza un error 500 que no es amigable con el usuario.
## INCIDENTES (ISSUES) 
Se muestra un formato de ejemplo para el Expiry Date (MM/YYYY) pero no valida que los datos ingresados tengan sentido, ejemplo: se ingresa 21/2022 (mes que no existe, año ya pasado) y la compra de igual manera es exitosa.