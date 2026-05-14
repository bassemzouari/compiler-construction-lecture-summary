# Compiler Construction Lecture Summary

Comprehensive LaTeX-based lecture summary for a university-level
Compiler Construction / Programming Languages course covering
syntax analysis, parsing algorithms, compiler architecture,
and runtime systems.

The project focuses on structured technical documentation,
formal language theory, and concise explanations of compiler
design concepts, parsing strategies, and execution models.

---

## Topics Covered

- Compilation Process & Phases
- One-Pass vs Multi-Pass Compilers
- Lexical Analysis & Tokenization
- Syntax Analysis (Parsing)
- Abstract Syntax Trees (AST)
- Context-Free Grammars (CFG)
- Extended Backus-Naur Form (EBNF)
- Grammar Transformations
- Left Recursion Elimination
- Top-Down Parsing (Recursive Descent)
- Bottom-Up Parsing (Shift-Reduce)
- LL(k) vs LR(k) Parsing
- Parser Construction Techniques
- Runtime Systems & Memory Management
- Stack vs Register Machines
- Triangle Abstract Machine (TAM)

---

## Build Instructions

Requirements:
- A LaTeX installation (e.g. MikTeX or TeX Live)
- Installation of the [TU Template](https://github.com/tudace/tuda_latex_templates) and the required plugins
- Installation of Pygments (for code blocks), e.g. via `pip install Pygments`

First, the folder structure must of course be downloaded, for example using `git clone`.  
Afterwards, the summary/document must be compiled with the `--shell-escape` flag.  

If you are using VS Code with LaTeX Workshop, you can modify the `settings.json` by appending the following:

```jsonc
"latex-workshop.latex.tools": [
    {
        "name": "latexmk",
        "command": "latexmk",
        "args": [
            "--shell-escape",
            "-synctex=1",
            "-interaction=nonstopmode",
            "-file-line-error",
            "-lualatex",
            "-outdir=%OUTDIR%",
            "%DOC%"
        ]
    },
],
```

---

## Preview

The compiled PDF can be found in:

```text
output/summary.pdf
```

---

## Goals of the Project

- Create a structured and maintainable compiler reference
- Summarize theoretical foundations of programming languages
- Provide clear explanations of parsing and compilation techniques
- Bridge theory and practical compiler implementation concepts
- Improve technical documentation and LaTeX workflow skills

---

## Disclaimer

This document was independently written for educational purposes.
It is intended as a personal lecture summary and study reference.

Some topics may be based on university lecture material and publicly
known concepts in compiler construction and formal language theory.
All rights to original course content remain with their respective owners.

---

## License

This repository is licensed under the MIT License.
