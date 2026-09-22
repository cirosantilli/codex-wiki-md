<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $U=M-\tfrac12[M]$. Since the bracket is continuous [finite variation](../../../../../../total-variation-of-a-function.md), $[U]=[M]$. The [Itô formula](../../../../../../ito-s-lemma.md) applied to $Z=e^U$ gives

$$
dZ_t=Z_t\,dU_t+\frac12Z_t\,d[U]_t=Z_t\,dM_t-\frac12Z_t\,d[M]_t+\frac12Z_t\,d[M]_t.
$$

Therefore

$$
\boxed{dZ_t=Z_t\,dM_t.}
$$

With the printed exponential formula, $Z_0=e^{M_0}$. The usual unit-initial-value [stochastic exponential](../../../../../../doleans-dade-exponential.md) is $\exp(M_t-M_0-\tfrac12[M]_t)$; the two coincide when $M_0=0$, as in part (c).

For any strictly positive solution of this stochastic equation, its bracket is $d[Z]_t=Z_t^2d[M]_t$. Applying Itô to the logarithm, after localizing away from zero if necessary, gives

$$
d\log Z_t=\frac{dZ_t}{Z_t}-\frac{d[Z]_t}{2Z_t^2}=dM_t-\frac12d[M]_t.
$$

The same identity holds for $Z'$, so $\log Z_t'-\log Z_t$ is constant in time and is zero initially. Their continuous versions agree at all times on one full-probability event. Thus [pathwise uniqueness for a multiplicative martingale equation](../../../../../../pathwise-uniqueness-for-a-multiplicative-martingale-equation.md) gives

$$
\boxed{\mathbb P(Z_t'=Z_t\text{ for every }t\geq0)=1.}
$$

This is [indistinguishability of stochastic processes](../../../../../../indistinguishability-of-stochastic-processes.md), not just equality almost surely at each separately chosen time.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
