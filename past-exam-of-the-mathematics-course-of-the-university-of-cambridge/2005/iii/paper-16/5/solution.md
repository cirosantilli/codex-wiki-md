<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

We first prove invariance, before using any assertion that requires it. Write $A_n\varphi(x)=n^{-1}\sum_{k=0}^{n-1}\varphi(f^kx)$. Choose a point whose forward [orbit](../../../../../orbit-dynamical-system.md) has the prescribed convergence against every [continuous function](../../../../../continuous-function.md); the hypothesis gives a set of such points of full [measure](../../../../../measure.md). For each [continuous function](../../../../../continuous-function.md) $\varphi$, telescoping gives

$$
A_n(\varphi\circ f)(x)-A_n\varphi(x)
=\frac{\varphi(f^nx)-\varphi(x)}n\longrightarrow0,
$$

because a [continuous function](../../../../../continuous-function.md) on a [compact metric space](../../../../../compact-metric-space.md) is bounded. Both test functions are continuous, so their averages converge to their prescribed integrals. Hence

$$
\int_X\varphi\circ f\,d\mu=\int_X\varphi\,d\mu
$$

for every [continuous function](../../../../../continuous-function.md) $\varphi$. The continuous-test criterion for an [invariant measure](../../../../../invariant-measure.md) therefore gives **$f_*\mu=\mu$**. The points in the hypothesis can now be called [generic points for an invariant measure](../../../../../generic-point-for-an-invariant-measure.md).

For [ergodicity](../../../../../ergodicity.md), let $B$ be a [Borel set](../../../../../borel-set.md) invariant modulo null sets, and set $h=\mathbf1_B$, $p=\mu(B)$. Then $h\circ f=h$ almost everywhere. Since invariance preserves null preimages, deleting the union of all iterated preimages of the exceptional [null set](../../../../../null-set.md) gives $h(f^kx)=h(x)$ for every $k\geq0$ on one full-measure set. Thus $A_nh=h$ almost everywhere for every $n$.

Given $\epsilon>0$, the [continuous approximation of Borel indicators on a compact metric space](../../../../../continuous-approximation-of-borel-indicators-on-a-compact-metric-space.md), proved in the supporting steps below, supplies $\varphi\in C(X)$ with $0\leq\varphi\leq1$ and $\|h-\varphi\|_{L^1(\mu)}<\epsilon$. By the hypothesis, $A_n\varphi\to\int\varphi\,d\mu$ almost everywhere. Since $0\leq A_n\varphi\leq1$, the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) also gives convergence in $L^1(\mu)$. Invariance and the [triangle inequality](../../../../../triangle-inequality.md) give the uniform estimate

$$
\|A_n(h-\varphi)\|_{L^1(\mu)}
\leq\frac1n\sum_{k=0}^{n-1}\int_X|h-\varphi|\circ f^k\,d\mu
=\|h-\varphi\|_{L^1(\mu)}<\epsilon.
$$

Consequently,

$$
\begin{aligned}
\|h-p\|_{L^1(\mu)}
&\leq\|A_nh-A_n\varphi\|_{L^1(\mu)}
 +\left\|A_n\varphi-\int\varphi\,d\mu\right\|_{L^1(\mu)}
 +\left|\int\varphi\,d\mu-p\right|\\
&<2\epsilon+\left\|A_n\varphi-\int\varphi\,d\mu\right\|_{L^1(\mu)}.
\end{aligned}
$$

Letting $n\to\infty$ and then $\epsilon\downarrow0$ proves $\|h-p\|_1=0$. Explicitly,

$$
\|\mathbf1_B-p\|_1=p(1-p)+(1-p)p=2p(1-p),
$$

so $p\in\{0,1\}$. Every invariant [Borel set](../../../../../borel-set.md) has [measure](../../../../../measure.md) zero or one, which proves

$$
\boxed{\mu\text{ is invariant and ergodic}.}
$$

This proof controls measurable-set averages through a uniform $L^1$ estimate; convergence only against continuous test functions is not silently assumed to include [indicator functions](../../../../../indicator-function.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
