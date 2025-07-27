# C-Assembler

A two-pass assembler with macro support, implemented in C.

---

## Overview

This project implements an assembler for a simplified assembly language.  
The assembler uses a two-pass architecture and handles macro expansion, symbol management, and error reporting.

---

## Features

- **Two-Pass Assembler:**
  - First pass: macro expansion, label detection, symbol table construction.
  - Second pass: address resolution, symbol linking, memory image generation.

- **Macro Support:**
  - Supports custom macro definitions (`macr ... endmacr`).

- **Symbol Table Management:**
  - Handles local labels, `.entry` and `.extern` directives.
  - Generates external and entry symbol files.

- **Full Error Detection:**
  - Syntax errors.
  - Undefined labels.
  - Invalid operands.
  - Invalid macro definitions.
  - Illegal symbol names.

- **Output Files:**
  - `.am` - expanded source after macro processing.
  - `.ob` - object file (machine code representation).
  - `.ent` - entry symbols.
  - `.ext` - external symbols.
