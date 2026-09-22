<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Start from the constant-coefficient [mean-field dynamo](../../../../../../mean-field-dynamo.md) equation

$$
\partial_t\overline B=\nabla\times(U\times\overline B+\alpha\overline B)+\eta\nabla^2\overline B.
$$

Here $\eta$ may include turbulent as well as microscopic diffusion. Use a local Cartesian model, neglect meridional circulation and curvature, and assume independence of $y$. Represent the [poloidal magnetic field](../../../../../../poloidal-magnetic-field.md) by a vector potential along $y$ and the [toroidal magnetic field](../../../../../../toroidal-magnetic-field.md) by its $y$ component:

$$
\overline B=\nabla\times(A\hat y)+B\hat y=(-A_z,B,A_x),\qquad U=\Omega z\hat y.
$$

The shear contributes $(\overline B\cdot\nabla)U=\Omega A_x\hat y$. The poloidal part of $\alpha\nabla\times(B\hat y)$ gives $A_t=\alpha B+\eta\nabla^2A$, while the toroidal part of $\alpha\nabla\times\overline B_{\rm pol}$ is $-\alpha\nabla^2A$. Therefore

$$
B_t=\Omega A_x-\alpha\nabla^2A+\eta\nabla^2B.
$$

Retaining one common transverse dependence $e^{i\ell z}$ changes $\nabla^2$ to $\partial_x^2-\ell^2$, producing the two requested equations. The first coupling is the [alpha effect](../../../../../../alpha-effect.md) regenerating poloidal field from toroidal field; the shear is differential-rotation winding in an [Alpha-Omega dynamo](../../../../../../alpha-omega-dynamo.md). Retaining the alpha contribution in the second equation also allows [alpha-squared dynamo](../../../../../../alpha-squared-dynamo.md) feedback, rather than making the pure Parker shear-dominated approximation.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
