<h1 id="3c/solution">Solution</h1>

↑ **Parent:** [3C](../3c.md)

A [differential one-form](../../../../../one-form.md) $P\,dx+Q\,dy$ is an [exact differential](../../../../../exact-differential.md) if there is a differentiable [function](../../../../../function-split.md) $F$ with $P=F_x$ and $Q=F_y$, so the form equals $dF$. For continuously differentiable $P,Q$, equality of mixed [partial derivatives](../../../../../partial-derivative.md) gives the necessary condition

$$
\boxed{P_y=Q_x.}
$$

A local differential condition need not by itself give a global potential on a domain with holes; no such issue arises for the explicit primitives here.

For the first form, $P_y=2y=Q_x$ and direct differentiation gives

$$
\boxed{y^2\,dx+2xy\,dy=d(xy^2).}
$$

For the second, $P_y=2y$ but $Q_x=y^2$. These are not equal on any nonempty open subset of the plane, so that form is not an [exact differential](../../../../../exact-differential.md). Nevertheless,

$$
y^2\,dx+xy^2\,dy=y^2(dx+x\,dy)
=\boxed{y^2e^{-y}\,d(xe^y)}.
$$

Thus one suitable pair is $f(x,y)=xe^y$, $g(y)=y^2e^{-y}$. This factorization is smooth even at $y=0$. On regions where $y\ne0$, its reciprocal factor $e^y/y^2$ is an [integrating factor](../../../../../integrating-factor.md) which turns the original form into $df$.

## ↑ Ancestors (10)

1. [3C](../3c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
