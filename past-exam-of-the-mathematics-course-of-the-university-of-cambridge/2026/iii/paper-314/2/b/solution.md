<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Linearize the inviscid momentum equation in the uniformly rotating frame. The [Coriolis acceleration](../../../../../../coriolis-acceleration.md) is $2\boldsymbol\Omega\times\delta\mathbf u$, and the equilibrium pressure gradient cancels gravity. For perturbations proportional to $e^{ik_xx-i\omega t}$, the horizontal components are

$$
-i\omega\rho\,\delta u_x-2\Omega\rho\,\delta u_y
=-ik_x\delta p,
$$



$$
-i\omega\rho\,\delta u_y+2\Omega\rho\,\delta u_x=0.
$$

The vertical component is

$$
-i\omega\rho\,\delta u_z
=-g\delta\rho-\frac{d\delta p}{dz}.
$$

Linearizing mass conservation,

$$
\partial_t\delta\rho+\nabla\mathbin\cdot(\rho\delta\mathbf u)=0,
$$

gives

$$
-i\omega\delta\rho+\delta u_z\frac{d\rho}{dz}
=-\rho\left(ik_x\delta u_x+\frac{d\delta u_z}{dz}\right).
$$

Finally, linearizing the adiabatic pressure equation gives

$$
-i\omega\delta p+\delta u_z\frac{dp}{dz}
=-\gamma p\left(ik_x\delta u_x+\frac{d\delta u_z}{dz}\right).
$$

These are the stated five equations. Self-gravity contributes no perturbation because it is neglected, and the equilibrium centrifugal term has already been absorbed or omitted.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
