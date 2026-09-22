<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

**Images and uniqueness.** The [method of images](../../../../../method-of-images.md) replaces a conducting boundary by fictitious charges outside the physical field region. Choose them so that the resulting [electric potential](../../../../../electric-potential.md) satisfies the required conductor potentials. The [Uniqueness of the Dirichlet problem](../../../../../uniqueness-of-the-dirichlet-problem.md) then guarantees the same physical exterior field. For example, a point charge $q$ at height $h$ above a grounded plane has an image $-q$ at height $-h$: the plane is an equipotential at zero, and the charge is attracted toward it by $q^2/(16\pi\varepsilon_0h^2)$. The image is a computational device; the physical conductor carries a continuous induced [surface charge density](../../../../../surface-charge-density.md).

**Potential of a line.** Surround an infinite [line charge](../../../../../line-charge.md) $\lambda$ by a coaxial Gaussian cylinder of radius $r$ and length $L$. [Gauss's law](../../../../../gauss-s-law.md) gives $E_r(2\pi rL)=\lambda L/\varepsilon_0$, hence $E_r=\lambda/(2\pi\varepsilon_0r)$. Integrating $E_r=-dV/dr$ gives

$$
\boxed{V(r)-V(r_0)=-\frac\lambda{2\pi\varepsilon_0}\ln\frac r{r_0}.}
$$

Writing an additive constant instead is equivalent. The reference length makes the logarithm dimensionless; an isolated infinite line cannot be assigned a finite zero potential at infinity.

**Locating the two lines.** Put the grounded plane at $x=0$ and the physical cylinder at $(x,y)=(d,0)$, with axis along $z$ and radius $a<d$. Set $c=\sqrt{d^2-a^2}$, and place [line charges](../../../../../line-charge.md) $+\lambda$ and $-\lambda$ at $(c,0)$ and $(-c,0)$. If $R_+$ and $R_-$ are their distances from an observation point, the [cylinder-plane image charges](../../../../../cylinder-plane-image-charges.md) give

$$
V(x,y)=\frac\lambda{2\pi\varepsilon_0}\ln\frac{R_-}{R_+},
\quad R_\pm^2=(x\mp c)^2+y^2.
$$

On $x=0$, $R_-=R_+$, so $V=0$. To check the cylinder, define $q=(d+c)/a$. The level set $R_-=qR_+$ is a circle: completing the square gives

$$
\left(x-c\frac{q^2+1}{q^2-1}\right)^2+y^2
=\left(\frac{2cq}{q^2-1}\right)^2.
$$

Since $d^2-c^2=a^2$, its centre is $d$ and radius is $a$. The positive line lies inside the cylinder; the negative line lies behind the plane. There is consequently no fictitious charge in the exterior physical region. A Gaussian contour around the cylinder encloses $+\lambda$ only, so the required physical charge per unit length is also correct. These boundary conditions and the far-field behaviour determine the physical solution by [Uniqueness of the Dirichlet problem](../../../../../uniqueness-of-the-dirichlet-problem.md).

**Cylinder voltage.** The constant distance ratio on the cylinder immediately gives

$$
\boxed{V_c=\frac\lambda{2\pi\varepsilon_0}
\ln\frac{d+\sqrt{d^2-a^2}}a
=\frac\lambda{2\pi\varepsilon_0}\operatorname{arcosh}\frac da.}
$$

Its [capacitance per unit length](../../../../../capacitance-per-unit-length.md) is $C'=2\pi\varepsilon_0/\operatorname{arcosh}(d/a)$. In the thin-cable limit, $\operatorname{arcosh}(d/a)\simeq\ln(2d/a)$.

**Cable attraction.** Because the cable is idealized as infinite, the meaningful answer is [force](../../../../../force-split.md) per unit length. For $a=0.020\ \mathrm m$, centre height $d\simeq10\ \mathrm m$ and $V_c=1.1\times10^4\ \mathrm V$,

$$
\lambda=\frac{2\pi\varepsilon_0V_c}{\operatorname{arcosh}(500)}
\simeq8.86\times10^{-8}\ \mathrm{C\,m^{-1}}.
$$

The [electrostatic attraction per unit length of a cylinder above a plane](../../../../../electrostatic-attraction-per-unit-length-of-a-cylinder-above-a-plane.md) is

$$
\boxed{f=\frac{\lambda^2}{4\pi\varepsilon_0\sqrt{d^2-a^2}}
\simeq7.05\times10^{-6}\ \mathrm{N\,m^{-1}},\qquad\text{downward}.}
$$

For example, this follows without any ambiguity about moving image positions from $F_d=\tfrac12V_c^2\,dC'/dd$ at fixed voltage, including the work of the voltage source. Its sign is negative because [capacitance](../../../../../capacitance.md) decreases with height. A cable length $L$ experiences approximately $fL$ downward when end effects are negligible. This is the electrostatic contribution only.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
