<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $R=X(l)$ and $C$ be its complement, with Hilbert-space dimension $d_C$. Use [Haar twirling conditional expectation](../../../../../../haar-twirling-conditional-expectation.md) to define

$$
A_R(t)=\frac{\operatorname{Tr}_C A_X(t)}{d_C}\otimes I_C
=\int dU_C\,(I_R\otimes U_C)A_X(t)(I_R\otimes U_C^\dagger).
$$

This is an operator supported on $R$. The normalization $1/d_C$ is essential: the [partial trace](../../../../../../partial-trace.md) alone would not fix an operator already supported on $R$.

Subtract the integrand from $A_X(t)$ and use the [operator norm](../../../../../../operator-norm.md) triangle inequality. Since $A-U A U^\dagger=[A,U]U^\dagger$ and every [unitary operator](../../../../../../unitary-operator.md) has norm one, the assumed [Lieb-Robinson bound](../../../../../../lieb-robinson-bound.md), applied to a unitary supported on the entire complement, gives

$$
\|A_X(t)-A_R(t)\|
\leq 2|X|\,\|A_X\|e^{-\mu(vt+l)}(e^{2kst}-1).
$$

The factor $\min(|X|,|C|)$ was bounded by $|X|$; there is no sum over sites and hence no volume-dependent prefactor.

Choose

$$
\boxed{v=\frac{4ks}{\mu}.}
$$

For $t,l\geq0$, $e^{2kst}-1\leq2kst\,e^{2kst}$, and therefore

$$
\|A_X(t)-A_R(t)\|
\leq \mu vt\,|X|\,\|A_X\|e^{-2kst-\mu l}
\leq\boxed{\mu vt\,|X|\,\|A_X\|e^{-\mu l/2}.}
$$

Thus $A_{X(l)}(t)=A_R(t)$ is the desired [Lieb-Robinson localization by Haar twirling](../../../../../../lieb-robinson-localization-by-haar-twirling.md). The displayed choice assumes the usual positive constants $\mu,s$; if the interaction bound has $s=0$, the error is identically zero and any positive $v$ works. For negative times the same argument uses $|t|$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
