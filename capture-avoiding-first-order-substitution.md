# Capture-avoiding first-order substitution

↑ **Parent:** [First-order logic](first-order-logic.md)

To perform a [first-order substitution](first-order-substitution.md), first rename each conflicting [bound variable](bound-variable.md) to a fresh name, then replace the designated free occurrences. The fresh names must avoid the formula's relevant free names and all names in the inserted [first-order term](first-order-term.md). For instance, substituting $f(u,t)$ for $z$ in $\exists t\,Q(z,t)$ requires renaming the binder, producing $\exists s\,Q(f(u,t),s)$ rather than $\exists t\,Q(f(u,t),t)$. The latter would change the intended meaning by capturing $t$.

## ↑ Ancestors (6)

1. [First-order logic](first-order-logic.md)
2. [Mathematical logic](mathematical-logic-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [First-order substitution](first-order-substitution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof-resit/8/d/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/digital-systems-linear-algebra-introduction-to-formal-proof/8/f/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/digital-systems-linear-algebra-and-introduction-to-formal-proof/8/d/1/solution.md)
