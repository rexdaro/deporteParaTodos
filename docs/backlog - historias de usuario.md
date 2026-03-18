Contexto del Proyecto – MVP Gestión de Partidos Deportivos
1. Información General
Tipo de aplicación: Web App / MVP
Objetivo: Permitir organizar partidos deportivos, reservar canchas, gestionar asistencia y controlar pagos entre jugadores.
Usuario principal:
Organizador de partidos deportivos amateurs que necesita coordinar cancha, jugadores y pagos de forma simple desde una aplicación.
Problema:
Actualmente la organización de partidos se realiza mediante múltiples mensajes en WhatsApp u otras plataformas, lo que genera desorden, confusión sobre horarios, asistencia y pagos.
Propuesta de valor:
Centralizar en una sola aplicación la reserva de canchas, confirmación de jugadores y gestión de pagos para simplificar la organización de partidos.
________________________________________
Arquitectura de IA utilizada en el análisis
Modelo elegido: GPT-5.3
Motivo: modelo rápido y preciso para tareas de generación de requerimientos.
Infraestructura: Cloud API
Motivo:
•	facilita trabajo remoto del equipo
•	no requiere infraestructura local
•	acceso a modelos actualizados
•	no se procesan datos sensibles
________________________________________
Core Feature del MVP
Organización de partidos deportivos con reserva de cancha, confirmación de jugadores y control de pagos.
________________________________________
Backlog Inicial (Historias de Usuario MVP)
Historia 1 — Reserva de cancha
Como organizador de un partido deportivo
Quiero reservar una cancha desde la aplicación
Para asegurar el lugar y horario del partido.
Criterios de aceptación
•	Ver canchas disponibles por fecha y horario
•	Seleccionar una cancha
•	Confirmar reserva
•	Registrar la reserva en el panel del dueño
Prioridad: Alta
________________________________________
Historia 2 — Confirmación de asistencia
Como organizador del partido
Quiero que los jugadores confirmen su asistencia
Para saber si el equipo estará completo.
Criterios de aceptación
•	Los jugadores reciben una invitación al partido
•	Pueden confirmar o rechazar asistencia
•	El organizador ve la lista de confirmaciones
Prioridad: Alta
________________________________________
Historia 3 — Gestión de pagos
Como organizador del partido
Quiero gestionar el pago de los jugadores
Para asegurar que todos paguen su parte de la cancha.
Criterios de aceptación
•	El sistema muestra el costo total de la cancha
•	El sistema divide el costo entre jugadores
•	El organizador ve quién pagó y quién no
Prioridad: Alta
________________________________________
Auditoría de Resultados de IA
Herramientas utilizadas
•	NotebookLM
•	ChatGPT
Resultado
Ambos modelos generaron historias de usuario correctas y alineadas con el objetivo del MVP. No se detectaron alucinaciones funcionales.
Observación
ChatGPT generó respuestas más técnicas, mientras que NotebookLM mantuvo un enfoque más general.

