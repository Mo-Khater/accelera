# Code Parallelizer

The Code Parallelizer is a powerful feature that analyzes C/C++ source code to extract loop structures using Clang's Abstract Syntax Tree (AST).

!!! warning "Platform Availability"
    The Code Parallelizer is currently **Linux-only**. It requires LLVM/Clang 14+ development libraries.

## Overview

The Code Parallelizer uses Clang's AST infrastructure to:

- **Parse C/C++ source code** without executing it
- **Identify loop structures** (for, while, do-while loops)
- **Extract loop metadata** (type, line numbers, source code)
- **Export to JSON** for further analysis
- **Identify parallelizable loops** using trained ML models
- **Parallelize code** automatically based on model predictions

## Current Status

The Code Parallelizer is fully functional and available for use. Core features are implemented and tested. Comprehensive documentation with detailed API references, tutorials, and advanced examples is being prepared.

## Generator Evaluation Report

The current OpenMP generator report is available here:

[OpenMP Generator Evaluation Report](current-generator-report.md)

It explains how the generator works, how Python inputs are converted to C++,
how generated pragmas are validated, and how the latest classifier, pragma
accuracy, compile/run, and latency metrics are measured.

## Implementation

The implementation is available in `accelera/src/parallelizer/` and supporting
C++ AST utilities under `src/ast/`. The repository also includes tests,
evaluation data, generated parallelized files, and an OpenMP generator report.

## How You Can Help

We welcome contributions! Areas where you can help:

1. **Documentation**: Write tutorials and usage examples
2. **Testing**: Test on various C/C++ codebases and report issues
3. **Model Training**: Contribute to parallelization prediction models
4. **Feature Requests**: Suggest improvements and new features
5. **Bug Reports**: Help identify and fix issues

See [Contributing](contributing.md) for more details.

## Related Modules

- [Core Pipeline](core-pipeline.md) - The underlying pipeline framework
- [Examples](examples.md) - Code examples and tutorials
- [Installation](installation.md) - Setup and installation guide

## Questions?

If you have questions or suggestions about the Code Parallelizer:

1. Open an issue on [GitHub](https://github.com/Mohamed-Ashraf273/accelera/issues)
2. Check existing examples in the `examples/` directory

