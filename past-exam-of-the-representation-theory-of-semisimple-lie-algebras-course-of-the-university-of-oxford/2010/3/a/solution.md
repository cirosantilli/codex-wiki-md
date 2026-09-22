<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With the source's negative [root](../../../../root-of-a-root-system.md) partition function, interpret $Q_+=\sum_{\alpha\in B}\mathbb Z_{\ge0}\alpha$ and allow zero coefficients in the partitions. Write $e^\lambda$ for $\delta_\lambda$, with multiplication meaning [convolution](../../../../convolution.md). Then

$$
K=\prod_{\gamma>0}\left(\sum_{n\ge0}e^{-n\gamma}\right).
$$

The denominator needed for the asserted character identities is

$$
D=\prod_{\gamma>0}(e^{\gamma/2}-e^{-\gamma/2})
=e^\rho\prod_{\gamma>0}(1-e^{-\gamma}).
$$

The repeated identical subscripts in the printed denominator would instead make it zero, so those literal factors cannot satisfy an inverse identity. Also the required inverse uses the negative $\rho$ shift. Geometric-series cancellation gives

$$
\boxed{K*\delta_{-\rho}*D=\delta_0.}
$$

With a positive shift the left side would be $\delta_{2\rho}$, which displays the second printed sign problem even after the denominator is repaired.

[Poincaré-Birkhoff-Witt theorem](../../../../poincare-birkhoff-witt-theorem.md) gives $\pi_{M^\xi}=\delta_{\xi-\rho}*K$, since each ordered negative [root](../../../../root-of-a-root-system.md) monomial lowers the [highest weight](../../../../highest-weight-of-a-representation.md) by its corresponding partition. Therefore

$$
\boxed{D*\pi_{M^\xi}=\delta_\xi.}
$$

The remaining parts use $D$ for the intended [Weyl denominator](../../../../weyl-denominator.md), while the private TeX preserves the printed signs.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the representation theory of semisimple Lie algebras course of the University of Oxford](../../../split.md)
5. [Representation theory of semisimple Lie algebras course of the University of Oxford](../../../../representation-theory-of-semisimple-lie-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
