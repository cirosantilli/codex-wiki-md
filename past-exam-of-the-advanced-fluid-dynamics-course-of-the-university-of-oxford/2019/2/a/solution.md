<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work in the laboratory frame, with the fluid at rest at infinity. Set

$$
f(r)=\frac{3a}{4r}+\frac{a^3}{4r^3},\qquad
g(r)=\frac{3a}{4r^3}-\frac{3a^3}{4r^5},
\qquad \mathbf u=f\mathbf U+g(\mathbf U\cdot\mathbf x)\mathbf x.
$$

At $r=a$, $f=1$ and $g=0$, so the [no-slip boundary condition](../../../../no-slip-boundary-condition.md) is $\mathbf u=\mathbf U$ on the translating [sphere](../../../../sphere.md). As $r\to\infty$, $\mathbf u=O(r^{-1})\to0$ and the gauge-fixed [pressure](../../../../pressure-split.md) tends to zero.

It is also possible to check the exterior [Stokes equations](../../../../stokes-equation.md) directly. Differentiating the radial functions gives

$$
\nabla\cdot\mathbf u
=(\mathbf U\cdot\mathbf x)\left(\frac{f'}r+rg'+4g\right)=0,
$$

and

$$
\begin{aligned}
\nabla^2\mathbf u
&=\left(f''+\frac{2f'}r+2g\right)\mathbf U
+\left(g''+\frac{6g'}r\right)(\mathbf U\cdot\mathbf x)\mathbf x\\
&=\frac{3a}{2}\left(\frac{\mathbf U}{r^3}
-\frac{3(\mathbf U\cdot\mathbf x)\mathbf x}{r^5}\right)
=\frac{\nabla p}{\mu}.
\end{aligned}
$$

Thus the [Newtonian fluid stress tensor](../../../../newtonian-fluid-stress-tensor.md) $\sigma=-pI+\mu(\nabla\mathbf u+\nabla\mathbf u^T)$ satisfies $\nabla\cdot\sigma=0$ throughout $r>a$.

Let $\mathbf n$ point away from the common centre on each concentric [sphere](../../../../sphere.md). Applying the [divergence theorem](../../../../divergence-theorem.md) to the intervening fluid shell, whose inner normal is $-\mathbf n$, yields

$$
\boxed{\mathbf F_{\rm drag}
=\int_{r=a}\sigma\mathbf n\,dS
=\int_{r=R}\sigma\mathbf n\,dS,\qquad R>a.}
$$

This is the [force flux at infinity in Stokes flow](../../../../force-flux-at-infinity-in-stokes-flow.md). It is legitimate even though the [stress tensor](../../../../cauchy-stress-tensor.md) tends to zero pointwise, because the area of the large [sphere](../../../../sphere.md) grows as $R^2$.

For an explicit evaluation, put $A=3a/4$ and $\mathbf n=\mathbf x/R$. The leading terms are $\mathbf u=A[\mathbf U+(\mathbf U\cdot\mathbf n)\mathbf n]/R$ and $p=2\mu A(\mathbf U\cdot\mathbf n)/R^2$. Their [velocity gradient](../../../../velocity-gradient.md) is

$$
\partial_j u_i
=\frac{A}{R^2}\left[-U_i n_j+U_j n_i
+(\mathbf U\cdot\mathbf n)\delta_{ij}
-3(\mathbf U\cdot\mathbf n)n_i n_j\right]
+O\!\left(\frac{a^3|\mathbf U|}{R^4}\right).
$$

After symmetrizing and subtracting the [pressure](../../../../pressure-split.md) contribution,

$$
\sigma\mathbf n
=-\frac{9\mu a}{2R^2}(\mathbf U\cdot\mathbf n)\mathbf n
+O\!\left(\frac{\mu a^3|\mathbf U|}{R^4}\right).
$$

By [rotational symmetry](../../../../rotational-symmetry.md), $\int n_i n_j\,d\Omega=(4\pi/3)\delta_{ij}$. Hence

$$
\mathbf F_{\rm drag}
=-\frac{9\mu a}{2}\int(\mathbf U\cdot\mathbf n)\mathbf n\,d\Omega
=\boxed{-6\pi\mu a\mathbf U}.
$$

This is [Stokes's law](../../../../stokes-s-law.md), with the [force](../../../../force-split.md) on the [sphere](../../../../sphere.md) opposite its [velocity](../../../../velocity.md). For a component calculation with $\mathbf U=U\mathbf e_z$, the same integral is $F_z=-(9\mu aU/2)\int\cos^2\theta\,d\Omega$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
