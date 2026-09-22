<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

**Reduced radial equation.** A [spherical harmonic](../../../../../spherical-harmonic.md) satisfies $\widehat L^2Y_{\ell m}=\ell(\ell+1)\hbar^2Y_{\ell m}$. Substitute $\psi=RY_{\ell m}$ into the [time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md), divide out the angular function, and put $R=U/r$. Direct differentiation gives

$$
r^2R'=rU'-U,\qquad
\frac1{r^2}(r^2R')'=\frac{U''}{r}.
$$

Multiplication by $r$ then gives the [Radial Schrodinger equation](../../../../../radial-schrodinger-equation-for-the-hydrogen-atom.md)

$$
\boxed{-\frac{\hbar^2}{2\mu}U''+
\frac{\ell(\ell+1)\hbar^2}{2\mu r^2}U+V(r)U=EU.}
$$

Here $\mu=m_1m_2/(m_1+m_2)$ is the [reduced mass](../../../../../reduced-mass.md), and the extra positive term is the [centrifugal potential](../../../../../centrifugal-potential.md).

**Boundary conditions.** At the origin this finite central potential has no point interaction. The physical radial solution is regular there, requiring $U(0)=0$; for $\ell=0$, a nonzero constant $U(0)$ would give $R\sim1/r$ and a point-source singularity of the three-dimensional [Laplacian](../../../../../laplacian.md). Mere square integrability alone would not remove that singular solution. For a [bound state](../../../../../bound-state.md), the radial [probability](../../../../../probability.md) integral is $\int_0^\infty |U|^2dr$, so the exterior solution must decay and $U(r)\to0$ as $r\to\infty$.

**Solutions for zero [orbital angular momentum](../../../../../orbital-angular-momentum.md).** For $\ell=0$ and $-V_0<E<0$, define

$$
\boxed{k=\frac{\sqrt{2\mu(V_0+E)}}{\hbar},\qquad
q=\frac{\sqrt{-2\mu E}}{\hbar}.}
$$

The interior equation is $U''+k^2U=0$; $U(0)=0$ excludes the cosine. The exterior equation is $U''-q^2U=0$; normalizability excludes the growing exponential. Thus

$$
\boxed{U(r)=\begin{cases}A\sin kr,&0\le r\le a,\\Be^{-qr},&r>a.\end{cases}}
$$

The constants cannot remain independent once the interface is matched. Since the [potential step](../../../../../step-potential.md) is finite, both $U$ and $U'$ are continuous at $a$:

$$
A\sin ka=Be^{-qa},\qquad Ak\cos ka=-qBe^{-qa}.
$$

Dividing the equations yields

$$
\boxed{k\cot ka=-q,\qquad\tan ka=-\frac kq.}
$$

**Existence and number of s-wave bound states.** Put $z=ka$, $y=qa$, and $\rho_0=a\sqrt{2\mu V_0}/\hbar$. Then

$$
z^2+y^2=\rho_0^2,\qquad z\cot z=-y.
$$

The lowest branch lies on $\pi/2<z<\pi$. Along it, $y=-z\cot z>0$ and $\rho_0=z/\sin z$ increases continuously from $\pi/2$ to infinity. Therefore a first negative-energy solution exists precisely when $\rho_0>\pi/2$, or

$$
\boxed{V_0>V_*\equiv\frac{\pi^2\hbar^2}{8\mu a^2}.}
$$

Further branches begin at $z=3\pi/2,5\pi/2,\ldots$ as $q\to0^+$. Hence the [bound-state thresholds of a spherical square well](../../../../../bound-state-thresholds-of-a-spherical-square-well.md) give exactly one negative-energy $\ell=0$ state when

$$
\boxed{\frac{\pi^2\hbar^2}{8\mu a^2}<V_0
\le\frac{9\pi^2\hbar^2}{8\mu a^2}.}
$$

The upper equality is included: the second branch is then only at $E=0$, with constant exterior $U$, and is not normalizable. If threshold cases are excluded by convention, the commonly quoted open interval has a strict upper inequality; the physical negative-energy state count at equality is still one.

**Deuteron estimate.** Using $m_pc^2\simeq938.27\,\mathrm{MeV}$, $m_nc^2\simeq939.57\,\mathrm{MeV}$ and $\hbar c\simeq197.327\,\mathrm{MeV\,fm}$ gives $\mu c^2\simeq469.46\,\mathrm{MeV}$. At $a=2.1\,\mathrm{fm}$,

$$
\boxed{
V_*=\frac{\pi^2(197.327)^2}{8(469.46)(2.1)^2}\,\mathrm{MeV}
=23.2\,\mathrm{MeV},\qquad V_0>23.2\,\mathrm{MeV}.}
$$

The threshold for a second $s$ state is $9V_*\simeq209\,\mathrm{MeV}$, far above the stipulated depth $33.5\,\mathrm{MeV}$. Thus this model has **no radially excited s-wave [bound state](../../../../../bound-state.md)**.

Checking other [orbital angular momentum](../../../../../orbital-angular-momentum.md) sectors matters before ruling out every excitation. At the first $p$-wave threshold, the regular interior reduced radial function is $rj_1(kr)$ and the zero-energy exterior function is proportional to $r^{-1}$. Matching their logarithmic [derivatives](../../../../../derivative.md) requires $j_0(ka)=0$, whose first root is $ka=\pi$. Hence

$$
V_{p,*}=\frac{\pi^2\hbar^2}{2\mu a^2}=4V_*\simeq92.8\,\mathrm{MeV}>33.5\,\mathrm{MeV}.
$$

Larger $\ell$ only increases the [centrifugal potential](../../../../../centrifugal-potential.md). Therefore **no bound orbital excited states are expected in the specified central square-well model**. Its [spin](../../../../../spin.md) dependence and tensor nuclear forces have not been specified; the calculation does not resolve the real deuteron's internal [spin](../../../../../spin.md) structure.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
