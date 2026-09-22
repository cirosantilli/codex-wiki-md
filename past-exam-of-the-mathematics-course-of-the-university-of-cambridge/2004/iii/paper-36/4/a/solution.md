<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Normalize the second price to one and write $p>0$ for the first price and $t>0$ for the varying endowment. Let $Z(p,t)$ be first-good [aggregate excess demand](../../../../../../aggregate-excess-demand.md). Under [Walras law](../../../../../../walras-s-law.md), the second excess-demand coordinate equals $-pZ(p,t)$, so one market-clearing equation suffices. A [regular exchange economy](../../../../../../regular-exchange-economy.md) at fixed $t$ has $Z_p(p,t)\ne0$ at every equilibrium.

A sufficient joint condition is that zero be a [regular value](../../../../../../regular-value.md) of the smooth map $Z:(0,\infty)^2\to\mathbb R$:

$$
\boxed{Z(p,t)=0\quad\Longrightarrow\quad (Z_p(p,t),Z_t(p,t))\ne(0,0).}
$$

To prove the almost-everywhere conclusion, the [regular level set theorem](../../../../../../regular-level-set-theorem.md) makes $M=Z^{-1}(0)$ a smooth one-dimensional [manifold](../../../../../../topological-manifold.md). Project $M$ to the parameter axis by $\pi(p,t)=t$. Its [tangent space](../../../../../../tangent-space.md) consists of vectors $(h,k)$ with $Z_ph+Z_tk=0$. If $Z_p\ne0$, every $k$ is possible, so the derivative of $\pi$ is surjective. If $Z_p=0$, the joint condition gives $Z_t\ne0$, forcing $k=0$; the point is critical for $\pi$.

Thus the parameters with a singular equilibrium are exactly the critical values of this projection. [Sard theorem](../../../../../../sard-s-theorem.md) makes that set a [null set](../../../../../../null-set.md). Therefore **almost every parameter gives a regular economy**. No claim of existence at every parameter is needed for this sufficient regularity criterion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
