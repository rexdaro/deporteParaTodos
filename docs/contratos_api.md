Base URL
/api

Usuarios
Crear usuario
POST /api/users
Obtener usuario por ID
GET /api/users/{id}

Canchas
Listar canchas
GET /api/canchas
Crear cancha
POST /api/canchas

Reservas
Ver disponibilidad de canchas
GET /api/reservas?fecha=YYYY-MM-DD
Crear reserva
POST /api/reservas

Body ejemplo:

{
  "cancha_id": 1,
  "fecha": "2026-01-01",
  "hora_inicio": "20:00",
  "hora_fin": "21:00"
}

Partidos
Crear partido
POST /api/partidos
Obtener partido por ID
GET /api/partidos/{id}

Participaciones
Confirmar o rechazar asistencia
POST /api/participaciones

Body ejemplo:

{
  "usuario_id": 1,
  "partido_id": 2,
  "estado": "confirmado"
}

Pagos
Registrar pago
POST /api/pagos

Body ejemplo:

{
  "usuario_id": 1,
  "partido_id": 2,
  "monto": 2000
}

Endpoint adicional
Obtener estado del partido
GET /api/partidos/{id}/estado

Debe devolver:

Lista de jugadores confirmados
Estado de pagos
Cupos disponibles

Reglas generales
Todos los endpoints deben validar datos de entrada
Usar códigos HTTP correctos (ver manejo_errores.md)
Respuestas en formato JSON
No exponer errores internos