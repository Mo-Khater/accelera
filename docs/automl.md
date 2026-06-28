# AutoML Module

The Accelera AutoML module provides classification and regression model search,
evaluation, warm-start metadata, optimizer integration, and ensemble utilities.
It lives under `accelera/src/accelera_automl/`.

## Overview

Accelera AutoML is designed to automate practical model selection workflows. It
searches candidate estimators, evaluates them under configurable budgets, stores
benchmark results, and can combine strong candidates through voting or stacked
ensembles.

## Key Components

- **Core orchestration**: `accelera/src/accelera_automl/core/automl.py`
- **Classification tasks**: `classification.py` and
  `components/classification.py`
- **Regression tasks**: `regression.py` and `components/regression.py`
- **Optimization**: `optimization/smac_optimizer.py`
- **Meta-learning warm starts**: `meta_learning/warmstart.py`,
  `meta_learning/metafeatures.py`, and bundled JSON metadata
- **Evaluation utilities**: `evaluation.py` and `base_evaluation.py`
- **Ensembles**: `stacked_ensemble.py` and `stacked_ensemble_regression.py`
- **AutoML benchmark integration**:
  `automlbenchmark_custom_myautoml/`

## Capabilities

- Run classification and regression searches.
- Configure time budgets and trial counts.
- Evaluate candidate pipelines with common metrics.
- Warm-start search from dataset meta-features.
- Build voting and stacked ensemble models.
- Reproduce benchmark experiments from included benchmark configuration files.

## Example Commands

```bash
python examples/run_classification_task_automl.py
python examples/run_regression_task_automl.py --time-budget 300 --n-trials 10
```

## Benchmark Assets

The repository includes benchmark configuration and result artifacts:

- `accelera/src/accelera_automl/automlbenchmark_custom_myautoml/`
- `docs/accelera_automl_benchmark_results/`
- `data/accelera_automl/`

These files support reproducible classification and regression comparisons
against common AutoML frameworks.

## Related Modules

- [Core Pipeline](core-pipeline.md) - Graph pipeline execution.
- [Auto Preprocessing examples](examples.md) - Dataset preparation workflows.
- [Deployment Module](deployment.md) - Package selected models as services.
- [Benchmark Platform](benchmark.md) - Web platform for comparing results.
