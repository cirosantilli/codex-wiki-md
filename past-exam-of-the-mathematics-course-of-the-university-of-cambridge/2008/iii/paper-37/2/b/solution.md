<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0<a<x<b$, put $S=\tau_a\wedge\tau_b$. The process $\phi(\|B_{t\wedge S}\|)$, where $\phi(r)=r^{2-d}$, is a bounded [martingale](../../../../../../martingale-split.md) by part (a). Also $S<\infty$ almost surely: before exit the endpoint $B_t$ lies inside the radius-$b$ ball, whose Gaussian probability tends to zero as $t\to\infty$. Path continuity makes the terminal radius either $a$ or $b$. If $p=\mathbb P_{\bar x}(\tau_a<\tau_b)$, the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) applied to this bounded stopped [martingale](../../../../../../martingale-split.md) gives

$$
\phi(x)=p\phi(a)+(1-p)\phi(b).
$$

Solving yields

$$
\boxed{\mathbb P_{\bar x}(\tau_a<\tau_b)=\frac{\phi(b)-\phi(x)}{\phi(b)-\phi(a)}.}
$$

The denominator is nonzero because $\phi$ is strictly decreasing for $d\geq3$.

As $b\uparrow\infty$, the events $\{\tau_a<\tau_b\}$ increase to $\{\tau_a<\infty\}$. In one direction membership already implies a finite hit of $a$; in the other direction a continuous path up to its finite hit of $a$ has a finite maximum radius, so it lies in the event for every sufficiently large $b$. Continuity from below of probability and $\phi(b)\to0$ now give

$$
\boxed{\mathbb P_{\bar x}(\tau_a<\infty)=\frac{x^{2-d}}{a^{2-d}}=\left(\frac ax\right)^{d-2}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
