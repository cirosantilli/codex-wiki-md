<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

An [ideal hyperbolic triangle](../../../../../ideal-triangle.md) has its three vertices at infinity, with sides given by [geodesics](../../../../../geodesic.md). In curvature $-1$ its angles are zero and its area is **$\pi$**, using the [hyperbolic triangle area](../../../../../hyperbolic-triangle-area.md) formula $\pi-(\alpha+\beta+\gamma)$.

To calculate the [area of a hyperbolic disc](../../../../../area-of-a-hyperbolic-disc.md), use the [Poincare disc model](../../../../../poincare-disk-model.md) centered at the origin. Hyperbolic radial distance is $\rho=\int_0^R2\,dr/(1-r^2)=2\operatorname{artanh}R$, so its Euclidean radius is $R=\tanh(\rho/2)$. The metric area density is $4r\,dr\,d\theta/(1-r^2)^2$, giving

$$
A(\rho)=2\pi\int_0^R\frac{4r}{(1-r^2)^2}\,dr=4\pi\left(\frac1{1-R^2}-1\right)=\boxed{2\pi(\cosh\rho-1)}.
$$

Every [hyperbolic triangle](../../../../../hyperbolic-triangle.md), including ones with ideal vertices, has area at most $\pi$. But $A(2)=2\pi(\cosh2-1)>\pi$. A [hyperbolic triangle](../../../../../hyperbolic-triangle.md) is geodesically convex, so if it contains a complete [hyperbolic circle](../../../../../hyperbolic-circle.md), it also contains the enclosed [hyperbolic disc](../../../../../hyperbolic-disc.md), its [geodesic](../../../../../geodesic.md) convex hull. This would violate the area comparison. Therefore **no hyperbolic triangle contains a complete circle of radius two**.

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
