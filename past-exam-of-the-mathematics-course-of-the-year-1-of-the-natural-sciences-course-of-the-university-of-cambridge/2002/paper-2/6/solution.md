<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Compute the [curl](../../../../curl.md) component by component from the given [vector field](../../../../vector-field.md):

$$
\boxed{B=\nabla\times A=(2xz,\ 2yz,\ 2(1-z^2)).}
$$

For example, $B_x=\partial_y A_z-\partial_z A_y=0-(-2xz)$ and $B_z=\partial_x A_y-\partial_y A_x=(1-z^2)-(z^2-1)$. Its [divergence](../../../../divergence.md) is

$$
\boxed{\nabla\cdot B=2z+2z-4z=0,}
$$

as expected because the [divergence of a curl is zero](../../../../divergence-of-a-curl-is-zero.md).

Take $C$ counterclockwise when viewed from positive $z$, the [disc](../../../../topological-disc.md) $D$ upward oriented, and the [hemisphere](../../../../hemisphere.md) $H$ outward oriented. These choices give both [surfaces](../../../../topological-surface-split.md) the same positive boundary orientation. Parametrize $C$ by $r(t)=(\cos t,\sin t,0)$, $0\leq t\leq2\pi$. On it, $A=(-\sin t,\cos t,0)$ and $dr=(-\sin t,\cos t,0)\,dt$, so the [line integral](../../../../line-integral.md) is

$$
\boxed{\oint_C A\cdot dr=\int_0^{2\pi}1\,dt=2\pi.}
$$

On $D$, use [polar coordinates](../../../../polar-coordinates.md) $(x,y)=(r\cos\phi,r\sin\phi)$ and $d\mathbf S=(0,0,1)r\,dr\,d\phi$. Since $B_z=2$ there, the [surface flux](../../../../flux-integral.md) is

$$
\boxed{\int_D B\cdot d\mathbf S=\int_0^{2\pi}\int_0^1 2r\,dr\,d\phi=2\pi.}
$$

On the unit [hemisphere](../../../../hemisphere.md), the outward [unit normal vector](../../../../unit-normal.md) is $n=(x,y,z)$. Since $x^2+y^2=1-z^2$, we have $B\cdot n=4z(1-z^2)$. In [spherical polar coordinates](../../../../spherical-coordinate-system.md), $z=\cos\theta$ and $dS=\sin\theta\,d\theta\,d\phi$, giving the explicit [surface integral](../../../../surface-integral.md)

$$
\boxed{\int_H B\cdot d\mathbf S=\int_0^{2\pi}\int_0^{\pi/2}4\cos\theta\sin^3\theta\,d\theta\,d\phi=2\pi.}
$$

Indeed the inner [integral](../../../../integral-split.md) is $[\sin^4\theta]_0^{\pi/2}=1$.

These equalities illustrate [Stokes theorem](../../../../stokes-theorem.md) twice: $B=\nabla\times A$ and either upward $D$ or outward $H$ spans the oriented [circle](../../../../circle.md) $C$, so each [surface flux](../../../../flux-integral.md) equals the same [line integral](../../../../line-integral.md). For the [divergence theorem](../../../../divergence-theorem.md), close the upper half-ball by adjoining the downward oriented base, namely $-D$. Its outward [surface flux](../../../../flux-integral.md) is

$$
\int_{H\cup(-D)}B\cdot d\mathbf S=2\pi-2\pi=0=\int_V\nabla\cdot B\,dV.
$$

The minus sign on the base is required because its outward [normal vector](../../../../normal-vector.md) points down. Reversing a specified orientation reverses that integral's sign.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
