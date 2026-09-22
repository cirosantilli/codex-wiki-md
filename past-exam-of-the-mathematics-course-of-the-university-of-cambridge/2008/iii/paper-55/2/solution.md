<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $\Omega=e^{2\rho}$, $F=\partial_xA_2-\partial_yA_1$, and $s=|\Phi|^2$, so the physical [magnetic field](../../../../../magnetic-field.md) is $B=F/\Omega$. Use finite-energy [Abelian Higgs vortex](../../../../../nielsen-olesen-vortex.md) boundary data: the field tends to unit magnitude at the ideal boundary, its phase winds $N$ times, and the boundary limits in the decomposition exist. This vacuum asymptotic behavior is the setting in which the stated degree gives an energy bound. We retain the current boundary term; degree alone must not be silently equated with [magnetic flux](../../../../../magnetic-flux.md) on an open disk.

Define $j_i=\operatorname{Im}(\bar\Phi D_i\Phi)$. The [gauge-covariant derivative of a charged scalar field](../../../../../gauge-covariant-derivative-of-a-charged-scalar-field.md) satisfies $[D_x,D_y]\Phi=-iF\Phi$. Differentiating the current gives

$$
\partial_xj_y-\partial_yj_x
=2\operatorname{Im}(\overline{D_x\Phi}D_y\Phi)-F|\Phi|^2.
$$

On the other hand,

$$
|(D_x+iD_y)\Phi|^2
=|D_x\Phi|^2+|D_y\Phi|^2
-2\operatorname{Im}(\overline{D_x\Phi}D_y\Phi).
$$

Combining the two identities and [completing the square](../../../../../completing-the-square.md) in the magnetic and potential terms yields the [conformal-surface vortex square completion](../../../../../conformal-surface-vortex-square-completion.md)

$$
\begin{aligned}
V={}&\frac12\int_\Sigma
\left[\Omega^{-1}\left(F-\frac\Omega2(1-s)\right)^2
+|(D_x+iD_y)\Phi|^2\right]dxdy\\
&+\frac12\int_\Sigma F\,dxdy
+\frac12\int_\Sigma(\partial_xj_y-\partial_yj_x)dxdy.
\end{aligned}
$$

All integrations on the noncompact metric disk can first be made over $|z|<R<1$ and then passed to the limit. By the [Stokes theorem](../../../../../stokes-theorem.md), the two boundary contributions combine to $\tfrac12\oint(A+j)$. At the vacuum boundary write $\Phi=e^{i\chi}$. Then $j=d\chi-A$, so this combined integral is $\tfrac12\oint d\chi=\pi N$, even if the current term does not vanish separately. The usual additional condition of tangential covariant decay makes that current term vanish and yields [magnetic flux quantization of an Abelian Higgs vortex](../../../../../magnetic-flux-quantization-of-an-abelian-higgs-vortex.md), but is not needed if the combined boundary term has this phase limit. Thus for $N\geq0$, $V\geq\pi N$. Reversing both signs in the square completion gives $V\geq-\pi N$ for $N\leq0$, hence

$$
\boxed{V\geq\pi|N|.}
$$

For positive degree, equality is attained precisely when the [Bogomolny vortex equations](../../../../../bogomolny-vortex-equation.md) are

$$
(D_x+iD_y)\Phi=0,\qquad
F=\frac\Omega2(1-|\Phi|^2),
\quad\text{or equivalently}\quad B=\frac12(1-|\Phi|^2).
$$

Distinguishing the physical field $B$ from the coordinate curvature coefficient $F$ prevents an erroneous conformal factor.

For the proposed field, set $q=x^2+y^2$ and choose the smooth [connection one-form](../../../../../connection-one-form.md)

$$
\boxed{A=\frac{2(x\,dy-y\,dx)}{1+q},\qquad
A_1=-\frac{2y}{1+q},\quad A_2=\frac{2x}{1+q}.}
$$

Indeed, with $\partial_{\bar z}=\tfrac12(\partial_x+i\partial_y)$ and $A_{\bar z}=\tfrac12(A_1+iA_2)$,

$$
\partial_{\bar z}\Phi=-\frac{2z^2}{(1+q)^2},\qquad
A_{\bar z}=\frac{iz}{1+q},\qquad
(\partial_{\bar z}-iA_{\bar z})\Phi=0.
$$

The second [Bogomolny vortex equation](../../../../../bogomolny-vortex-equation.md) follows from

$$
F=\frac4{(1+q)^2},\qquad
1-|\Phi|^2=\frac{(1-q)^2}{(1+q)^2},\qquad
\Omega=\frac8{(1-q)^2}.
$$

Thus both squares vanish, including at the simple zero $z=0$ by smoothness. At $r\to1$, $\Phi\to e^{i\vartheta}$ and $A=2r^2d\vartheta/(1+r^2)\to d\vartheta$, proving degree one. Moreover, $j_\vartheta=4r^2(1-r^2)/(1+r^2)^3\to0$, so the current boundary term really vanishes for this solution. The [magnetic flux](../../../../../magnetic-flux.md) is explicitly

$$
\int_\Sigma F\,dxdy
=8\pi\int_0^1\frac{r\,dr}{(1+r^2)^2}=2\pi.
$$

Consequently

$$
\boxed{V(A,\Phi)=\pi,\qquad N=1.}
$$

This is the [hyperbolic one-vortex at curvature minus one half](../../../../../hyperbolic-one-vortex-at-curvature-minus-one-half.md); its finite energy follows directly from the vanishing squares and the finite flux.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
