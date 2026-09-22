<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

For curvature $-1$, the [Poincare disc model](../../../../../poincare-disk-model.md) has metric and area element

$$
\boxed{ds^2=\frac{4(dx^2+dy^2)}{(1-x^2-y^2)^2}},\qquad dA=\frac{4r\,dr\,d\theta}{(1-r^2)^2}.
$$

The given minimizing-diameter property makes the distance from zero to Euclidean radius $R$ equal to

$$
\rho=\int_0^R\frac{2\,dr}{1-r^2}=\log\frac{1+R}{1-R},\qquad\boxed{R=\tanh(\rho/2)}.
$$

Radial symmetry therefore identifies the whole [hyperbolic circle in the Poincare disc](../../../../../hyperbolic-circle-in-the-poincare-disc.md). Integrating its enclosed [hyperbolic area](../../../../../hyperbolic-area.md) gives

$$
A=\int_0^{2\pi}\int_0^R\frac{4r}{(1-r^2)^2}\,dr\,d\theta=4\pi\left(\frac1{1-R^2}-1\right)=\boxed{2\pi(\cosh\rho-1)}.
$$

For a geodesic [hyperbolic triangle](../../../../../hyperbolic-triangle.md) with angles $\alpha,\beta,\gamma$, the [Gauss-Bonnet theorem](../../../../../gauss-bonnet-theorem.md) states $A=\pi-(\alpha+\beta+\gamma)$, in particular $A\leq\pi$, with strict inequality for ordinary finite vertices. Let $d$ be the distance of the interior point $P$ to the nearest side. The open disc of radius $d$ about $P$ is contained in the triangle: a path from $P$ to an exterior point must first cross the boundary at distance at least $d$. A hyperbolic isometry carries its center to zero, so its area is the area already calculated. Consequently

$$
2\pi(\cosh d-1)\leq A\leq\pi,\qquad\boxed{d\leq\operatorname{arcosh}(3/2)}.
$$

This uses [hyperbolic area bounds an inscribed disc](../../../../../hyperbolic-area-bounds-an-inscribed-disc.md) and establishes the requested bound without assuming that $P$ is an incenter. A sharper universal triangle bound is possible, but is not needed here.

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
