#Code Analyser (Python)
A Python-based static analysis tool that examines Python files to detect errors, inconsistencies, and encoding issues (such as UTF-8 incompatibilities).

#Overview
This program allows users to analyze a Python file through command-line arguments and apply different types of checks, including line-based analysis and Abstract Syntax Tree (AST) analysis.

##Features
 - Analyze a Python file provided via command-line arguments (argparse)

Perform: 
 - Line-based checks
 - AST-based checks
 - Combined analysis
 - Detect syntax issues and potential inconsistencies
 - Identify encoding-related problems (e.g. UTF-8 compatibility)

Project Structure
 - main.py – Entry point of the program
 - line_checks.py – Contains line-by-line validation functions
 - ast_checks.py – Basic AST-based analysis
 - advanced_ast_checks.py – More advanced AST validations
 - decorators.py – Shared decorators used across check functions

Technical Details
 - Modular design with separated concerns for different types of analysis
 - Use of decorators to standardize and enhance function behavior
 - Built using Python’s AST module for deeper code inspection

Requirements
All required libraries are part of Python’s standard library (no external dependencies needed).

How to Run
python main.py <filename> --checks [line|ast|all]
Example:
python main.py script.py --checks all

Notes
This project was developed to explore static code analysis, modular design, and working with Python’s AST for deeper program inspection.
