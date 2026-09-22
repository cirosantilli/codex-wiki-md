<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $u(t,x)=P_{1-t}f(x)$ for $t<1$. Differentiating the [Brownian transition semigroup](../../../../../../brownian-transition-semigroup.md) in the spatial variables is justified by the bounded gradient and gives

$$
\partial_i u(t,x)=P_{1-t}(\partial_i f)(x).
$$

The [heat equation](../../../../../../heat-equation.md) for this [semigroup](../../../../../../semigroup.md) is the backward equation $\partial_tu+\tfrac12\Delta u=0$. Applying the multidimensional [Itô formula](../../../../../../ito-s-lemma.md) yields

$$
du(t,X_t)=\left(\partial_tu+\tfrac12\Delta u\right)(t,X_t)\,dt
+\sum_{i=1}^d\partial_i u(t,X_t)\,dX_t^i.
$$

The finite-variation term vanishes. Thus

$$
\boxed{dM_t=\sum_{i=1}^d P_{1-t}(\partial_i f)(X_t)\,dX_t^i.}
$$

Initially this calculation holds on $[0,1-\varepsilon]$. The vector of [stochastic integral](../../../../../../stochastic-integral.md) coefficients has norm at most $K$, so the [Itô isometry](../../../../../../ito-isometry.md) lets the integrals extend to time one. Also $P_{1-t}f(X_t)\to f(X_1)$ in $L^2$ by the [Lipschitz function](../../../../../../lipschitz-continuity.md) bound and continuity of [Brownian motion](../../../../../../brownian-motion-split.md). The same representation therefore holds on the entire interval.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
