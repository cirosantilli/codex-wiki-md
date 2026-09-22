# Lambda definition of primitive recursion

↑ **Parent:** [Lambda-definable function](lambda-definable-function.md)

Using a [fixed-point combinator](fixed-point-combinator.md), Church Boolean conditionals, a zero test, and a predecessor term, lambda-definable $g$ and $h$ give

$$
R\mathbf x0=g(\mathbf x),
\qquad
R\mathbf x(n+1)=h(\mathbf x,n,R\mathbf x n).
$$

Normal-order beta reduction evaluates only the selected conditional branch, so this term implements primitive recursion on [Church numerals](church-numeral.md).

**Table of contents**

- [Lambda definition of primitive recursion by pair iteration](lambda-definition-of-primitive-recursion-by-pair-iteration.md)

## ↑ Ancestors (9)

1. [Lambda-definable function](lambda-definable-function.md)
2. [Church numeral](church-numeral.md)
3. [Church encoding](church-encoding.md)
4. [Lambda calculus](lambda-calculus.md)
5. [Computability theory](computability-theory.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-135/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-120/3/solution.md)
- [Strict sequencing of partial numeral computations](strict-sequencing-of-partial-numeral-computations.md)
