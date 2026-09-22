<h1 id="6b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In the characteristic coordinates, the [chain rule](../../../../../../chain-rule.md) gives $\partial_x=\partial_\xi+\partial_\eta$ and $\partial_t=c(\partial_\xi-\partial_\eta)$. Hence

$$
\zeta_{tt}-c^2\zeta_{xx}=-4c^2\zeta_{\xi\eta}=0.
$$

Integrating this mixed derivative gives $\zeta=F(\xi)+G(\eta)$, a sum of oppositely traveling profiles. The initial data require $F+G=u_0$ and $c(F'-G')=v_0$, so

$$
F'=\frac12\left(u_0'+\frac{v_0}c\right),\qquad G'=\frac12\left(u_0'-\frac{v_0}c\right).
$$

Integrating the profiles and matching their total additive constant gives the [D'Alembert formula with initial velocity](../../../../../../d-alembert-formula-with-initial-velocity.md):

$$
\boxed{\zeta(x,t)=\frac{u_0(x+ct)+u_0(x-ct)}2+\frac1{2c}\int_{x-ct}^{x+ct}v_0(s)\,ds.}
$$

Here $u_0$ names the initial surface displacement, rather than the water velocity $u$ appearing in the original [shallow water equations](../../../../../../shallow-water-equations.md). The formula verifies both initial conditions directly.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6B](../../6b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
