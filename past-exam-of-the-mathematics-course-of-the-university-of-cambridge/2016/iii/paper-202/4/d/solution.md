<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The **[Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md)** states that an [adapted](../../../../../../adapted-process.md) continuous real process $M$ with $M_0=0$ is standard [Brownian motion](../../../../../../brownian-motion-split.md) relative to $(\mathcal F_t)$ if and only if it is a [continuous local martingale](../../../../../../continuous-local-martingale.md) and $[M]_t=t$. The multidimensional version replaces the bracket identity by $[M^i,M^j]_t=\delta_{ij}t$.

For the converse direction, a standard [Brownian motion](../../../../../../brownian-motion-split.md) is a continuous [martingale](../../../../../../martingale-split.md), and its independent centered increments give [quadratic variation](../../../../../../quadratic-variation.md) $t$. Distinct independent coordinates have zero [quadratic covariation](../../../../../../quadratic-covariation.md).

For the substantive direction, fix a vector $\theta\in\mathbb R^d$. The [Itô formula](../../../../../../ito-s-lemma.md) applied to

$$
E_t(\theta)=\exp\{i\theta\cdot M_t+\tfrac12|\theta|^2t\}
$$

shows that its drift is zero: the second-order term is $-\tfrac12|\theta|^2E_tdt$ and cancels the time derivative. Thus $E(\theta)$ is a complex [local martingale](../../../../../../local-martingale.md). On $[0,T]$ its modulus is the deterministic value $e^{|\theta|^2t/2}\leq e^{|\theta|^2T/2}$; localization and the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) make it a true [martingale](../../../../../../martingale-split.md). Hence

$$
\boxed{\mathbb E[e^{i\theta\cdot(M_t-M_s)}\mid\mathcal F_s]=e^{-\frac12|\theta|^2(t-s)}.}
$$

This conditional [characteristic function](../../../../../../characteristic-function.md) is the deterministic [characteristic function](../../../../../../characteristic-function.md) of $N(0,(t-s)I)$. For $A\in\mathcal F_s$, multiplying by $\mathbf1_A$ and taking [expectations](../../../../../../expected-value.md), then using uniqueness of [characteristic functions](../../../../../../characteristic-function.md), proves that $M_t-M_s$ has this [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) and is independent of $\mathcal F_s$. Iterated conditioning gives independent increments with [Gaussian distributions](../../../../../../normal-distribution.md). Continuity, the zero initial value and these increment laws are the definition of standard [Brownian motion](../../../../../../brownian-motion-split.md). The case $d=1$ proves the requested statement; the vector form will also be used below.

## ↑ Ancestors (11)

1. [D](../d.md)
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
