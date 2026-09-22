<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret $\rho_2$ as the ambient [density](../../../../../../density.md): the PDF's phrase assigning it a “depth” is a typographical error. Take $0<\rho_1-\rho_2\ll\rho_2$, and use a common reference [density](../../../../../../density.md) in inertia while retaining the [density](../../../../../../density.md) difference in [buoyancy](../../../../../../buoyancy.md). This is the [Boussinesq approximation](../../../../../../boussinesq-approximation.md), with [reduced gravity](../../../../../../reduced-gravity-split.md) $g'=g(\rho_1-\rho_2)/\rho_{\mathrm{ref}}>0$. For the [shallow water](../../../../../../shallow-water-approximation.md) approximation, the lower-layer depth must be small compared with longitudinal variation scales, vertical accelerations must be negligible and [pressure](../../../../../../pressure.md) hydrostatic. The deep ambient is approximated as a [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) reservoir away from the nose; assume a uniform [velocity](../../../../../../velocity.md) over each lower-layer cross-section and neglect drag and entrainment.

Write the prismatic triangular area as $A(h)=kh^2$ with fixed $k>0$, so the width at height $z$ is $2kz$. The excess [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) force divided by reference [density](../../../../../../density.md) is

$$
P(h)=g'\int_0^h(h-z)2kz\,dz=\frac{g'kh^3}{3}.
$$

The [prismatic-channel shallow water equations](../../../../../../prismatic-channel-shallow-water-equations.md) are therefore

$$
\boxed{(kh^2)_t+(kh^2u)_x=0,\qquad
(kh^2u)_t+\left(kh^2u^2+\frac{g'kh^3}{3}\right)_x=0.}
$$

For positive depth, divide the first equation by $2kh$ and use it in the second to obtain

$$
\boxed{h_t+uh_x+\frac h2u_x=0,\qquad
u_t+uu_x+g'h_x=0.}
$$

The coefficient matrix in variables $(h,u)$ is $\begin{pmatrix}u&h/2\\g'&u\end{pmatrix}$. Its two distinct real [characteristic speeds](../../../../../../characteristic-speed.md) are

$$
\boxed{\lambda_\pm=u\pm c,\qquad c=\sqrt{g'h/2}.}
$$

Thus the system is strictly hyperbolic for $h>0$ and $g'>0$, though it degenerates at zero depth. Since $dc/dh=c/(2h)$, direct substitution in the two equations gives

$$
\boxed{\left[\partial_t+(u\pm c)\partial_x\right](u\pm4c)=0.}
$$

Hence $R_\pm=u\pm4c$ are the [Riemann invariants](../../../../../../riemann-invariant.md) conserved along their respective [characteristic curves](../../../../../../characteristic-curve.md). The factor four, rather than the rectangular-channel factor two, comes from the triangular relation $A\propto h^2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
