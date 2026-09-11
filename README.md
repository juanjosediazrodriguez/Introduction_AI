# Introduction_AI

Notebooks de la materia **SI3003 - Artificial Intelligence** (Universidad EAFIT). El curso sigue la tradición de agentes racionales (línea Berkeley CS188 / Stanford CS221) con un balance 50/50 entre fundamentos clásicos de IA y IA moderna. En este repo se sube el notebook trabajado en cada lecture.

## Progreso

- **Lecture 2 — Search algorithms**: formulación de problemas de búsqueda en espacio de estados, estrategias no informadas (DFS, BFS, UCS, profundización iterativa) e informadas (greedy, A*), heurísticas admisibles y consistentes, búsqueda en grafo.
- **Lecture 3 — Optimization**

## Estructura

Un directorio por lecture, con el o los notebooks trabajados en esa sesión:

```
lecture-2-search/
lecture-3-optimization/
lecture-4-markov/
lecture-5-reinforcement/
lecture-6-ml/
```

`lecture-6-ml/` tiene estructura propia, porque sus notebooks encadenan artefactos entre sí. Los notebooks resuelven las rutas con `Path.cwd()`, así que el kernel debe arrancar desde `challenge/`:

```
lecture-6-ml/challenge/
├── 01_data_challenge.ipynb                    → data/processed/, artifacts/data_contract.json
├── 02_training_challenge.ipynb                → artifacts/champion_model.joblib, reports/cv_results.csv
├── 03_evaluation_deployment_challenge.ipynb   → reports/test_metrics.json, reports/batch_predictions.csv
├── data/
│   ├── raw/wine.csv          dataset original
│   └── processed/            train.csv y test.csv (split estratificado 142/36)
├── artifacts/                contrato de datos, modelo campeón y metadatos de entrenamiento
└── reports/                  resultados de validación cruzada, métricas de test y predicciones por lote
```

## Referencias

- Sitio del curso: https://eafit-ia.github.io/si3003-artificial-intelligence/

## Declaracion de uso de IA 

se hizo uso de IA para fines de explicacion de codigo y apoyo corrigiendo segmentos de codigo, no se genero codigo o material directamente por IA sin por lo menos una primera version humana  

## Integrantes

- Juan Jose Diaz
- Jhesid Steven Suarez Berrio
- Felipe Martinez Cortes
- Alejandro Jaramillo Rodriguez
