# Accelera Documentation

<p align="center">
  <img src="accelera.png" alt="Accelera logo" width="180">
</p>

Welcome to **Accelera** - A High-Performance Machine Learning Pipeline Framework that combines the flexibility of Python with the performance of C++.

## Overview

Accelera is a cutting-edge ML pipeline framework designed for building and deploying machine learning workflows with optimized performance. It provides a robust, scalable solution that leverages C++ for compute-intensive operations while maintaining an intuitive Python API.

## Key Features

### Core Pipeline Module
- **Graph-Based Architecture**: Build ML pipelines as directed acyclic graphs
- **Fast Execution**: C++ backend for compute-intensive operations
- **Flexible Design**: Chain preprocessing, models, and metrics easily
- **Branch Support**: Create parallel pipeline paths for experimentation

### Code Parallelizer
- **Loop Extraction**: Extract loops from C/C++ code using AST analysis
- **Parallelization Detection**: Flag parallelizable loops using trained ML models
- **OpenMP Integration**: Automatically parallelize loops using OpenMP directives
- **Performance Optimization**: Transform sequential code into parallel execution
- **Linux Support**: Full support on Linux systems

### AutoML Module
- **Classification and Regression Search**: Search model candidates under time and trial budgets
- **Hyperparameter Optimization**: Tune model configurations automatically
- **Meta-Learning Warm Starts**: Use dataset meta-features to initialize searches
- **Ensembles**: Build voting and stacked ensembles from strong candidates

### Deployment Module
- **Model Registry**: Track model snapshots and active deployments
- **Schema Validation**: Validate request payloads before prediction
- **Prediction Service**: Serve model artifacts through an API
- **Deployment Targets**: Build and run locally with Docker, Heroku, or AWS EC2

### Benchmark Platform
- **Benchmark Management**: Create and organize benchmark definitions
- **Metrics and Submissions**: Define metrics and submit model results
- **Leaderboard**: Track performance across different approaches
- **Web Dashboard**: React frontend with user, admin, benchmark, and metric screens

## Quick Links

- [Installation Guide](installation.md) - Get started with Accelera
- [Core Pipeline](core-pipeline.md) - Graph-based ML pipelines
- [Code Parallelizer](code-parallelizer.md) - Loop extraction features
- [AutoML](automl.md) - Classification and regression model search
- [Deployment](deployment.md) - Model serving and deployment workflows
- [Benchmark Platform](benchmark.md) - Benchmark web application
- [Examples](examples.md) - Sample projects and tutorials
- [Contributing](contributing.md) - Help improve Accelera

## Platform Support

| Platform | Core Features | Code Parallelizer | Full Support |
|----------|--------------|-------------------|--------------|
| Linux    | Supported | Supported | Full |
| Windows  | Supported | Not Available | Partial |
| macOS    | Supported | Not Available | Partial |

## Requirements

- **Python**: 3.9 or higher
- **CMake**: 3.14 or higher
- **C++ Compiler**: C++20 support required
- **LLVM/Clang 14+**: Required for code parallelizer (Linux only)

## Community

- **GitHub**: [Mohamed-Ashraf273/accelera](https://github.com/Mohamed-Ashraf273/accelera)
- **Issues**: [Report bugs or request features](https://github.com/Mohamed-Ashraf273/accelera/issues)
- **License**: Apache 2.0

## Getting Help

If you encounter any issues or have questions:

1. Check module documentation ([Core Pipeline](core-pipeline.md), [Code Parallelizer](code-parallelizer.md))
2. Look at [Examples](examples.md) for usage patterns
3. Open an issue on GitHub if you find a bug
