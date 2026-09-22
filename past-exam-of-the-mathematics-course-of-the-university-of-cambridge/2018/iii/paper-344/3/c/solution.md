<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the stated [uniaxial nematic order](../../../../../../uniaxial-nematic-order.md) normalization, the [nematic director](../../../../../../nematic-director.md) is an [eigenvector](../../../../../../eigenvector.md) of $Q$ with [eigenvalue](../../../../../../eigenvalue.md) $\lambda$, and the two perpendicular [eigenvalues](../../../../../../eigenvalue.md) are $-\lambda/2$. Therefore

$$
\operatorname{Tr}Q^2=\frac32\lambda^2,
\qquad \operatorname{Tr}Q^3=\frac34\lambda^3,
\qquad (\operatorname{Tr}Q^2)^2=\frac94\lambda^4.
$$

Using precisely the [Landau-de Gennes free energy](../../../../../../landau-de-gennes-free-energy.md) convention in the preceding solution gives

$$
\boxed{\bar a=\frac{3a}{4},\qquad \bar b=\frac{9b}{16},\qquad \bar c=\frac c4}.
$$

If the quartic invariant were instead normalized as $b\operatorname{Tr}Q^4/4$, its coefficient would be $\bar b=9b/32$; the physical predictions are unchanged after redefining $b$.

For a nonzero [global minimizer](../../../../../../global-minimizer.md) of the [free energy](../../../../../../thermodynamic-free-energy.md), compare opposite values of the scalar [nematic order parameter](../../../../../../nematic-order-parameter.md):

$$
f(\lambda)-f(-\lambda)=2\bar c\lambda^3.
$$

The lower one has $\bar c\lambda<0$, so

$$
\boxed{\operatorname{sgn}\lambda_{\rm eq}=-\operatorname{sgn}\bar c\quad(\bar c\ne0)}.
$$

The claim concerns the stable ordered phase, not every metastable stationary point. For $\bar c=0$ the two signs are degenerate. For $\bar c\ne0$, equality of the ordered and isotropic [free energies](../../../../../../thermodynamic-free-energy.md), together with stationarity, gives $\lambda_t=-\bar c/(2\bar b)$ and $\bar a_t=\bar c^2/(4\bar b)>0$. The finite jump $\lambda_t$ exhibits the [first-order phase transition](../../../../../../first-order-phase-transition.md) driven by the cubic invariant.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
