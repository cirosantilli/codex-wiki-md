<h1 id="10c/solution">Solution</h1>

↑ **Parent:** [10C](../10c.md)

The [Stokes theorem](../../../../../stokes-theorem.md) states

$$
\int_S(\nabla\times\mathbf F)\cdot\mathbf n\,dS
=\oint_{\partial S}\mathbf F\cdot d\mathbf r,
$$

where the boundary orientation is induced by the chosen normal through the right-hand rule.

For $\mathbf F=(y^2z,xz+2xyz,0)$,

$$
\boxed{\nabla\times\mathbf F=(-x-2xy,\ y^2,\ z),}
$$

and its divergence is $(-1-2y)+2y+1=0$, verifying $\nabla\cdot(\nabla\times\mathbf F)=0$.

Orient the paraboloid $z=3-x^2-y^2$, $1\leq x^2+y^2\leq4$, upward and the planar annulus $z=-1$ downward. Their outer boundary orientations cancel. The remaining boundary is the unit circle at $z=-1$ counterclockwise and the unit circle at $z=2$ clockwise, viewed from above. On a unit circle at height $z_0$, direct parametrization gives

$$
\oint_{\rm CCW}\mathbf F\cdot d\mathbf r=\pi z_0.
$$

Hence the boundary integral is $-\pi-2\pi=-3\pi$.

On the lower annulus, $(\nabla\times\mathbf F)\cdot(0,0,-1)=1$, giving $3\pi$. On the paraboloid, $d\mathbf S=(2x,2y,1)\,dx\,dy$, so the flux integrand is

$$
-2x^2-4x^2y+2y^3+3-r^2.
$$

The odd terms integrate to zero over the annulus, while the rest integrates to $-6\pi$. The total surface integral is $3\pi-6\pi=-3\pi$, equal to the boundary integral.

## ↑ Ancestors (10)

1. [10C](../10c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
