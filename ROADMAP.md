# ROADMAP: Migración de Data Analytics a EduPlatform

Este documento rastrea todas las tareas necesarias para migrar el curso de Data Analytics a EduPlatform.

## 📊 Resumen de Progreso

| Fase | Descripción | Tareas | Completadas | Estado |
|------|-------------|--------|-------------|--------|
| 1 | Estructura base | 5 | 5 | ✅ Completada |
| 2 | Módulo 1 - Python | 8 | 0 | 🔲 Pendiente |
| 3 | Módulos 2-4 | 12 | 0 | 🔲 Pendiente |
| 4 | Módulos 5-8 | 12 | 0 | 🔲 Pendiente |
| 5 | Base de datos | 4 | 0 | 🔲 Pendiente |

---

## Fase 1: Estructura Base ✅

- [x] #1 Crear repositorio y estructura de carpetas
- [x] #2 Crear course.yaml con metadata
- [x] #3 Crear COURSE_STATE.yaml con progresión pedagógica
- [x] #4 Crear module.yaml para los 8 módulos
- [x] #5 Crear README.md y ROADMAP.md

**Tiempo estimado:** 2-3 horas  
**Tiempo real:** ~1 hora

---

## Fase 2: Módulo 1 - Introducción a Python 🔲

### Lecciones (5 archivos .md)

- [ ] #6 Crear `lessons/01-primeros-pasos.md`
  - Contenido: print, comentarios, primera ejecución
  - Embeds: ex-01-01-hello-world, ex-01-02-variables

- [ ] #7 Crear `lessons/02-tipos-datos.md`
  - Contenido: int, float, str, bool, operadores
  - Embeds: ex-01-03, ex-01-04, ex-01-05

- [ ] #8 Crear `lessons/03-colecciones.md`
  - Contenido: listas, diccionarios, indexing
  - Embeds: ex-01-06, ex-01-07, ex-01-08

- [ ] #9 Crear `lessons/04-control-flujo.md`
  - Contenido: if/elif/else, for, while
  - Embeds: ex-01-09, ex-01-10, ex-01-11

- [ ] #10 Crear `lessons/05-funciones.md`
  - Contenido: def, parámetros, return
  - Embeds: ex-01-12

### Ejercicios (12 archivos .yaml)

- [ ] #11 Crear ejercicio `ex-01-01-hello-world.yaml`
  ```yaml
  type: code-python
  difficulty: beginner
  concepts: [print]
  ```

- [ ] #12 Crear ejercicio `ex-01-02-variables.yaml`
  ```yaml
  type: code-python
  difficulty: beginner
  concepts: [variables, asignacion]
  ```

- [ ] #13 Crear ejercicios `ex-01-03` a `ex-01-12`
  - 03: Tipos de datos
  - 04: Operaciones aritméticas
  - 05: Strings y formato
  - 06: Crear listas
  - 07: Acceso a elementos
  - 08: Diccionarios
  - 09: if-else
  - 10: for loop
  - 11: while loop
  - 12: Funciones

**Tiempo estimado:** 4-6 horas  
**Dependencias:** Ninguna

---

## Fase 3: Módulos 2-4 (Pandas, EDA, Visualización) 🔲

### Módulo 2: Pandas

- [ ] #14 Mover datasets a `content/shared/datasets/`
  - drinks.csv
  - movies.csv (u.user)

- [ ] #15 Crear 4 lecciones de Pandas
  - 01-intro-pandas.md
  - 02-dataframes.md
  - 03-seleccion.md
  - 04-fuentes-datos.md

- [ ] #16 Crear 10 ejercicios de Pandas (ex-02-01 a ex-02-10)

### Módulo 3: EDA

- [ ] #17 Mover datasets EDA
  - ufo.csv
  - titanic.csv

- [ ] #18 Crear 4 lecciones de EDA
  - 01-estadisticas-descriptivas.md
  - 02-agrupacion.md
  - 03-datos-faltantes.md
  - 04-combinacion.md

- [ ] #19 Crear 12 ejercicios de EDA (ex-03-01 a ex-03-12)

### Módulo 4: Visualización

- [ ] #20 Mover datasets visualización
  - tips.csv (o usar builtin de seaborn)
  - iris.csv

- [ ] #21 Crear 4 lecciones de Visualización
  - 01-matplotlib-basico.md
  - 02-histogramas-boxplots.md
  - 03-seaborn.md
  - 04-plotly-interactivo.md

- [ ] #22 Crear 10 ejercicios de Visualización (ex-04-01 a ex-04-10)

**Tiempo estimado:** 6-8 horas por módulo (18-24 horas total)  
**Dependencias:** Fase 2 completada

---

## Fase 4: Módulos 5-8 (ML + Dashboards) 🔲

### Módulo 5: Regresión

- [ ] #23 Mover dataset bikeshare.csv

