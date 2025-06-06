# C_Assembler

![Final Grade](https://img.shields.io/badge/grade-95-brightgreen.svg)
![Language](https://img.shields.io/badge/language-C-blue.svg)
## Overview
![Course](https://img.shields.io/badge/course-systems_programming_laboratory-lightgrey.svg)

**C_Assembler** is a two-pass assembler written in C, designed to master bit-field methods, memory management, and modular programming. This project reads assembly code and generates machine code by executing two passes over the input source files.

## Features

- Two-pass assembly process
- Efficient memory management
- Modular design with multiple functions and files
- Comprehensive error checking and reporting

## File Structure

### Main Files

- **assembler.c**: Contains the `main` function and the `executePasses` function that runs the entire project.

### Helper Files

- **assemblerHelper.c / assemblerHelper.h**: Functions for argument checking and loops for the first and second passes.
- **dataStructure.c / dataStructure.h**: Defines the line and label structs, their flags, and initialization functions.
- **reservedWords.c / reservedWords.h**: Functions and arrays for identifying line attributes based on reserved words, such as opcode, number of arguments, and argument types.
- **strHandle.c / strHandle.h**: Parsing functions.
- **firstPass.c / firstPass.h**: Controls the first pass loop and calls relevant functions.
- **secondPassHelper.c / secondPassHelper.h**: Functions for the second pass, called from `assemblerHelper.c`.
- **outputPrint.c / outputPrint.h**: Printing functions for every line type and responsible for creating the output files.

### Auxiliary Files

- **makefile**: Build configuration file.

### Object Files

- **.o files**: Compiled object files for each corresponding source file.

## Getting Started

### Prerequisites

- C Compiler (e.g., `gcc`)

### Building the Project

To build the project, use the provided `makefile`. Run the following command in the terminal:

```sh
make
Running the Assembler
To run the assembler, use the following command:

sh
Copy code
./assembler <source-file>
Replace <source-file> with the path to your assembly source file.

Usage:
Compile the Project: Ensure all source files are compiled by running make.
Run the Assembler:   Execute the assembler with your assembly file as an argument.
Output:              The assembler will generate output files containing the machine code.

- **.o files**: Compiled object files for each corresponding source file.  
  These files are automatically generated during compilation and should not be manually included in the repository.  
  Use `make clean` to remove them when needed.
- To remove object files (.o) and other temporary files, run:
  make clean
```

Contributions are welcome! Please fork the repository and submit pull requests.

The assembler was built as a final project in a laboratory course in system programming in the C language
