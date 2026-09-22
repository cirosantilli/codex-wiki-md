<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [toroidal magnetic field](../../../../../../toroidal-magnetic-field.md) introduces an inward hoop force. In [cylindrical coordinates](../../../../../../cylindrical-coordinate-system.md), the radial [magnetic tension](../../../../../../magnetic-tension.md) is $-B_\phi^2/(\mu_0s)$, so [cylindrical magnetostatic pressure balance](../../../../../../cylindrical-magnetostatic-pressure-balance.md) in SI units becomes

$$
P'(s)=-\frac{B_\phi(s)^2}{\mu_0s},\qquad
P=p+\frac{B_z^2+B_\phi^2}{2\mu_0}.
$$

At the field-free boundary $P(s_0)=p_e$. Hence

$$
p(s)+\frac{B_z(s)^2+B_\phi(s)^2}{2\mu_0}
=p_e+\frac1{\mu_0}\int_s^{s_0}\frac{B_\phi(r)^2}{r}\,dr.
$$

Regularity on the axis gives $B_\phi=O(s)$, which makes the integral finite and gives $B_\phi(0)=0$. Evaluating at the axis proves **the central-field identity**:

$$
\boxed{B_z(0)^2=B_p^2-2\mu_0p(0)+2\int_0^{s_0}\frac{B_\phi(s)^2}{s}\,ds.}
$$

The positive hoop-tension contribution allows the central axial field to exceed $B_p$ without negative [pressure](../../../../../../pressure.md). For an explicit regular example, put $x=s^2/s_0^2$, choose a constant $a>0$ and $0<\varepsilon<1$, and take inside the [flux tube](../../../../../../flux-tube.md)

$$
\begin{aligned}
p&=p_e[1-(1-\varepsilon)(1-x)^2],\qquad B_\phi=\sqrt a\,(s/s_0)B_z,\\
B_z^2&=(1-\varepsilon)B_p^2\frac{(1-x)^2[1+a(1+2x)/3]}{(1+ax)^2}.
\end{aligned}
$$

Substitution verifies the radial balance, with continuous zero field at $s=s_0$ and positive gas [pressure](../../../../../../pressure.md). For $a=3$, $\varepsilon=1/4$, the central value is $B_z(0)^2=3B_p^2/2$.

To obtain the cross-sectional average, multiply the radial balance by $s^2$ and integrate by parts:

$$
s_0^2p_e-2\int_0^{s_0}sP(s)\,ds=-\frac1{\mu_0}\int_0^{s_0}sB_\phi(s)^2\,ds.
$$

The toroidal contributions cancel. The resulting [flux-tube axial field virial identity](../../../../../../flux-tube-axial-field-virial-identity.md) is

$$
\boxed{\frac2{s_0^2}\int_0^{s_0}sB_z(s)^2\,ds
=B_p^2-\frac{4\mu_0}{s_0^2}\int_0^{s_0}sp(s)\,ds.}
$$

This is at most $B_p^2$, and is strictly smaller whenever the weighted [pressure](../../../../../../pressure.md) integral is positive. In particular, continuous matching with $p_e>0$ guarantees strictness. If only $p\geq0$ is assumed without a nondegenerate gas or continuous positive boundary pressure, the justified conclusion is the non-strict bound; the identity specifies exactly when equality occurs.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
