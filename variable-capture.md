# Variable capture

↑ **Parent:** [Capture-avoiding substitution](capture-avoiding-substitution.md)

An unintended change of binding caused by moving or substituting a term beneath a binder. In [first-order logic](first-order-logic.md), substituting $y$ for the free $x$ in $\forall y\,S(x,y)$ without renaming would yield $\forall y\,S(y,y)$, incorrectly binding the substituted occurrence. First rename the bound $y$ to a fresh $z$, obtaining $\forall z\,S(x,z)$, and then substitute to get $\forall z\,S(y,z)$. The paper's condition that a term be free for a variable excludes such capture.

## ↑ Ancestors (9)

1. [Capture-avoiding substitution](capture-avoiding-substitution.md)
2. [Beta reduction](beta-reduction.md)
3. [Untyped lambda calculus](untyped-lambda-calculus.md)
4. [Lambda calculus](lambda-calculus.md)
5. [Computability theory](computability-theory-split.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/lambda-calculus-and-types/3/b/solution.md)
- [Solution](past-exam-of-the-logic-and-set-theory-course-of-the-university-of-oxford/2011/a/3/b/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/digital-systems-linear-algebra-introduction-to-formal-proof/8/a/i/solution.md)
