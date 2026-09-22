<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $A=\operatorname{Leb}(\mathcal C)>0$ and let $\mu$ be the [uniform distribution](../../../../../../continuous-uniform-distribution.md) on the body. The [hit-and-run kernel density](../../../../../../hit-and-run-kernel-density.md) lower bound implies

$$
P(x,B)\geq\frac{\operatorname{Leb}(B\cap\mathcal C)}{\pi D^2}\geq\varepsilon\mu(B),\qquad
\varepsilon=\frac{A}{2\pi D^2}\in(0,1).
$$

For the last range, $\mathcal C$ lies in a radius-$D$ disc about any of its points, so $A\leq\pi D^2$ and $\varepsilon\leq1/2$. This global [Doeblin condition](../../../../../../doeblin-s-condition.md) proves irreducibility with respect to $\mu$ and aperiodicity. The entire state space is a [small set](../../../../../../small-set.md); $V=1$, $\lambda=1/2$, and $b=1/2$ satisfy the [geometric drift condition](../../../../../../geometric-drift-condition.md).

In fact the conclusion is stronger. Write $P=\varepsilon\Pi+(1-\varepsilon)R$, where $\Pi(x,\cdot)=\mu$ and $R$ is the residual [Markov kernel](../../../../../../markov-kernel.md). Since $\mu P=\mu$, also $\mu R=\mu$. Each transition has a probability $\varepsilon$ of resetting to stationarity, and after such a reset every subsequent distribution remains stationary. Equivalently,

$$
\boxed{\sup_{x\in\mathcal C}\|P^n(x,\cdot)-\mu\|_{\mathrm{TV}}\leq(1-\varepsilon)^n.}
$$

Thus the algorithm has [uniform geometric ergodicity](../../../../../../uniform-geometric-ergodicity.md), using the full-dimensional and boundary conventions stated in part (a).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
