<h1 id="h/h1/solution">Solution</h1>

↑ **Parent:** [H1](../h1.md)

Time [independence](../../../../independent-random-variables.md) conserves the [energy](../../../../energy-split.md) $E=T+mga\cos\theta$. The two cyclic coordinates give

$$
p_\psi=C(\dot\psi+\dot\phi\cos\theta)=Cn,\qquad
p_\phi=A\dot\phi\sin^2\theta+Cn\cos\theta=h.
$$

These are respectively [angular momentum](../../../../angular-momentum.md) along the symmetry axis and [angular momentum](../../../../angular-momentum.md) along the fixed upward vertical; $n$ is the axial spin rate. For $u=\cos\theta$ and $-1<u<1$, eliminate $\dot\phi$ using $\dot\phi=(h-Cnu)/[A(1-u^2)]$. The [energy](../../../../energy-split.md) becomes

$$
E=\frac A2\dot\theta^2+\frac C2n^2+mga u+\frac{(h-Cnu)^2}{2A(1-u^2)}.
$$

Multiplying and rearranging gives

$$
\boxed{A^2\dot\theta^2=\frac{A(2E-Cn^2-2mga u)(1-u^2)-(h-Cnu)^2}{1-u^2}}.
$$

To justify the double-root condition, use the [effective potential](../../../../effective-potential.md)

$$
U(u)=\frac C2n^2+mga u+\frac{(h-Cnu)^2}{2A(1-u^2)}.
$$

Eliminating the cyclic coordinates by Routh reduction gives the remaining equation $A\ddot\theta=-dU(\cos\theta)/d\theta$. A constant nonvertical angle therefore has $U'(u_0)=0$ and $E=U(u_0)$. Since $P(u)=2A(E-U(u))(1-u^2)$, both $P(u_0)$ and $P'(u_0)$ vanish. This argument uses the second-order equation; merely differentiating the [energy](../../../../energy-split.md) identity at a stationary angle would not establish the derivative condition.

Thus **steady nonvertical [precession](../../../../precession.md) gives a common root in $(-1,1)$**. The nonvertical qualification is implicit in the denominator used by the source. A top spinning exactly upright or inverted is also possible but corresponds to an endpoint $u=\pm1$, not an interior root; the unrestricted literal claim would need that exception.

The distinction is captured by the [double-root criterion for steady precession of a symmetric top](../../../../double-root-criterion-for-steady-precession-of-a-symmetric-top.md).

## ↑ Ancestors (12)

1. [H1](../h1.md)
2. [H](../../h.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
