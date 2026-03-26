Usuario: id, nombre, email, telefono, rol
relaciones: 1 usuario puede tener muchas reservas y muchos partidos, 1 usuario puede ser dueño de muchas canchas, 1 usuario puede tener muchos pagos, 1 usuario puede tener muchas participaciones.

Cancha: id, nombre, direccion, precio_por_hora, telefono, dueño_id, tipo_cancha
relaciones: 1 cancha puede tener muchas reservas y muchos partidos.

Reserva: id, cancha_id, usuario_id, fecha, hora_inicio, hora_fin, estado, precio.
relaciones: 1 reserva debe tener 0 o 1 partido y 1 cancha.

Partido: id, usuario_id, reserva_id, fecha, estado, cantidad_jugadores, costo_total.
relaciones: 1 partido debe tener 1 reserva, 1 partido puede tener muchos participantes, 1 partido puede tener muchos pagos.

Participacion: id, usuario_id, partido_id, estado.
relaciones: 1 participacion debe tener 1 usuario y 1 partido.

Pago: id, usuario_id, partido_id, monto, estado, metodo_pago, fecha_pago.
relaciones: 1 pago debe tener 1 usuario y 1 partido.