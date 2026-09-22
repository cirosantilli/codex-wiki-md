<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On the finite horizon $[0,T]$, strict positivity gives equivalence of the restricted probability measures: for $A\in\mathcal F_T$, $\mathbb Q(A)=\mathbb E_{\mathbb P}(Z_T\mathbf1_A)$ vanishes if and only if $\mathbb P(A)$ vanishes. The standard change-of-measure theorem gives [semimartingale invariance under equivalent measures](../../../../../../semimartingale-invariance-under-equivalent-measures.md): **a process is a semimartingale under $\mathbb P$ on this horizon if and only if it is one under $\mathbb Q$**. The sample-path [quadratic variation](../../../../../../quadratic-variation.md) is unchanged, but the local-[martingale](../../../../../../martingale-split.md) and finite-variation parts generally change.

More explicitly, set $N=\int Z^{-1}\,dZ$, the zero-start [stochastic logarithm](../../../../../../stochastic-logarithm.md) of the density. For every continuous $\mathbb P$-[local martingale](../../../../../../local-martingale.md) $L$, the [Girsanov theorem](../../../../../../girsanov-theorem.md) states that

$$
\boxed{L_t^{\mathbb Q}=L_t-\int_0^t\frac{d[L,Z]_s}{Z_s}=L_t-[L,N]_t}
$$

is a continuous $\mathbb Q$-[local martingale](../../../../../../local-martingale.md). Consequently, if the continuous [semimartingale decomposition](../../../../../../semimartingale-decomposition.md) under $\mathbb P$ is $X=X_0+L+V$, its decomposition under $\mathbb Q$ is

$$
X=X_0+L^{\mathbb Q}+\bigl(V+[L,N]\bigr).
$$

The covariation correction is a continuous [finite-variation process](../../../../../../finite-variation-process.md), locally well-defined because $Z$ stays strictly positive. In the Brownian case, if $dZ_t=Z_t\theta_t\,dB_t$, then

$$
B_t^{\mathbb Q}=B_t-\int_0^t\theta_s\,ds
$$

is a [Brownian motion](../../../../../../brownian-motion-split.md) under $\mathbb Q$. The inverse finite-horizon density is $1/Z$, giving the reverse change of measure. These assertions apply on each horizon on which the density is strictly positive; they do not assert equivalence on a larger terminal sigma-algebra where the full density $D$ may vanish.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
