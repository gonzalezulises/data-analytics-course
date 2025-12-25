# GitHub Issues para Data Analytics Course

Para importar estos issues, puedes usar GitHub CLI o crearlos manualmente.

## Usando GitHub CLI (después de crear el repo)

```bash
# Autenticar
gh auth login

# Crear issues desde este archivo
gh issue create --title "..." --body "..." --label "..."
```

---

## Issues por Fase

### Fase 1: Estructura Base ✅ (ya completada en el commit inicial)

### Fase 2: Módulo 1 - Python (Label: `module-01`, `content`)

```bash
gh issue create \
  --title "[M01] Crear lesson 01-primeros-pasos.md" \
  --body "Crear lección con:
- Introducción a Python y por qué aprenderlo
- print() y comentarios
- Primera ejecución
- Embeds: ex-01-01-hello-world, ex-01-02-variables

**Archivo:** content/courses/data-analytics/module-01/lessons/01-primeros-pasos.md" \
  --label "module-01,content,lesson"

gh issue create \
  --title "[M01] Crear lesson 02-tipos-datos.md" \
  --body "Crear lección con:
- int, float, str, bool
- Operadores aritméticos
- Conversión de tipos
- Embeds: ex-01-03, ex-01-04, ex-01-05

**Archivo:** content/courses/data-analytics/module-01/lessons/02-tipos-datos.md" \
  --label "module-01,content,lesson"

gh issue create \
  --title "[M01] Crear lesson 03-colecciones.md" \
  --body "Crear lección con:
- Listas: crear, acceder, modificar
- Diccionarios: crear, acceder
- Métodos comunes
- Embeds: ex-01-06, ex-01-07, ex-01-08

**Archivo:** content/courses/data-analytics/module-01/lessons/03-colecciones.md" \
  --label "module-01,content,lesson"

gh issue create \
  --title "[M01] Crear lesson 04-control-flujo.md" \
  --body "Crear lección con:
- if/elif/else
- for loops
- while loops
- break y continue
- Embeds: ex-01-09, ex-01-10, ex-01-11

**Archivo:** content/courses/data-analytics/module-01/lessons/04-control-flujo.md" \
  --label "module-01,content,lesson"

gh issue create \
  --title "[M01] Crear lesson 05-funciones.md" \
  --body "Crear lección con:
- def y return
- Parámetros y argumentos
- Valores por defecto
- Embed: ex-01-12

**Archivo:** content/courses/data-analytics/module-01/lessons/05-funciones.md" \
  --label "module-01,content,lesson"

gh issue create \
  --title "[M01] Crear ejercicios ex-01-01 a ex-01-06" \
  --body "Crear ejercicios YAML:
- ex-01-01-hello-world: print()
- ex-01-02-variables: crear variables
- ex-01-03-tipos-datos: identificar tipos
- ex-01-04-operaciones: aritmética
- ex-01-05-strings: manipulación de texto
- ex-01-06-listas-crear: crear listas

**Directorio:** content/courses/data-analytics/module-01/exercises/" \
  --label "module-01,content,exercise"

gh issue create \
  --title "[M01] Crear ejercicios ex-01-07 a ex-01-12" \
  --body "Crear ejercicios YAML:
- ex-01-07-listas-acceso: indexing
- ex-01-08-diccionarios: crear y acceder
- ex-01-09-if-else: condicionales
- ex-01-10-for-loop: iterar listas
- ex-01-11-while-loop: bucles condicionales
- ex-01-12-funciones: definir funciones

**Directorio:** content/courses/data-analytics/module-01/exercises/" \
  --label "module-01,content,exercise"
```

### Fase 3: Módulos 2-4 (Labels: `module-02`, `module-03`, `module-04`)

