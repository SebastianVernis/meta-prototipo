# meta-prototipo

Plataforma interna de la agencia para la **gestión centralizada de Pages de Meta**, con enfoque en **control, gobernanza y operación humana asistida**, sin automatización de interacciones sociales.

Este proyecto **no es un SaaS** ni una herramienta pública.  
Es una **infraestructura interna**, diseñada para escalar operación sin violar políticas de Meta ni asumir riesgos innecesarios.

---

## 🎯 Objetivo del proyecto

- Centralizar la gestión de múltiples Pages de Facebook / Instagram
- Publicar contenido vía API sin depender de Meta Business Suite
- Asistir (no automatizar) la operación humana mediante sugerencias
- Mantener trazabilidad, auditoría y control de fatiga
- Reducir riesgo operativo y dependencia de perfiles personales

---

## 🧭 Principios clave

- **Human-in-the-loop**: el sistema sugiere, las personas deciden
- **Nada de automatizar likes, comentarios o shares**
- **Gobernanza primero, volumen después**
- **Plataforma interna**, no producto comercial
- **Evolución incremental**, MVP temprano y estable

---

## 🧱 Stack tecnológico

### Backend
- Python
- FastAPI
- PostgreSQL (self-hosted)
- Alembic (migraciones)

### Frontend
- React
- Vite
- JavaScript (sin TypeScript por ahora)

### Infraestructura
- Docker / Docker Compose
- PostgreSQL en contenedor
- Redis (planeado, no inicial)
- Workers (planeados, no iniciales)

---

## 📁 Estructura del monorepo

```text
meta-prototipo/
├── backend/        # API y lógica de negocio (FastAPI)
├── frontend/       # Panel de operación (React)
├── scripts/        # Scripts auxiliares (Python / Node)
├── docs/           # Documentación técnica
├── docker-compose.yml
├── .env.example
└── README.md
```

## 🚦 Estado actual
Planeación: ✅ cerrada
Stack: ✅ definido
Roadmap: ✅ 16 semanas
Fase actual: Semana 1 – Arranque técnico
Desarrollo: en curso

## 🗺️ Roadmap (alto nivel)
Semana 1: Base técnica y scaffolding
Semanas 2–4: Publicación vía Meta API
Semanas 5–6: MVP operativo
Semanas 7–9: Sugerencias y cola de trabajo
Semanas 10–11: Auditoría y control
Semanas 12–13: KPIs de salud
Semanas 14–15: UX y refinamiento
Semana 16: Estabilización

## ⚠️ Fuera de alcance (por diseño)
Automatización de interacciones sociales
Simulación de comportamiento humano
Multi-tenant público
Escalado automático
Optimización prematura

## 🛠️ Cómo levantar el proyecto (placeholder)
Se completará al finalizar la Semana 1.
```bash
docker-compose up --build
```

### 📌 Nota final
Este repositorio prioriza control, claridad y estabilidad sobre velocidad o features.
Si algo no reduce riesgo u operación real, no entra.

