# Private-witness diagonalization for incomparable enumerable sets

↑ **Parent:** [Finite-injury priority construction](finite-injury-priority-construction.md)

To prevent a [Turing functional](turing-functional.md) $\Phi_e^B$ from computing the [indicator function](indicator-function.md) of an enumerated [set](set-split.md) $A$, reserve a permanently unique fresh witness $x$. On observing a convergent computation with [oracle use](oracle-use.md) $u$, enumerate $x$ into $A$ if the answer is zero; otherwise keep it out. Restrain subsequent lower-priority enumerations into $B$ below $u$. Higher-priority actions may initialize this strategy and retire its witness, but witnesses are never reused. In a [finite-injury priority construction](finite-injury-priority-construction.md), [mathematical induction](mathematical-induction.md) on priority shows that the final computation, if observed, remains correct as a computation from the final oracle and disagrees with $A$ at $x$. If no computation is ever observed after the final initialization, the final oracle computation diverges, since any convergent computation uses only finitely many eventually stable oracle bits.

## ↑ Ancestors (6)

1. [Finite-injury priority construction](finite-injury-priority-construction.md)
2. [Computability theory](computability-theory.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135/2/solution.md)
