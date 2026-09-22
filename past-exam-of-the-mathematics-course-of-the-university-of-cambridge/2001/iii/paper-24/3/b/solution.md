<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There is an initial-value qualification in the printed conclusion. As written, nothing requires $A_0=0$. For example, $M\equiv0$ and $A\equiv1$ satisfy the hypotheses, because $M^2-A\equiv-1$ is a [local martingale](../../../../../../local-martingale.md), but $M_t$ is not $N(0,1)$. **The correct variance is $A_t-A_0$; the printed formula holds under the usual normalization $A_0=0$.**

Indeed, $M^2-[M]$ is a [continuous local martingale](../../../../../../continuous-local-martingale.md). Subtracting it from $M^2-A$ shows that $[M]-A$ is a continuous [local martingale](../../../../../../local-martingale.md) with [finite variation](../../../../../../total-variation-of-a-function.md), hence is its initial constant $-A_0$. Thus

$$
C_t:=A_t-A_0=[M]_t.
$$

In particular, $C$ is deterministic, continuous, nonnegative and increasing, regardless of the apparent allowance of a general [finite-variation process](../../../../../../finite-variation-process.md) in the premise.

For a real parameter $\theta$, the [Itô formula](../../../../../../ito-s-lemma.md) gives the complex [local martingale](../../../../../../local-martingale.md)

$$
Z_t=\exp\left(i\theta M_t+\frac{\theta^2}{2}C_t\right),
\qquad dZ_t=i\theta Z_t\,dM_t.
$$

On every deterministic interval $[0,T]$, its modulus is at most $e^{\theta^2C_T/2}$, so its real and imaginary parts are bounded [local martingales](../../../../../../local-martingale.md), hence true [martingales](../../../../../../martingale-split.md). Taking [expectations](../../../../../../expected-value.md) and using $Z_0=1$ yields

$$
\mathbb E e^{i\theta M_t}=e^{-\theta^2C_t/2}.
$$

By the [uniqueness theorem for characteristic functions](../../../../../../uniqueness-theorem-for-characteristic-functions.md),

$$
\boxed{M_t\sim N(0,A_t-A_0).}
$$

A zero variance means the point mass at zero. This proves the requested normalized version by a direct [characteristic function](../../../../../../characteristic-function.md) calculation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
