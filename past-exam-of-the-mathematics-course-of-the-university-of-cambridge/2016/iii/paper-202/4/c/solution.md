<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use two standard results: for every [continuous local martingale](../../../../../../continuous-local-martingale.md) $U$, there is a unique continuous [adapted](../../../../../../adapted-process.md) increasing [quadratic variation](../../../../../../quadratic-variation.md) $[U]$, starting at zero, such that $U^2-U_0^2-[U]$ is a [local martingale](../../../../../../local-martingale.md); and a [continuous finite-variation local martingale is constant](../../../../../../continuous-finite-variation-local-martingale-is-constant.md).

Define the **[quadratic covariation](../../../../../../quadratic-covariation.md)** by the [polarization identity](../../../../../../polarization-identity.md)

$$
\boxed{[M,N]=\frac14\bigl([M+N]-[M-N]\bigr).}
$$

This is continuous, [adapted](../../../../../../adapted-process.md), starts at zero, and is of [finite variation](../../../../../../total-variation-of-a-function.md) on compact time intervals. Since $(M+N)^2-(M-N)^2=4MN$, subtraction of the two quadratic-variation identities shows that $MN-M_0N_0-[M,N]$ is a [continuous local martingale](../../../../../../continuous-local-martingale.md). In the zero-start convention this is exactly $MN-[M,N]\in\mathcal M_{c,\mathrm{loc}}$.

If $A$ is another continuous [adapted](../../../../../../adapted-process.md) [finite-variation process](../../../../../../finite-variation-process.md) with $A_0=0$ and the same [local martingale](../../../../../../local-martingale.md) property, then $A-[M,N]$ is both a [continuous local martingale](../../../../../../continuous-local-martingale.md) and of [finite variation](../../../../../../total-variation-of-a-function.md). It is constant, and its initial value is zero, so it vanishes. Uniqueness is up to [indistinguishability of stochastic processes](../../../../../../indistinguishability-of-stochastic-processes.md).

**The normalization $[M,N]_0=0$ is essential.** If arbitrary nonzero initial constants are allowed in the [martingale](../../../../../../martingale-split.md) class and this normalization is omitted, adding a constant to the bracket preserves the claimed property. The usual definition of [quadratic covariation](../../../../../../quadratic-covariation.md) always includes the zero initial value.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