- [ ] #24 Crear 4 lecciones de Regresión
  - 01-intro-ml.md
  - 02-regresion-lineal.md
  - 03-evaluacion-modelos.md
  - 04-practica-bikeshare.md (link a Colab)

- [ ] #25 Crear 6 ejercicios de Regresión (ex-05-01 a ex-05-06)

- [ ] #26 Crear notebook Colab para práctica Bikeshare

### Módulo 6: Clasificación

- [ ] #27 Crear 4 lecciones de Clasificación
  - 01-regresion-logistica.md
  - 02-matriz-confusion.md
  - 03-arboles-decision.md
  - 04-practica-titanic.md

- [ ] #28 Crear 6 ejercicios de Clasificación (ex-06-01 a ex-06-06)

- [ ] #29 Crear notebook Colab para Titanic

### Módulo 7: Clustering

- [ ] #30 Crear dataset sintético customers.csv

- [ ] #31 Crear 4 lecciones de Clustering
  - 01-intro-clustering.md
  - 02-kmeans.md
  - 03-dbscan.md
  - 04-practica-segmentacion.md

- [ ] #32 Crear 5 ejercicios de Clustering (ex-07-01 a ex-07-05)

- [ ] #33 Crear notebook Colab para Segmentación

### Módulo 8: Dashboards (reemplaza Tableau)

- [ ] #34 Crear 4 lecciones de Dashboards
  - 01-plotly-avanzado.md
  - 02-graficos-combinados.md
  - 03-streamlit-intro.md
  - 04-dashboard-completo.md

- [ ] #35 Crear 8 ejercicios de Dashboards (ex-08-01 a ex-08-08)

**Tiempo estimado:** 4-6 horas por módulo (16-24 horas total)  
**Dependencias:** Fase 3 completada

---

## Fase 5: Base de Datos y Deploy 🔲

- [ ] #36 Crear migración SQL para Supabase
  ```
  supabase/migrations/YYYYMMDD_seed_data_analytics.sql
  ```
  - INSERT curso
  - INSERT módulos
  - INSERT lecciones con contenido markdown

- [ ] #37 Aplicar migración en Supabase
  ```bash
  source .env.local && supabase db push --linked
  ```

- [ ] #38 Verificar datos en Supabase Dashboard

- [ ] #39 Integrar con EduPlatform
  - Copiar `content/` a edu-platform
  - Verificar rutas de API
  - Test de ejercicios

- [ ] #40 Deploy final
  - Push a main
  - Verificar en Vercel
  - Cambiar `is_published: true`

**Tiempo estimado:** 2-4 horas  
**Dependencias:** Todas las fases anteriores

---

## 📌 Notas de Implementación

### Convenciones de Código (OBLIGATORIO)

```python
# Variables estándar
df = pd.read_csv(...)
X = df[features]
y = df[target]
X_train, X_test, y_train, y_test = train_test_split(X, y)
model = LinearRegression()
y_pred = model.predict(X_test)
```

### Formato de Ejercicio YAML

```yaml
id: ex-XX-YY-nombre
type: code-python  # code-python | sql | colab
title: "Título descriptivo"
description: "Qué aprenderá el estudiante"
instructions: |
  Instrucciones claras...

difficulty: beginner  # beginner | intermediate | advanced
estimated_time_minutes: 5
points: 10
runtime_tier: pyodide

starter_code: |
  # Código inicial

solution_code: |
  # Solución completa

test_cases:
  - id: test-1
    name: "Nombre del test"
    test_code: |
      assert condicion, "Mensaje de error"
    points: 10

hints:
  - "Hint 1: Concepto"
  - "Hint 2: Sintaxis"
  - "Hint 3: Casi la solución"

tags:
  - tag1
  - tag2
```

### Embed en Markdown

```markdown
## Ejercicio: Nombre

<!-- exercise:ex-XX-YY-nombre -->

Texto después del ejercicio...
```

---

## 🔄 Flujo de Trabajo

1. **Antes de crear contenido:**
   - Leer `COURSE_STATE.yaml`
   - Verificar `next_module_spec`

2. **Al crear un módulo:**
   - Crear lecciones .md con embeds
   - Crear ejercicios .yaml
   - Probar en EduPlatform local

3. **Al completar un módulo:**
   - Actualizar `exercises_registry` en COURSE_STATE
   - Actualizar `last_module_completed`
   - Escribir nueva `next_module_spec`

4. **Commit message format:**
   ```
   feat(module-XX): add [N] exercises for [topic]
   
   - Lesson: topic-name
   - Exercises: ex-XX-01 to ex-XX-NN
   ```

---

## 📅 Estimación Total

| Fase | Horas Estimadas |
|------|-----------------|
| 1 - Estructura | ✅ 1h |
| 2 - Módulo 1 | 4-6h |
| 3 - Módulos 2-4 | 18-24h |
| 4 - Módulos 5-8 | 16-24h |
| 5 - DB & Deploy | 2-4h |
| **Total** | **41-59h** |

---

*Última actualización: 2025-12-25*
