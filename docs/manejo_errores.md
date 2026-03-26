Manejo de Errores – DPT

Errores de Reserva
Si la cancha no está disponible → mostrar mensaje claro
Evitar reservas duplicadas
Validar solapamiento de horarios

Errores de Usuario
Validar datos obligatorios (fecha, cancha, jugadores)
No permitir acciones sin autenticación
No permitir que un usuario modifique partidos de otro

Errores de Partido
No permitir unirse a partidos completos
No permitir confirmar asistencia dos veces
No permitir acciones si el partido está finalizado o cancelado

Errores de Pago
Evitar marcar pago duplicado
Validar monto correcto
Mostrar estado actualizado

Reglas de Mensajes al Usuario
Los errores deben ser claros y simples
Evitar mensajes técnicos
Explicar qué pasó y cómo solucionarlo

Formato de Error (Backend)
Todas las respuestas de error deben seguir una estructura estándar:

{
  "error": "tipo_error",
  "message": "mensaje claro",
  "status": 400
}

Códigos HTTP
400 – Bad Request
401 – Unauthorized
403 – Forbidden
404 – Not Found
409 – Conflict
500 – Internal Server Error