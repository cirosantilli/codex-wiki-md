<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [probability measures](../../../../../../probability-measure.md) on a metric space, [weak convergence of probability measures](../../../../../../weak-convergence-of-probability-measures.md) $\mu_n\Rightarrow\mu$ means $\int f\,d\mu_n\to\int f\,d\mu$ for every bounded continuous real function $f$. On the real line it is equivalently convergence of the [cumulative distribution functions](../../../../../../cumulative-distribution-function.md) at every continuity point of the limiting [cumulative distribution function](../../../../../../cumulative-distribution-function.md). Bounded continuous upper and lower approximations to interval indicators give one direction; a partition at continuity points, uniform approximation on a compact interval, and control of the tails give the reverse direction.

For a [probability measure](../../../../../../probability-measure.md) $\mu$ on $\mathbb R$, its [characteristic function](../../../../../../characteristic-function.md) is $\varphi_\mu(t)=\int e^{itx}\mu(dx)$. The [Lévy continuity theorem](../../../../../../levy-continuity-theorem.md) states: $\mu_n\Rightarrow\mu$ implies $\varphi_{\mu_n}(t)\to\varphi_\mu(t)$ for every real $t$; conversely, if these [characteristic functions](../../../../../../characteristic-function.md) have a pointwise limit $\varphi$ which is continuous at zero, there is a unique [probability measure](../../../../../../probability-measure.md) $\mu$ with [characteristic function](../../../../../../characteristic-function.md) $\varphi$, and $\mu_n\Rightarrow\mu$. In particular, for a specified limiting [probability measure](../../../../../../probability-measure.md), weak convergence is equivalent to pointwise convergence of its [characteristic functions](../../../../../../characteristic-function.md).

The forward implication follows by testing cosine and sine. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) shows that every [characteristic function](../../../../../../characteristic-function.md) is continuous at zero and has value one there. For the converse, first establish [tightness of probability measures](../../../../../../uniform-tightness.md). By [Fubini's theorem](../../../../../../fubini-s-theorem.md), for $h>0$,

$$
\frac1{2h}\int_{-h}^h(1-\operatorname{Re}\varphi_{\mu_n}(t))\,dt
=\int\left(1-\frac{\sin(hx)}{hx}\right)\mu_n(dx).
$$

The integrand on the right is at least $1/2$ when $|x|\geq2/h$. This proves the [characteristic-function tightness bound](../../../../../../characteristic-function-tightness-bound.md)

$$
\mu_n(|x|\geq2/h)\leq\frac1h\int_{-h}^h(1-\operatorname{Re}\varphi_{\mu_n}(t))\,dt.
$$

The integrals converge for each $h$ by [dominated convergence](../../../../../../dominated-convergence-theorem.md), and continuity of $\varphi$ at zero makes the limit as small as desired by choosing $h$ small. Thus all sufficiently late measures have a common tail bound; the finitely many earlier measures also have small tails once the radius is increased. This is uniform [tightness of probability measures](../../../../../../uniform-tightness.md).

We give the required compactness argument explicitly. For any subsequence, choose a further diagonal subsequence whose [cumulative distribution functions](../../../../../../cumulative-distribution-function.md) $F_n$ converge at every rational $q$, to $f(q)$. Define

$$
F(x)=\inf_{\substack{q>x\\q\in\mathbb Q}}f(q).
$$

This function is nondecreasing and right-continuous: given a rational $q>x$ with $f(q)$ close to $F(x)$, the same bound holds for $F(y)$ when $x<y<q$. Tightness gives $F(-\infty)=0$ and $F(+\infty)=1$, so $F$ is a [cumulative distribution function](../../../../../../cumulative-distribution-function.md) of a [probability measure](../../../../../../probability-measure.md) $\nu$. For rationals $r<x<s$, $F_n(r)\leq F_n(x)\leq F_n(s)$. The limits bracket $F(x-)$ and $F(x)$; at a continuity point of $F$ they coincide. Thus $F_n(x)\to F(x)$ at all such points. To obtain weak convergence, choose a compact interval with small tails and partition it using continuity points of $F$. A bounded continuous function is uniformly continuous there, so step-function approximations and convergence of interval probabilities prove convergence of its integral. This proves [Helly selection for distribution functions](../../../../../../helly-selection-for-distribution-functions.md) and supplies a weak subsequential limit $\nu$.

Its [characteristic function](../../../../../../characteristic-function.md) is $\varphi$ by the already proved forward implication. We also prove uniqueness rather than assume it. If two [probability measures](../../../../../../probability-measure.md) $\nu,\rho$ have the same [characteristic function](../../../../../../characteristic-function.md), convolve each with a centered [normal distribution](../../../../../../normal-distribution.md) of variance $\varepsilon^2>0$. Their densities are, by the [Gaussian integral](../../../../../../gaussian-integral.md) and [Fubini's theorem](../../../../../../fubini-s-theorem.md),

$$
p_{\nu,\varepsilon}(x)=\frac1{2\pi}\int_{\mathbb R}e^{-itx}\varphi_\nu(t)e^{-\varepsilon^2t^2/2}\,dt,
$$

and likewise for $\rho$. The integrable Gaussian factor justifies exchanging the integrals, so these densities agree. For every bounded continuous $f$, letting $\varepsilon\downarrow0$ in $\int\mathbb E[f(x+\varepsilon Z)]\nu(dx)$, with $Z$ a standard [normal random variable](../../../../../../gaussian-random-variable.md), gives $\int f\,d\nu$ by [bounded convergence theorem](../../../../../../bounded-convergence-theorem.md). Hence the two measures have equal integrals against all these test functions, and approximating interval indicators shows $\nu=\rho$. This proves the [uniqueness theorem for characteristic functions](../../../../../../uniqueness-theorem-for-characteristic-functions.md).

Every subsequence therefore has a further subsequence weakly converging to the same unique $\mu$. If the original sequence failed weak convergence, some bounded continuous test function would have a subsequence of integrals staying a fixed distance from its integral under $\mu$, contradicting that further convergence. This completes both directions of the theorem. Continuity at zero is essential: the laws $N(0,n)$ have pointwise limiting [characteristic function](../../../../../../characteristic-function.md) zero away from zero and one at zero, and are not tight.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