```bash
# Módulo 2: Pandas
gh issue create \
  --title "[M02] Migrar datasets drinks.csv y movies.csv" \
  --body "Mover datasets a content/shared/datasets/:
- drinks.csv (fivethirtyeight)
- movies.csv (u.user de MovieLens)

Verificar columnas y documentar en README." \
  --label "module-02,data"

gh issue create \
  --title "[M02] Crear 4 lecciones de Pandas" \
  --body "Lecciones:
1. 01-intro-pandas.md
2. 02-dataframes.md
3. 03-seleccion.md
4. 04-fuentes-datos.md

Total: 10 ejercicios embebidos" \
  --label "module-02,content,lesson"

gh issue create \
  --title "[M02] Crear 10 ejercicios de Pandas" \
  --body "Ejercicios ex-02-01 a ex-02-10:
- import pandas
- read_csv
- explorar df
- head/tail
- shape/dtypes
- selección columnas
- iloc/loc
- filtrado básico
- read_excel
- crear dataframe" \
  --label "module-02,content,exercise"

# Módulo 3: EDA
gh issue create \
  --title "[M03] Migrar datasets ufo.csv y titanic.csv" \
  --body "Mover datasets a content/shared/datasets/:
- ufo.csv
- titanic.csv

Verificar y limpiar si es necesario." \
  --label "module-03,data"

gh issue create \
  --title "[M03] Crear 4 lecciones de EDA" \
  --body "Lecciones:
1. 01-estadisticas-descriptivas.md
2. 02-agrupacion.md
3. 03-datos-faltantes.md
4. 04-combinacion.md

Total: 12 ejercicios embebidos" \
  --label "module-03,content,lesson"

gh issue create \
  --title "[M03] Crear 12 ejercicios de EDA" \
  --body "Ejercicios ex-03-01 a ex-03-12:
- describe
- value_counts
- unique/nunique
- groupby simple
- groupby + agg
- pivot_table
- isna/sum
- fillna
- dropna
- merge
- concat
- filtrado avanzado" \
  --label "module-03,content,exercise"

# Módulo 4: Visualización
gh issue create \
  --title "[M04] Configurar datasets de visualización" \
  --body "Datasets:
- tips.csv (puede usar seaborn.load_dataset)
- iris.csv (puede usar sklearn)

Decidir si copiar localmente o usar builtins." \
  --label "module-04,data"

gh issue create \
  --title "[M04] Crear 4 lecciones de Visualización" \
  --body "Lecciones:
1. 01-matplotlib-basico.md
2. 02-histogramas-boxplots.md
3. 03-seaborn.md
4. 04-plotly-interactivo.md

Total: 10 ejercicios embebidos" \
  --label "module-04,content,lesson"

gh issue create \
  --title "[M04] Crear 10 ejercicios de Visualización" \
  --body "Ejercicios ex-04-01 a ex-04-10:
- plot línea
- scatter
- bar chart
- histograma
- boxplot
- seaborn scatter
- heatmap
- plotly scatter
- plotly bar
- subplots" \
  --label "module-04,content,exercise"
```

### Fase 4: Módulos 5-8 (Labels: `module-05` a `module-08`)

```bash
# Módulo 5: Regresión
gh issue create \
  --title "[M05] Migrar dataset bikeshare.csv" \
  --body "Dataset para regresión:
- bikeshare.csv (Kaggle Bike Sharing)

Target: count
Features: season, weather, temp, humidity, etc." \
  --label "module-05,data"

gh issue create \
  --title "[M05] Crear 4 lecciones de Regresión" \
  --body "Lecciones:
1. 01-intro-ml.md
2. 02-regresion-lineal.md
3. 03-evaluacion-modelos.md
4. 04-practica-bikeshare.md (link Colab)

Total: 6 ejercicios + 1 Colab" \
  --label "module-05,content,lesson"

gh issue create \
  --title "[M05] Crear 6 ejercicios + Colab notebook" \
  --body "Ejercicios:
- train_test_split
- LinearRegression
- fit/predict
- MSE/RMSE
- R² score
- cross_validation

Notebook Colab: Práctica completa Bikeshare" \
  --label "module-05,content,exercise"

# Módulo 6: Clasificación
gh issue create \
  --title "[M06] Crear 4 lecciones de Clasificación" \
  --body "Lecciones:
1. 01-regresion-logistica.md
2. 02-matriz-confusion.md
3. 03-arboles-decision.md
4. 04-practica-titanic.md (link Colab)

Dataset: titanic.csv (ya migrado en M03)
Total: 6 ejercicios + 1 Colab" \
  --label "module-06,content,lesson"

gh issue create \
  --title "[M06] Crear 6 ejercicios + Colab notebook" \
  --body "Ejercicios:
- LogisticRegression
- predict_proba
- confusion_matrix
- precision/recall
- DecisionTree
- ROC/AUC

Notebook Colab: Supervivencia Titanic" \
  --label "module-06,content,exercise"

# Módulo 7: Clustering
gh issue create \
  --title "[M07] Crear dataset sintético customers.csv" \
  --body "Generar dataset para segmentación:
- ~200 filas
- Features: Annual Income, Spending Score, Age
- Sin target (unsupervised)

Usar para ejercicios de clustering." \
  --label "module-07,data"

gh issue create \
  --title "[M07] Crear 4 lecciones de Clustering" \
  --body "Lecciones:
1. 01-intro-clustering.md
2. 02-kmeans.md
3. 03-dbscan.md
4. 04-practica-segmentacion.md (link Colab)

Total: 5 ejercicios + 1 Colab" \
  --label "module-07,content,lesson"

gh issue create \
  --title "[M07] Crear 5 ejercicios + Colab notebook" \
  --body "Ejercicios:
- KMeans básico
- Elbow method
- Silhouette score
- DBSCAN
- Comparar algoritmos

Notebook Colab: Segmentación de clientes" \
  --label "module-07,content,exercise"

# Módulo 8: Dashboards
gh issue create \
  --title "[M08] Crear 4 lecciones de Dashboards" \
  --body "NOTA: Reemplaza Tableau con Plotly/Streamlit

Lecciones:
1. 01-plotly-avanzado.md (Graph Objects)
2. 02-graficos-combinados.md
3. 03-streamlit-intro.md
4. 04-dashboard-completo.md

Total: 8 ejercicios" \
  --label "module-08,content,lesson"

gh issue create \
  --title "[M08] Crear 8 ejercicios de Dashboards" \
  --body "Ejercicios:
- graph_objects básico
- layout/styling
- subplots avanzados
- dual axis
- streamlit básico
- widgets
- dashboard layout
- interactividad

Todo ejecutable en browser (Pyodide/Streamlit)." \
  --label "module-08,content,exercise"
```

