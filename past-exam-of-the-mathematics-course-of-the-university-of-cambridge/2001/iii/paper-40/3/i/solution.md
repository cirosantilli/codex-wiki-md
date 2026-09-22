<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [gravitational acceleration](../../../../../../gravitational-acceleration.md) $\mathbf g=\nabla\psi$. Through the plane with upward unit normal, the signed gravitational flux per unit area of the point mass is

$$
g_z(R,0)=\left.\partial_z\psi\right|_{z=0}=-\frac{Gmb}{(R^2+b^2)^{3/2}}.
$$

Thus its downward flux magnitude is $Gmb/(R^2+b^2)^{3/2}$. Subtracting a constant from the [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md) does not change this flux.

The [Kuzmin reflection method](../../../../../../kuzmin-reflection-method.md) gives the even [relative potential](../../../../../../relative-potential.md) $\psi=Gm/\sqrt{R^2+(|z|+b)^2}$. It is harmonic above and below the plane because the corresponding point masses lie outside the respective half-spaces. At the plane the derivative jump is

$$
\partial_z\psi(R,0^+)-\partial_z\psi(R,0^-)
=-\frac{2Gmb}{(R^2+b^2)^{3/2}}.
$$

Integrating the [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) $\nabla^2\psi=-4\pi G\Sigma(R)\delta(z)$ through a thin layer, with $\delta$ the [Dirac delta](../../../../../../dirac-delta-function.md), equates this jump to $-4\pi G\Sigma$. Therefore

$$
\boxed{\Sigma(R)=\frac{mb}{2\pi(R^2+b^2)^{3/2}}.}
$$

This is a [Kuzmin disk](../../../../../../kuzmin-disk.md). As a check, its total [mass](../../../../../../mass.md) is $2\pi\int_0^\infty R\Sigma(R)\,dR=m$.

Replace the point mass by $dm=\mu(b)\,db$ and superpose the [Kuzmin disks](../../../../../../kuzmin-disk.md). Linearity of the [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md) gives, whenever the force integral converges,

$$
\boxed{\Sigma(R)=\frac1{2\pi}\int_0^\infty\frac{b\mu(b)}{(R^2+b^2)^{3/2}}\,db.}
$$

Both choices of potential reference give this same [surface density](../../../../../../surface-density-of-a-disk.md). If the unreferenced potential diverges, perform the reference subtraction in each component before taking the integral limit; the force and the [surface density](../../../../../../surface-density-of-a-disk.md) may still be finite.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
