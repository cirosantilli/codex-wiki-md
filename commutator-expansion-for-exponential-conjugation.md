# Commutator expansion for exponential conjugation

↑ **Parent:** [Commutator](commutator.md)

For bounded [linear operators](linear-operator.md), or formally in an associative algebra,

$$
e^{\lambda A}Be^{-\lambda A}=\sum_{n\ge0}\frac{\lambda^n}{n!}\operatorname{ad}_A^n(B),\qquad \operatorname{ad}_A(B)=[A,B].
$$

Differentiate the two exponentials using the product rule: the result is $e^{\lambda A}[A,B]e^{-\lambda A}$. Induction gives the $n$th derivative $e^{\lambda A}\operatorname{ad}_A^n(B)e^{-\lambda A}$, and the [Taylor series](taylor-series.md) at zero proves the formula. For bounded operators convergence follows from $\|\operatorname{ad}_A^n(B)\|\le(2\|A\|)^n\|B\|$. For unbounded quantum operators, use a common invariant domain and justify the series there, or use the finite-dimensional system of commutators when their span closes.

**Table of contents**

- [Central-commutator exponential identity](central-commutator-exponential-identity.md)

## ↑ Ancestors (9)

1. [Commutator](commutator.md)
2. [Lie bracket](lie-bracket.md)
3. [Lie algebra](lie-algebra-split.md)
4. [Lie theory](lie-theory-split.md)
5. [Diagonal dominance](diagonal-dominance.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-49/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4/32c/solution.md)
