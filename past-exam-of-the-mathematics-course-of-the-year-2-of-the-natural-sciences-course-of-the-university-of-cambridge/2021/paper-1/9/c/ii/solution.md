<h1 id="9/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The downward drop from the starting rim to angle $\theta$ is $R\cos\theta$. With no dissipative forces, [conservation of energy](../../../../../../conservation-of-energy.md) gives $mv^2/2=mgR\cos\theta$, so $v=\sqrt{2gR\cos\theta}$. Dividing the [line element](../../../../../../line-element.md) by this speed yields

$$
\boxed{T[z]=\frac1{\sqrt{2gR}}\int_{-\pi/2}^{\pi/2}\sqrt{\frac{R^2+z'^2}{\cos\theta}}\,d\theta.}
$$

The endpoint singularities are integrable for the minimizing path. The integrand is independent of $z$; its [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) gives a constant $K$, after absorbing the overall prefactor:

$$
\frac{z'}{\sqrt{\cos\theta}\sqrt{R^2+z'^2}}=K.
$$

Solving for $z'$ and taking the positive branch required by $z_2>z_1$ gives

$$
\boxed{\frac{dz}{d\theta}=\frac{RK\sqrt{\cos\theta}}{\sqrt{1-K^2\cos\theta}},\qquad0<K<1.}
$$

The constant is fixed implicitly by

$$
z_2-z_1=RK\int_{-\pi/2}^{\pi/2}\frac{\sqrt{\cos\theta}}{\sqrt{1-K^2\cos\theta}}\,d\theta.
$$

This integral is strictly increasing from zero to infinity as $K$ increases from zero to one, so every finite positive separation selects a unique $K$. The time integrand has second [derivative](../../../../../../derivative.md) $R^2/[\sqrt{\cos\theta}(R^2+z'^2)^{3/2}]>0$ with respect to $z'$. Its supporting-line inequality, integrated between fixed endpoints with constant first [derivative](../../../../../../derivative.md) with respect to $z'$, proves this stationary path is the unique [global minimum](../../../../../../global-minimum.md) within the stated single-valued class.

As $\theta\downarrow-\pi/2$, $z'\to0$. Therefore the skater should initially head **directly down the curved ramp, perpendicular to the cylinder axis**, and gain axial motion later. The path differs from the constant-pitch shortest route because extra distance is cheaper in time near the faster, lower part of the ramp. This is the [brachistochrone on a horizontal half-cylinder](../../../../../../brachistochrone-on-a-horizontal-half-cylinder.md).

<a id="9/c/ii/image-shortest-and-fastest-routes-on-the-unrolled-half-cylinder-for-z-2-z-1-2r"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1-half-cylinder-paths.png)

**[Figure 1](#9/c/ii/image-shortest-and-fastest-routes-on-the-unrolled-half-cylinder-for-z-2-z-1-2r). Shortest and fastest routes on the unrolled half-cylinder for $z_2-z_1=2R$**.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [9](../../../9.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
