<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [spherical tensor operator](../../../../spherical-tensor-operator.md) of rank $k$ transforms under [rotation](../../../../rotation-mathematics.md) like an [angular momentum](../../../../angular-momentum.md) $k$. The [Wigner-Eckart theorem](../../../../wigner-eckart-theorem.md) writes its [matrix elements](../../../../matrix-element.md) as

$$
\langle\lambda'j'm'|T_q^{(k)}|\lambda jm\rangle
=\frac{\langle jm;kq|j'm'\rangle}{\sqrt{2j'+1}}\,
\langle\lambda'j'\Vert T^{(k)}\Vert\lambda j\rangle.
$$

The [reduced matrix element](../../../../reduced-matrix-element.md) contains the radial and other dynamical information; the [Clebsch-Gordan coefficients](../../../../clebsch-gordan-coefficients.md) determine the dependence on the projections. Ratios within a fixed pair of multiplets therefore follow without a radial integral. The angular [selection rules](../../../../selection-rule.md) include $m'=m+q$ and $|j-k|\leq j'\leq j+k$.

For the position vector, choose the rank-one components

$$
T_0=z,\qquad T_{\pm1}=\mp\frac{x\pm iy}{\sqrt2},\qquad
x=\frac{T_{-1}-T_{+1}}{\sqrt2}.
$$

Let $R=\langle\lambda',3/2\Vert T^{(1)}\Vert\lambda,1/2\rangle$. The stretched [Clebsch-Gordan coefficients](../../../../clebsch-gordan-coefficients.md) and one lowering step give

$$
\left\langle\frac12,\frac12;1,1\middle|\frac32,\frac32\right\rangle=1,\qquad
\left\langle\frac12,\frac12;1,0\middle|\frac32,\frac12\right\rangle=\sqrt{\frac23}.
$$

For example, apply the total [angular momentum ladder operator](../../../../angular-momentum-ladder-operator.md) to the stretched state. The result has components with coefficients $1/\sqrt3$ and $\sqrt{2/3}$, corresponding to lowering the initial [angular momentum](../../../../angular-momentum.md) and the vector component, respectively.

Only the $q=+1$ component of $x$ contributes to $M_1$. The $q=0$ operator $z$ cannot connect the projections in $M_2$, so that [matrix element](../../../../matrix-element.md) vanishes. With the convention above,

$$
M_1=-\frac{R}{2\sqrt2},\qquad M_2=0,\qquad M_3=\frac{R}{\sqrt6}.
$$

Thus the requested relative magnitudes and their squared values are

$$
\boxed{|M_1|:|M_2|:|M_3|=\sqrt3:0:2},\qquad
\boxed{|M_1|^2:|M_2|^2:|M_3|^2=3:0:4}.
$$

These ratios presume a common nonzero [reduced matrix element](../../../../reduced-matrix-element.md). The position operator has odd [parity](../../../../parity.md), so an [electric dipole transition](../../../../electric-dipole-transition.md) requires opposite-parity multiplets; for one [electron](../../../../electron.md) the [electric-dipole selection rule](../../../../electric-dipole-selection-rule.md) also gives $\Delta\ell=\pm1$. The displayed $j,m$ labels alone do not establish that condition. If the common [reduced matrix element](../../../../reduced-matrix-element.md) vanishes, all three [matrix elements](../../../../matrix-element.md) vanish and no nonzero ratio can be inferred.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Physics course of the University of Cambridge](../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
