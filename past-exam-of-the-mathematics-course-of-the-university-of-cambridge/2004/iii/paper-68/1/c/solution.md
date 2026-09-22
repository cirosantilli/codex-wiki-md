<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The centripetal acceleration of the purely rotating [barotropic fluid](../../../../../../barotropic-fluid.md) is $-r\Omega^2\mathbf e_r$. For $p=K\rho^2$, the pressure force satisfies $\rho^{-1}\nabla p=2K\nabla\rho$, so its [barotropic enthalpy function](../../../../../../barotropic-enthalpy-function.md) is $w=2K\rho$. The equilibrium equation is therefore

$$
\nabla(w+\Phi)=r\Omega^2(r,z)\mathbf e_r.
$$

Taking its curl gives $\partial_z(r\Omega^2)=0$. Thus $\Omega^2$ is independent of z; for a continuous, consistently signed rotation law, so is $\Omega$. This proves the [barotropic cylindrical rotation theorem](../../../../../../barotropic-cylindrical-rotation-theorem.md). Integrating the remaining radial force yields

$$
\boxed{2K\rho+\Phi_3=C,\qquad\Phi_3=\Phi-\int r\Omega^2(r)\,dr.}
$$

The constant C is common to a connected fluid region.

Interpret the semi-thickness as a free surface with $\rho(r,\pm H)=0$, taking the exterior pressure to be negligible. At $H=\epsilon r$, the [gravitational potential](../../../../../../newtonian-potential-of-a-point-mass.md) on this surface is $\Phi_s=-GM/[r\sqrt{1+\epsilon^2}]$. The first integral evaluated at the surface says $C=\Phi_s(r)-\int r\Omega^2dr$. Differentiating along it gives

$$
0=\frac{GM}{r^2\sqrt{1+\epsilon^2}}-r\Omega^2,
$$

and therefore **$\boxed{\Omega^2=(1+\epsilon^2)^{-1/2}GM/r^3}$**. Radial pressure support makes this slightly slower than [Keplerian rotation](../../../../../../keplerian-disk.md) for nonzero thickness.

Subtracting the free-surface first integral from its value inside the disc gives the complete density profile

$$
\rho(r,z)=\frac{GM}{2K}\left[\frac1{\sqrt{r^2+z^2}}-\frac1{r\sqrt{1+\epsilon^2}}\right],\qquad |z|\leq\epsilon r.
$$

It is nonnegative for $K>0$. Integrating over height, with $y=z/r$, gives

$$
\Sigma(r)=\frac{GM}{K}\int_0^\epsilon\left[\frac1{\sqrt{1+y^2}}-\frac1{\sqrt{1+\epsilon^2}}\right]dy=\boxed{\frac{GM}{K}\left[\operatorname{arsinh}\epsilon-\frac{\epsilon}{\sqrt{1+\epsilon^2}}\right]}.
$$

Thus **the [surface density](../../../../../../surface-density-of-a-disk.md) is independent of r** in this [quadratic-polytrope disk with constant aspect ratio](../../../../../../quadratic-polytrope-disk-with-constant-aspect-ratio.md). The factor $1/r$ in density is canceled by the scale r in the vertical extent. The free-surface assumption is essential to this determination; a prescribed nonzero boundary pressure would require its own boundary data. No radial edges are specified, so the formula describes the local equilibrium rather than a finite-mass disc extended to all radii.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
