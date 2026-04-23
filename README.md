# Sección de Pádel — App

Aplicación web para gestionar la sección de pádel de un club deportivo. Cubre la gestión de rankings, inscripciones diarias, generación automática de partidos, registro de resultados y agenda de eventos.

> Estado: **Prototipo en desarrollo**

---

## Screenshots

### Ranking
![Ranking](docs/screenshots/ranking.png)

### Jugar — listas de inscripción
![Jugar](docs/screenshots/jugar.png)

### Partidos — generación automática
![Partidos](docs/screenshots/partidos.png)

### Resultados
![Resultados](docs/screenshots/resultados.png)

### Agenda
![Agenda](docs/screenshots/agenda.png)

### La sección — organigrama
![La sección](docs/screenshots/seccion.png)

---

## Funcionalidades principales

- **Ranking** — clasificación de jugadores con fórmula de eficacia y ajuste por pocos partidos
- **Jugar** — inscripción por día de la semana con reglas de apertura automática a las 19:00
- **Partidos** — generación automática por ranking según pistas disponibles, con formato rotativo de 3 sets
- **Resultados** — registro de partidos y actualización automática del ranking
- **Agenda** — calendario de eventos especiales (torneos, actividades sociales, escapadas)
- **La sección** — organigrama con datos de contacto de coordinadores

---

## Roles de usuario

| Rol | Permisos |
|---|---|
| Jugador | Lectura general · Inscribirse y darse de baja |
| Coordinador | Todo lo anterior · Introducir resultados · Generar partidos |
| Admin | Gestión completa de la aplicación |

---

## Stack tecnológico

| Capa | Tecnología |
|---|---|
| Frontend | Web app |
| Base de datos | Supabase |
| Autenticación | Supabase Auth + Google OAuth |
| Hosting | Vercel |

---

## Documentación

- [`REQUIREMENTS.md`](REQUIREMENTS.md) — requisitos funcionales completos del proyecto

---

## Estructura del repositorio

```
/
├── README.md
├── REQUIREMENTS.md
└── docs/
    └── screenshots/
        ├── ranking.png
        ├── jugar.png
        ├── partidos.png
        ├── resultados.png
        ├── agenda.png
        └── seccion.png
```

---

## Contexto del proyecto

La sección cuenta con aproximadamente 300 jugadores distribuidos entre dos centros: **Club Cornellà Up** y **Club Delfos**. El sistema actual está basado en un Google Sheet con JavaScript. Esta aplicación lo sustituye con una plataforma moderna, accesible para todos los jugadores desde el navegador.

---

## Pendiente

- [ ] Ponderación temporal del ranking
- [ ] Ranking Manual Override
- [ ] Panel de administración completo
- [ ] Notificaciones de apertura de listas y generación de partidos
- [ ] Perfil individual de jugador con historial
- [ ] Gestión de torneos internos
