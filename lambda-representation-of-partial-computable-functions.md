# Lambda representation of partial computable functions

↑ **Parent:** [Lambda-definable partial function](lambda-definable-partial-function.md)

Every [partial computable function](computable-function.md) is represented on [Church numerals](church-numeral.md) by a closed [untyped lambda calculus](untyped-lambda-calculus.md) term. First represent all [primitive recursive functions](primitive-recursive-function.md) using zero, successor, projections, composition and [lambda definition of primitive recursion by pair iteration](lambda-definition-of-primitive-recursion-by-pair-iteration.md). Apply the [Kleene normal form theorem](kleene-normal-form-theorem.md) and search successive history codes with a [fixed-point combinator](fixed-point-combinator.md). Test the represented total predicate using a [Church numeral zero test](church-numeral-zero-test.md); return the decoded output only on the true branch. If no history passes, normal-order head reduction continues the search indefinitely and the term has no [head normal form](head-normal-form.md), so cannot be in [beta equivalence](beta-equivalence.md) with a [Church numeral](church-numeral.md). This avoids the incorrect assumption that a lazy outer [function](function-split.md) must evaluate a divergent argument in an unguarded composition.

**Table of contents**

- [Lambda simulation of a Turing machine](lambda-simulation-of-a-turing-machine.md)

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

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-20/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135/6/solution.md)
