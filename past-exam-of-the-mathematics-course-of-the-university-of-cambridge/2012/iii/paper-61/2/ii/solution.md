<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The steady incompressible [shearing sheet](../../../../../../shearing-sheet.md) equation is

$$
\mathbf u\cdot\nabla\mathbf u+2\Omega\mathbf e_z\times\mathbf u=-\rho^{-1}\nabla p+2\Omega Sx\mathbf e_x.
$$

The final term follows from the local tidal potential $-\Omega Sx^2$. For the given linear velocity, the advective acceleration is $-\alpha\beta(x\mathbf e_x+y\mathbf e_y)$, while the [Coriolis acceleration](../../../../../../coriolis-acceleration.md) is $2\Omega\beta x\mathbf e_x+2\Omega\alpha y\mathbf e_y$. Equating components gives

$$
\frac{p_x}\rho=[\alpha\beta+2\Omega(S-\beta)]x,\qquad\frac{p_y}\rho=\alpha(\beta-2\Omega)y.
$$

The cross derivatives vanish, so the [pressure Hessian of an elliptical shearing-sheet vortex](../../../../../../pressure-hessian-of-an-elliptical-shearing-sheet-vortex.md) integrates to

$$
\boxed{\frac p\rho=\frac12Ax^2+\frac12By^2+\text{constant},\quad A=\frac{S^2}{(r-1)^2}-\frac{2\Omega S}{r-1},\quad B=\frac{S^2}{(r-1)^2}-\frac{2\Omega S}{r(r-1)}.}
$$

The additive constant is fixed by exterior matching or the [pressure](../../../../../../pressure.md) reference. No zero-pressure free-boundary condition is imposed on an incompressible vortex patch: it is embedded in a surrounding fluid.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
