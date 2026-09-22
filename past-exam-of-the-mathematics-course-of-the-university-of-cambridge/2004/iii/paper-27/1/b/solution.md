<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The shifted [cyclotomic polynomial](../../../../../../cyclotomic-polynomial.md) $\Phi_{p^{n+1}}(1+T)$ is Eisenstein at $p$: its constant coefficient is $p$, and modulo $p$ it is $T^{p^n(p-1)}$. Thus $[K_n:\mathbb Q_p]=p^n(p-1)$, $\zeta_n-1$ is a [uniformizer](../../../../../../uniformizer.md), and $[K_n:K_{n-1}]=p$ for $n\geq1$. The $p$ automorphisms over $K_{n-1}$ send $\zeta_n$ to $\xi\zeta_n$ for $\xi\in\mu_p$.

Since $\zeta_n-1$ has positive valuation, evaluating an integral [formal power series](../../../../../../formal-power-series.md) there converges. A [unit](../../../../../../unit-in-a-ring.md) series has [unit](../../../../../../unit-in-a-ring.md) constant coefficient and evaluates to a [unit](../../../../../../unit-in-a-ring.md). Evaluate the [Coleman norm operator](../../../../../../coleman-norm-operator.md) identity at $T=\zeta_n-1$:

$$
\begin{aligned}
N_{K_n/K_{n-1}}\bigl(f(\zeta_n-1)\bigr)
&=\prod_{\xi^p=1}f(\xi\zeta_n-1)\\
&=(Nf)(\zeta_n^p-1)
=f(\zeta_{n-1}-1).
\end{aligned}
$$

The final equality uses norm fixation and the compatible choice of roots. Hence

$$
\boxed{N_{K_n/K_{n-1}}(u_n)=u_{n-1}\qquad(n\geq1).}
$$

In particular, norm fixation of a single [Coleman power series](../../../../../../coleman-power-series.md) produces a [norm-compatible sequence of local units](../../../../../../norm-compatible-sequence-of-local-units.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
