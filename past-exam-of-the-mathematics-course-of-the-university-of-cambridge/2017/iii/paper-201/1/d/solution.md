<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $M_k=S_k-mk$ as above. Centering the [linear interpolation](../../../../../../linear-interpolation.md) also interpolates the centered values: for $u\in[0,1]$,

$$
S_{k+u}-m(k+u)=(1-u)M_k+uM_{k+1}.
$$

The absolute value of this convex combination is at most the larger endpoint absolute value. For every fixed $A>0$, part (c) therefore gives

$$
\mathbb E\!\left[\sup_{0\leq t\leq A}|S_t^{(N)}-mt|^2\right]
\leq \frac{4\sigma^2\lceil NA\rceil}{N^2}\longrightarrow0.
$$

Hence there is [uniform convergence on compacts in probability](../../../../../../uniform-convergence-on-compacts-in-probability.md) to the deterministic path $h(t)=mt$, by [Markov inequality](../../../../../../markov-inequality.md). Equip $C([0,\infty),\mathbb R)$ with its standard [compact-open topology](../../../../../../compact-open-topology.md), metrized by

$$
d(f,g)=\sum_{j=1}^{\infty}2^{-j}\left(1\wedge\sup_{0\leq t\leq j}|f(t)-g(t)|\right).
$$

For each finite number of terms their suprema converge to zero in probability, and the remaining tail is bounded deterministically by $\sum_{j>J}2^{-j}$. Thus $d(S^{(N)},h)\to0$ in probability. [Convergence in probability](../../../../../../convergence-in-probability.md) to a deterministic point implies [weak convergence of probability measures](../../../../../../weak-convergence-of-probability-measures.md), so the [fluid limit](../../../../../../fluid-limit.md) is

$$
\boxed{\mu_N\Longrightarrow\delta_h,\qquad h(t)=mt.}
$$

Here $\delta_h$ is the [Dirac measure](../../../../../../dirac-measure.md) concentrated on that continuous path. The topology is [locally uniform convergence](../../../../../../locally-uniform-convergence.md); no assertion of [uniform convergence](../../../../../../uniform-convergence.md) over the entire unbounded half-line is needed. The interpolation is intended for integers $k\geq0$, including the initial interval $[0,1]$. If the PDF's $\mathbb Z^+$ is interpreted as strictly positive integers, that initial piece is omitted from the displayed definition and must be supplied by the same formula using $S_0=0$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
