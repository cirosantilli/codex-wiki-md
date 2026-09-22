<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take a standard [Brownian motion](../../../../../../brownian-motion-split.md) $B$ and define

$$
\boxed{M_t=B_{t\wedge1},\qquad N_t=B_{t\wedge1}^2-(t\wedge1)}.
$$

The [Itô formula](../../../../../../ito-s-lemma.md) gives $N_t=2\int_0^{t\wedge1}B_s\,dB_s$, so both are [continuous martingales](../../../../../../continuous-martingale.md) starting at zero. Their second moments are $\mathbb EM_t^2=t\wedge1$ and $\mathbb EN_t^2=2(t\wedge1)^2$, making them [L2-bounded continuous martingales](../../../../../../l2-bounded-continuous-martingale.md). At equal times, the odd moments of a centered [normal random variable](../../../../../../gaussian-random-variable.md) vanish, so

$$
\mathbb E[M_tN_t]=\mathbb E[B_{t\wedge1}^3]-(t\wedge1)\mathbb EB_{t\wedge1}=0.
$$

They are consequently [weakly orthogonal continuous martingales](../../../../../../weakly-orthogonal-continuous-martingales.md) by [solution](../a/i/solution.md).

Their product, for $t<1$, is $B_t^3-tB_t$. The [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
d(M_tN_t)=(3B_t^2-t)\,dB_t+2B_t\,dt.
$$

The continuous finite-variation term $2\int_0^tB_s\,ds$ is not identically zero: it has variance $4t^3/3$ at every $t>0$. Uniqueness of the continuous semimartingale decomposition therefore shows that $MN$ is not even a [local martingale](../../../../../../local-martingale.md). Equivalently $[M,N]_t=2\int_0^{t\wedge1}B_s\,ds$ is not zero, so the pair is not [orthogonal continuous local martingales](../../../../../../orthogonal-continuous-local-martingales.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
