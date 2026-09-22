# Abstract syntax tree source location

↑ **Parent:** [Abstract syntax tree](abstract-syntax-tree.md)

An [abstract syntax tree](abstract-syntax-tree.md) can retain source locations even while omitting punctuation nodes. [Python](python-programming-language.md) records one-based line numbers and zero-based UTF-8 byte offsets, with the end offset exclusive. In `x=2+3*4`, the [multiplication](multiplication.md) node spans offsets $4$ through $7$, and `ast.get_source_segment` returns `3*4`. A copied location on a folded `12` describes the original span, not text newly present in the source. Such metadata supports error messages and editing tools without making an [abstract syntax tree](abstract-syntax-tree.md) a lossless record of formatting. [Node classes: lineno, col\_offset, end\_lineno and end\_col\_offset; get\_source\_segment and copy\_location](python-3-14-documentation/ast-abstract-syntax-trees-python-3-14-documentation.md)

// Target: computer-science.bigb

## ↑ Ancestors (4)

1. [Abstract syntax tree](abstract-syntax-tree.md)
2. [Programming language](programming-language.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)
