# Strict sequencing of partial numeral computations

↑ **Parent:** [Lambda-definable partial function](lambda-definable-partial-function.md)

The term $\mathrm{Force}\,c_m\,K$ beta-reduces to $K$ for every [Church numeral](church-numeral.md) $c_m$. If its first argument has no [head normal form](head-normal-form.md), the whole application has no head normal form. Nesting this operation forces each represented inner computation before applying an outer function, implementing [composition of partial functions](composition-of-partial-functions.md) even when an outer projection would discard an argument. The same guard makes [lambda definition of primitive recursion](lambda-definition-of-primitive-recursion.md) strict in the preceding recursive value.

## ↑ Ancestors (10)

1. [Lambda-definable partial function](lambda-definable-partial-function.md)
2. [Lambda-definable function](lambda-definable-function.md)
3. [Church numeral](church-numeral.md)
4. [Church encoding](church-encoding.md)
5. [Lambda calculus](lambda-calculus.md)
6. [Computability theory](computability-theory.md)
7. [Foundations of mathematics](foundations-of-mathematics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)
