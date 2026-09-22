# Strong induction

↑ **Parent:** [Mathematical induction](mathematical-induction.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strong_induction)

[Strong induction](strong-induction.md) establishes a [proposition](proposition.md) $P(n)$ for all [integers](integer-split.md) $n\geq n_0$. Prove $P(n_0)$; then, for each $n\geq n_0$, assume every $P(k)$ with $n_0\leq k\leq n$ and prove $P(n+1)$. The [induction hypothesis](induction-hypothesis.md) includes all earlier cases, so the [inductive step](inductive-step.md) can use whichever smaller indices it needs. It cannot use $P(n+1)$ itself.[§5.2.1, printed p. 125: strong induction principle](mathematics-for-computer-science-by-eric-lehman-and-others.md)

This is useful when a construction breaks into smaller pieces of varying sizes. A [prime factorization](fundamental-theorem-of-arithmetic.md) splits a [composite number](composite-number.md) into smaller [integer divisors](divisor.md), which need not be one less than the original [integer](integer-split.md). A [recursive procedure](recursive-procedure.md) can likewise call itself on several smaller [inputs](input-computer-science.md). The available cases should match those dependencies. [Strong induction](strong-induction.md) lets the [mathematical proof](mathematical-proof.md) follow the construction rather than forcing every step through the immediately preceding size.

**Table of contents**

- [Strong induction with four starting cases](strong-induction-with-four-starting-cases.md)
- [Strong induction for factorization existence](strong-induction-for-factorization-existence.md)
- [Strong induction and accumulated hypotheses](strong-induction-and-accumulated-hypotheses.md)

## ↑ Ancestors (6)

1. [Mathematical induction](mathematical-induction.md)
2. [Mathematical proof](mathematical-proof.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ia/paper-4/2e/a/solution.md)
- [Strong induction](strong-induction.md)
- [Strong induction and accumulated hypotheses](strong-induction-and-accumulated-hypotheses.md)
- [Strong induction for factorization existence](strong-induction-for-factorization-existence.md)
- [Strong induction with four starting cases](strong-induction-with-four-starting-cases.md)