### Fase 5: Database & Deploy (Label: `infrastructure`)

```bash
gh issue create \
  --title "[DB] Crear migración SQL para Supabase" \
  --body "Crear archivo:
supabase/migrations/YYYYMMDD_seed_data_analytics.sql

Incluir:
- INSERT curso
- INSERT módulos
- INSERT lecciones con markdown

Usar estructura de edu-platform." \
  --label "infrastructure,database"

gh issue create \
  --title "[DB] Aplicar migración en Supabase" \
  --body "Ejecutar:
\`\`\`bash
source .env.local && supabase db push --linked
\`\`\`

Verificar datos en Supabase Dashboard." \
  --label "infrastructure,database"

gh issue create \
  --title "[Deploy] Integrar con EduPlatform" \
  --body "Pasos:
1. Copiar content/ a edu-platform
2. Verificar rutas de API
3. Test de ejercicios en local
4. Verificar renderizado de markdown
5. Test de ejecución Pyodide" \
  --label "infrastructure,integration"

gh issue create \
  --title "[Deploy] Deploy final" \
  --body "Pasos:
1. Push a main
2. Verificar en Vercel
3. Cambiar is_published: true en course.yaml
4. Smoke test de todos los módulos" \
  --label "infrastructure,deploy"
```

---

## Labels sugeridos para crear

```bash
gh label create "module-01" --color "1d76db" --description "Módulo 1: Python"
gh label create "module-02" --color "1d76db" --description "Módulo 2: Pandas"
gh label create "module-03" --color "1d76db" --description "Módulo 3: EDA"
gh label create "module-04" --color "1d76db" --description "Módulo 4: Visualización"
gh label create "module-05" --color "1d76db" --description "Módulo 5: Regresión"
gh label create "module-06" --color "1d76db" --description "Módulo 6: Clasificación"
gh label create "module-07" --color "1d76db" --description "Módulo 7: Clustering"
gh label create "module-08" --color "1d76db" --description "Módulo 8: Dashboards"
gh label create "content" --color "0e8a16" --description "Contenido educativo"
gh label create "lesson" --color "c5def5" --description "Lección markdown"
gh label create "exercise" --color "bfd4f2" --description "Ejercicio YAML"
gh label create "data" --color "fbca04" --description "Datasets"
gh label create "infrastructure" --color "d93f0b" --description "Infra/DB/Deploy"
gh label create "database" --color "e99695" --description "Supabase/SQL"
gh label create "integration" --color "f9d0c4" --description "Integración EduPlatform"
gh label create "deploy" --color "b60205" --description "Deploy a producción"
```

---

## Milestones

```bash
gh api repos/{owner}/{repo}/milestones -f title="Fase 2: Módulo 1 Python" -f due_on="2025-01-15T00:00:00Z" -f description="5 lecciones + 12 ejercicios"
gh api repos/{owner}/{repo}/milestones -f title="Fase 3: Módulos 2-4" -f due_on="2025-02-15T00:00:00Z" -f description="12 lecciones + 32 ejercicios"
gh api repos/{owner}/{repo}/milestones -f title="Fase 4: Módulos 5-8" -f due_on="2025-03-15T00:00:00Z" -f description="16 lecciones + 25 ejercicios + 4 Colab"
gh api repos/{owner}/{repo}/milestones -f title="Fase 5: Deploy" -f due_on="2025-03-31T00:00:00Z" -f description="DB + Deploy"
```
