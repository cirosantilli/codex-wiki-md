<h1 id="15d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Dot the [Ampère-Maxwell equation](../../../../../../ampere-s-circuital-law.md) with $E$, dot [Faraday's law](../../../../../../faraday-s-law-of-induction.md) with $B/\mu_0$, and use the stated [vector](../../../../../../vector.md) identity. The result is the local balance law

$$
\frac{\partial}{\partial t}
\left[
\frac12\left(\epsilon_0E^2+\frac{B^2}{\mu_0}\right)
\right]
+\nabla\cdot S=-J\cdot E,
\qquad
S=\frac1{\mu_0}E\times B.
$$

Here $S$ is the [Poynting vector](../../../../../../poynting-vector.md). Integration over $V$ gives the [Poynting theorem](../../../../../../poynting-theorem.md)

$$
\frac{dU}{dt}
=-\int_{\partial V}S\cdot n\,dS
-\int_VJ\cdot E\,d^3x.
$$

The field energy decreases through outward electromagnetic energy flux and through work done on charges.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15D](../../15d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
