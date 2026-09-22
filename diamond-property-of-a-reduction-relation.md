# Diamond property of a reduction relation

↑ **Parent:** [Beta reduction](beta-reduction.md)

A reduction relation $\to$ has the diamond property if $a\to b$ and $a\to c$ imply a common one-step successor $b\to d\leftarrow c$. For relations allowing an identity step, the same definition includes zero-length joins. A finite grid of these diamonds proves confluence of $\to^*$. Ordinary one-step [beta reduction](beta-reduction.md) fails this property because contracting before duplication can save two separate contractions.

**Table of contents**

- [Church-Rosser property of a reduction relation](church-rosser-property-of-a-reduction-relation.md)

## ↑ Ancestors (8)

1. [Beta reduction](beta-reduction.md)
2. [Untyped lambda calculus](untyped-lambda-calculus.md)
3. [Lambda calculus](lambda-calculus.md)
4. [Computability theory](computability-theory.md)
5. [Foundations of mathematics](foundations-of-mathematics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
