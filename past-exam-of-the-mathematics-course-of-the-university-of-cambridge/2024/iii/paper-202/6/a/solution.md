<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix $t>0$ and define $w(s,y)=u(t-s,|y|)$ for $0\leq s\leq t$. The assumed smooth extension and the [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) at zero make $w$ a $C^{1,2}$ function. The [heat equation](../../../../../../heat-equation.md) gives

$$
w_s+\frac12w_{yy}=0.
$$

The [Itô formula](../../../../../../ito-s-lemma.md) therefore makes $w(s,B_s)$ a local martingale. Stop first when $|B|$ leaves a large compact interval. The exponential growth bound and the finite exponential moments of the maximum of [Brownian motion](../../../../../../brownian-motion-split.md) on $[0,t]$ give [uniform integrability](../../../../../../uniform-integrability.md), so localization and the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) yield

$$
u(t,x)=w(0,x)=\mathbb E_x[w(t,B_t)]=\mathbb E_x[f(|B_t|)].
$$

This is the [Feynman-Kac formula](../../../../../../feynman-kac-formula.md) for the Neumann heat problem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
