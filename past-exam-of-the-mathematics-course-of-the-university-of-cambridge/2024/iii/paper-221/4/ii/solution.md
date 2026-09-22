<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $p_x=\mathbb P(X=x)$, $\pi_x=\mathbb E(A\mid X=x)$, and $\mu_x=\mathbb E(Y\mid X=x)$. The functional is

$$
\beta=\mathbb E(AY)-\sum_xp_x\pi_x\mu_x.
$$

The first term has [influence function](../../../../../../influence-function.md) $AY-\mathbb E(AY)$. Applying the product rule to the second term, including perturbations of $p_x$, $\pi_x$, and $\mu_x$, gives

$$
\pi(X)\mu(X)-\mathbb E[\pi(X)\mu(X)]
+\mu(X)\{A-\pi(X)\}
+\pi(X)\{Y-\mu(X)\}.
$$

Subtracting and using $\beta=\mathbb E(AY)-\mathbb E[\pi\mu]$ yields

$$
\psi(X,A,Y)
=\{A-\pi(X)\}\{Y-\mu(X)\}-\beta.
$$

Its expectation is zero because the first product has expectation $\mathbb E\{\operatorname{Cov}(A,Y\mid X)\}=\beta$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
