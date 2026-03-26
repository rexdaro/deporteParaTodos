Flujo básico
Usuario accede a la aplicación
Usuario inicia sesión o se registra
El sistema valida las credenciales
Se genera una sesión (token)
El usuario accede a funcionalidades protegidas

Registro
Endpoint
POST /api/auth/register
Datos requeridos
nombre
email
contraseña

Login
Endpoint
POST /api/auth/login
Resultado esperado
Token de autenticación
Datos básicos del usuario

Sesión
El token se envía en cada request protegido
Se recomienda usar Authorization Bearer Token
Authorization: Bearer <token>

Acciones que requieren autenticación
Crear partido
Reservar cancha
Confirmar asistencia
Registrar pagos
Ver partidos propios

Acciones sin autenticación
Ver canchas disponibles (opcional)
Ver información pública básica

Manejo de errores de autenticación
Token inválido → 401 Unauthorized
Token expirado → 401 Unauthorized
Sin permisos → 403 Forbidden

Consideraciones
Un usuario puede ser organizador y jugador
No se necesitan roles complejos para el MVP
La autenticación es obligatoria para acciones críticas

Conclusión
Este flujo asegura que:
Solo usuarios autenticados gestionen partidos
Se mantenga el control sobre acciones importantes
La app sea segura y escalable