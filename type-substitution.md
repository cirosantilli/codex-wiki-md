# Type substitution

↑ **Parent:** [Type variable](type-variable.md)

A [type substitution](type-substitution.md) replaces [type variables](type-variable.md) by type expressions consistently. For example, $S=\{\alpha\mapsto\mathrm{int}\}$ gives $S(\alpha\to\alpha)=\mathrm{int}\to\mathrm{int}$. Applying a [type substitution](type-substitution.md) to a [type scheme](type-scheme.md) must respect its bound [type variables](type-variable.md); separate instantiation first replaces those bound placeholders by fresh ones.

## ↑ Ancestors (5)

1. [Type variable](type-variable.md)
2. [Type system](type-system.md)
3. [Programming language](programming-language.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Algorithm W](algorithm-w.md)
- [Occurs check](occurs-check.md)
- [Type substitution](type-substitution.md)
- [Type unification](type-unification.md)
- [Type variable](type-variable.md)
