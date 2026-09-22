<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a sufficiently smooth exact solution, the centered spatial residual is

$$
D_{xx}u-\alpha D_xu-(u_{xx}-\alpha u_x)
=h^2\left(\frac{u_{xxxx}}{12}-\frac{\alpha u_{xxx}}6\right)+O(h^4).
$$

Let $e=U-R_hu$ be the nodal error. It satisfies $e'=A_he+\tau_h$, with $A_h=D_{xx}-\alpha D_x$ and $\|\tau_h\|_h\leq Ch^2$ on the fixed time interval. Part (a) gives $\|e^{tA_h}\|\leq1$, so Duhamel's formula yields

$$
\boxed{\|e(t)\|_h\leq\|e(0)\|_h+\int_0^t\|\tau_h(s)\|_hds
\leq\|e(0)\|_h+Cth^2.}
$$

Thus the method is convergent, with second-order spatial error for smooth data and second-order compatible initialization. The homogeneous endpoint values introduce no boundary residual. For nonsmooth L2 data, stable approximating projections and a density argument extend [numerical convergence](../../../../../../convergence-of-a-numerical-method.md), although the same order need not hold without the [derivative](../../../../../../derivative.md) bounds used above.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
