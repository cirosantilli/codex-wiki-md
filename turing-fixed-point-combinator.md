# Turing fixed-point combinator

↑ **Parent:** [Fixed-point combinator](fixed-point-combinator.md)

Put $D=\lambda x f.f(xxf)$ and $\Theta=DD$. Then $\Theta f\to_\beta^*f(\Theta f)$. Unlike the [Curry fixed-point combinator](curry-fixed-point-combinator.md), every finite reduct retains a closed subterm $DD$. Contracting this subterm recreates one; every other generated redex substitutes a variable and preserves it. The [Church-Rosser theorem](church-rosser-theorem.md) therefore proves $Y\not\equiv_\beta\Theta$.

## ↑ Ancestors (9)

1. [Fixed-point combinator](fixed-point-combinator.md)
2. [Combinator](combinator.md)
3. [Untyped lambda calculus](untyped-lambda-calculus.md)
4. [Lambda calculus](lambda-calculus.md)
5. [Computability theory](computability-theory.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-76/2/solution.md)
