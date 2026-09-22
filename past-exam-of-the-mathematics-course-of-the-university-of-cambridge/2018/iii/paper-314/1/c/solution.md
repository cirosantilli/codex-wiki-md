<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Expanding the [kinetic helicity conservation law](../../../../../../kinetic-helicity-conservation-law.md) separates [advection](../../../../../../advection.md) from the other flux:

$$
\boxed{\frac{Dq}{Dt}=\boldsymbol\omega\cdot\nabla\left(\frac{u^2}{2}-w\right)-q\nabla\cdot\mathbf u.}
$$

Thus [material conservation of kinetic helicity density](../../../../../../material-conservation-of-kinetic-helicity-density.md) holds precisely when

$$
\boxed{\boldsymbol\omega\cdot\nabla\left(\frac{u^2}{2}-w\right)=q\nabla\cdot\mathbf u.}
$$

An especially useful sufficient pair of conditions is [incompressible flow](../../../../../../incompressible-flow.md), $\nabla\cdot\mathbf u=0$, and constancy of $w-u^2/2$ along integral curves of the [vorticity](../../../../../../vorticity.md), $\boldsymbol\omega\cdot\nabla(w-u^2/2)=0$. Together these conditions make both terms vanish without cancellation. They are not necessary individually, because the two terms in the displayed balance can cancel. An [irrotational flow](../../../../../../irrotational-flow.md) is a trivial conserved case with $q=0$.

For contrast, combining the balance with [mass conservation](../../../../../../mass-conservation.md) gives

$$
\frac D{Dt}\left(\frac q\rho\right)=-\frac{\boldsymbol\omega}{\rho}\cdot\nabla\left(w-\frac{u^2}{2}\right).
$$

Consequently constancy of $w-u^2/2$ along integral curves of the [vorticity](../../../../../../vorticity.md) makes $q/\rho$ an advected scalar even in [compressible flow](../../../../../../compressible-flow-split.md); it does not generally make $q$ itself constant.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
