# Data Analytics Course for EduPlatform

[![Status](https://img.shields.io/badge/Status-In%20Development-yellow)]()
[![Modules](https://img.shields.io/badge/Modules-8-blue)]()
[![Exercises](https://img.shields.io/badge/Exercises-69%20planned-green)]()

Curso completo de Data Analytics con Python, migrado desde [101_Data_Analytics_Rizoma](https://github.com/gonzalezulises/101_Data_Analytics_Rizoma) para la plataforma [EduPlatform](https://github.com/gonzalezulises/edu-platform).

## 📋 Descripción

Este curso cubre las tres direcciones principales de Business Analytics:

| Tipo | Pregunta | Técnicas |
|------|----------|----------|
| **Descriptivo** | ¿Qué pasó? | Pandas, EDA, Visualización |
| **Predictivo** | ¿Qué pasará? | Regresión, Clasificación |
| **Prescriptivo** | ¿Qué hacer? | Clustering, Segmentación |

## 🗂 Estructura del Curso

| Módulo | Título | Ejercicios | Estrategia |
|--------|--------|------------|------------|
| 01 | Introducción a Python | 12 | Granular |
| 02 | Obtención de Datos con Pandas | 10 | Granular |
| 03 | Análisis Exploratorio (EDA) | 12 | Granular |
| 04 | Visualización de Datos | 10 | Granular |
| 05 | Modelos de Pronóstico | 6 + Colab | Híbrido |
| 06 | Clasificación | 6 + Colab | Híbrido |
| 07 | Clustering | 5 + Colab | Híbrido |
| 08 | Dashboards Interactivos | 8 | Granular |

**Total:** 69 ejercicios interactivos + 4 notebooks de Colab

## 🚀 Progreso de Migración

Ver [ROADMAP.md](ROADMAP.md) para el estado detallado de cada tarea.

```
[░░░░░░░░░░] 0% - En planificación
```

### Hitos

- [ ] **Fase 1:** Estructura base ✅ (completada)
- [ ] **Fase 2:** Módulo 1 - Python básico
- [ ] **Fase 3:** Módulos 2-4 (Pandas, EDA, Visualización)
- [ ] **Fase 4:** Módulos 5-8 (ML + Dashboards)
- [ ] **Fase 5:** Base de datos y deploy

## 📁 Estructura de Archivos

```
data-analytics-course/
├── content/
│   ├── courses/
│   │   └── data-analytics/
│   │       ├── course.yaml           # Metadata del curso
│   │       ├── COURSE_STATE.yaml     # Contrato pedagógico
│   │       └── module-XX/
│   │           ├── module.yaml
│   │           ├── lessons/*.md
│   │           └── exercises/*.yaml
│   └── shared/
│       ├── datasets/                 # CSVs compartidos
│       └── schemas/                  # SQL schemas
├── supabase/
│   └── migrations/                   # SQL para Supabase
├── docs/                             # Documentación adicional
├── ROADMAP.md                        # Tareas pendientes
└── README.md
```

## 🛠 Tecnologías

- **Plataforma:** [EduPlatform](https://github.com/gonzalezulises/edu-platform)
- **Runtime Python:** Pyodide (WebAssembly)
- **Runtime SQL:** sql.js (WebAssembly)
- **Editor:** Monaco Editor
- **Notebooks:** Google Colab (para ejercicios que requieren GPU)
- **Dashboards:** Plotly + Streamlit

## 📊 Datasets

| Dataset | Módulos | Descripción |
|---------|---------|-------------|
| drinks.csv | 02 | Consumo de alcohol por país |
| movies.csv | 02 | Usuarios de MovieLens |
| ufo.csv | 03 | Avistamientos de OVNIs |
| titanic.csv | 03, 06 | Pasajeros del Titanic |
| tips.csv | 04 | Propinas en restaurante |
| iris.csv | 04 | Dataset clásico de clasificación |
| bikeshare.csv | 05 | Demanda de bicicletas |
| customers.csv | 07 | Clientes para segmentación |

## 🔧 Desarrollo

### Prerrequisitos

1. Clonar el repositorio de EduPlatform
2. Copiar la carpeta `content/` a EduPlatform
3. Ejecutar migraciones de Supabase

### Crear ejercicios

Ver [COURSE_STATE.yaml](content/courses/data-analytics/COURSE_STATE.yaml) para:
- Convenciones de código
- Progresión pedagógica
- Especificación del próximo módulo

## 📝 Licencia

MIT License

## 👤 Autor

**Ulises González** - [Rizo.ma](https://rizo.ma)

---

*Migrado con asistencia de Claude Code*
