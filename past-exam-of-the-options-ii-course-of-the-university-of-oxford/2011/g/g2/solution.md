<h1 id="g/g2/solution">Solution</h1>

↑ **Parent:** [G2](../g2.md)

For a regular [isoperimetric constraint](../../../../isoperimetric-constraint.md), introduce a constant [Lagrange multiplier](../../../../lagrange-multiplier.md) $\lambda$ and set $L=F-\lambda G$. With fixed endpoint values, the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) is

$$
\boxed{L_y-\frac d{dx}L_{y'}=0.}
$$

If $F$ and $G$ have no explicit $x$ dependence, the [Beltrami identity](../../../../beltrami-identity.md) gives the [first integral](../../../../first-integral.md)

$$
L-y'L_{y'}=\text{constant}.
$$

The regularity assumption excludes the exceptional case in which the constraint itself has zero [first variation](../../../../first-variation.md) for every admissible perturbation.

Parametrize the [surface of revolution](../../../../surface-of-revolution.md) by $r(z,\theta)=(f(z)\cos\theta,f(z)\sin\theta,z)$. The magnitude of $r_z\times r_\theta$ is $f\sqrt{1+f'^2}$. Integrating the resulting [surface area](../../../../surface-area.md) element over $\theta$, and integrating the circular cross-sectional areas for the [volume](../../../../volume.md), gives

$$
A=2\pi\int_a^b f\sqrt{1+f'^2}\,dz,
\qquad V=\pi\int_a^b f^2\,dz.
$$

Here $f\geq0$ because it is a radius. For a regular connected closed surface, take $f>0$ in the interior; the closing endpoints can have unbounded $f'$ even when the surface itself is smooth.

After dividing $A-\lambda V$ by $\pi$, its integrand is $L=2f\sqrt{1+f'^2}-\lambda f^2$. The [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) and [Beltrami identity](../../../../beltrami-identity.md) become

$$
\sqrt{1+f'^2}-\lambda f-
\frac d{dz}\left(\frac{ff'}{\sqrt{1+f'^2}}\right)=0,
\qquad
\frac{2f}{\sqrt{1+f'^2}}-\lambda f^2=C.
$$

As $f$ tends to zero at an endpoint, $0\leq2f/\sqrt{1+f'^2}\leq2f$ also tends to zero, so $C=0$. On the positive interior this implies $\lambda>0$ and, writing $R=2/\lambda$,

$$
1+f'^2=\frac{R^2}{f^2}.
$$

The [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) also yields $f''=-R^2/f^3$. Therefore

$$
(f^2)''=2(f'^2+ff'')=-2,
$$

including at the maximum where $f'=0$. Integrating and using the [first integral](../../../../first-integral.md) gives

$$
f(z)^2=R^2-(z-z_0)^2.
$$

Thus the regular extremal is a [sphere](../../../../sphere.md). The two zeros fix its center and radius:

$$
\boxed{z_0=\frac{a+b}2,\qquad R=\frac{b-a}2,\qquad\lambda=\frac2R=\frac4{b-a}.}
$$

Equivalently, the prescribed [volume](../../../../volume.md) fixes $R=(3V/(4\pi))^{1/3}$. If $a,b$ are fixed in advance, their separation and the prescribed [volume](../../../../volume.md) must be compatible with these equations; there is no positive regular stationary profile of the stated type for an incompatible [volume](../../../../volume.md).

For minimality, the three-dimensional [isoperimetric inequality](../../../../isoperimetric-inequality.md) states that every sufficiently regular closed surface enclosing [volume](../../../../volume.md) $V$ has

$$
A^3\geq36\pi V^2,
$$

with equality precisely for a [sphere](../../../../sphere.md). Our extremal has $A=4\pi R^2$ and $V=4\pi R^3/3$, so it attains equality and is a **global minimum of area at the fixed [volume](../../../../volume.md)**. This also makes clear the connected-surface assumption behind uniqueness: allowing several disconnected components introduces stationary collections of spheres, rather than the single positive generating profile used here.

## ↑ Ancestors (12)

1. [G2](../g2.md)
2. [G](../../g.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
