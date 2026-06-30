# Code Analyser

A static analysis tool for Python files built with Python's `ast` module. Accepts a file path via command-line arguments and runs configurable checks to detect syntax issues, encoding problems, and code inconsistencies.

## Features

- Line-by-line validation (whitespace issues, encoding problems, UTF-8 incompatibilities)
- AST-based analysis for deeper structural inspection
- Advanced AST checks for additional code quality rules
- Shared decorator system for consistent check behavior
- Modular design — each check type lives in its own module
- No external dependencies

## Project Structure
├── codeanalyser.py        # Entry point, argument parsing
├── line_checks.py         # Line-based validation functions
├── atc_checks.py          # Basic AST checks
├── advanced_ast_checks.py # Advanced AST validations
└── decorators.py          # Shared decorators

## How to Run

```bash
python codeanalyser.py script.py --checks line
python codeanalyser.py script.py --checks ast
python codeanalyser.py script.py --checks all
```

## Concepts Demonstrated

- Python's `ast` module for code inspection
- Modular architecture with separated concerns
- Decorator pattern for reusable function behavior
- Command-line argument parsing with `argparse`
- Static analysis fundamentals
