<h1 id="15c/solution">Solution</h1>

↑ **Parent:** [15C](../15c.md)

For constant density, divide the incompressible [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) by $\rho$. The vector identity $(\mathbf u\cdot\nabla)\mathbf u=\nabla(|\mathbf u|^2/2)-\mathbf u\times\boldsymbol\omega$ converts them into $\partial_t\mathbf u=\mathbf u\times\boldsymbol\omega-\nabla(p/\rho+|\mathbf u|^2/2)$. Taking the [curl](../../../../../curl.md) eliminates the gradient. Expand the curl of the cross product, use $\nabla\cdot\mathbf u=0$ and $\nabla\cdot\boldsymbol\omega=0$, and obtain

$$
\partial_t\boldsymbol\omega=(\boldsymbol\omega\cdot\nabla)\mathbf u-(\mathbf u\cdot\nabla)\boldsymbol\omega,\qquad\boxed{\frac{D\boldsymbol\omega}{Dt}=(\boldsymbol\omega\cdot\nabla)\mathbf u.}
$$

This is the [vorticity equation](../../../../../vorticity-equation.md), including [vortex stretching](../../../../../vortex-stretching.md). Without constant density there would in general be an additional baroclinic term; the displayed source equations use the constant-density interpretation.

For the specified velocity, direct differentiation gives $\boldsymbol\omega=2\Omega(t)\mathbf k$. It is spatially uniform, while $(\boldsymbol\omega\cdot\nabla)\mathbf u=2\beta\boldsymbol\omega$. Thus $\Omega'=2\beta\Omega$ and

$$
\boxed{\boldsymbol\omega=2\Omega(0)e^{2\beta t}\mathbf k.}
$$

If the positive $z$ direction agrees with the initial vorticity, $2\Omega(0)=\omega_0$ as written in the question. For opposite rotation the initial component is signed and the vector has the corresponding minus sign.

For a material particle, $d(x^2+y^2)/dt=2x(-\beta x-\Omega y)+2y(-\beta y+\Omega x)=-2\beta(x^2+y^2)$, while $dz/dt=2\beta z$. The initial material circle therefore evolves into

$$
\boxed{a(t)=e^{-\beta t},\qquad x^2+y^2=a(t)^2,\qquad z=e^{2\beta t}=a(t)^{-2}.}
$$

The azimuthal rotation changes the labels of points on the circle but not the circle as a set. Its counterclockwise [circulation](../../../../../circulation-physics.md), viewed from positive $z$, is

$$
\Gamma=\oint\mathbf u\cdot d\mathbf r=2\pi\Omega(t)a(t)^2=2\pi\Omega(0)=\pi\omega_0
$$

for the positive-orientation convention. The strain contributes no tangential velocity. Thus **circulation stays constant although vorticity grows and the enclosed material area shrinks**, illustrating [Kelvin's circulation theorem](../../../../../kelvin-s-circulation-theorem.md) for a material loop in constant-density inviscid flow with no nonconservative body force.

## ↑ Ancestors (10)

1. [15C](../15c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
