<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use $-\pi<\theta_s<\pi$, with the [crack](../../../../crack-in-a-solid.md) along the negative radial axis. In the coefficient convention used here, the leading [crack](../../../../crack-in-a-solid.md)-tip expansion is

$$
\boxed{u^{(s)}=u_{\mathrm{reg}}+k_sR_s^{1/2}\sin(\theta_s/2),\qquad
\nabla u_{\mathrm{reg}}=o(R_s^{-1/2}).}
$$

The square-root term is harmonic and has zero angular [derivative](../../../../derivative.md) on both [crack](../../../../crack-in-a-solid.md) faces. Regular contributions may include a constant and bounded-[gradient](../../../../gradient.md) terms under smooth loading.

If $E(s)$ is the minimized elastic-plus-load potential, the [energy release rate](../../../../energy-release-rate.md) is $\boxed{G(s)=-dE(s)/ds}$. With this particular square-root coefficient normalization,

$$
\boxed{G(s)=\frac{\pi\mu}{4}k_s^2.}
$$

For example, the small-circle energy flux is $\int[\mathcal W n_1-\mu u_r u_{x_1}]R_s\,d\theta_s$. The singular term gives $\mathcal W=\mu k_s^2/(8R_s)$, $u_r=k_s\sin(\theta_s/2)/(2\sqrt{R_s})$ and $u_{x_1}=-k_s\sin(\theta_s/2)/(2\sqrt{R_s})$. Integration over $(-\pi,\pi)$ produces the stated factor. Other stress-intensity normalizations change that factor.

For toughness $G_c>0$, local stability against infinitesimal extension means $\boxed{G(s)\leq G_c}$, since the [derivative](../../../../derivative.md) of $E(s)+G_c(s+1)$ is nonnegative. Global energetic stability against every extension is the stronger condition $E(s)\leq E(r)+G_c(r-s)$ for all $r\geq s$.

In full isotropic linearized elasticity,

$$
\boxed{T^{\mathrm{lin}}=\lambda\operatorname{tr}(e)I+2\mu e.}
$$

For the antiplane field this becomes

$$
T^{\mathrm{lin}}=\mu\begin{pmatrix}0&0&u_{x_1}\\0&0&u_{x_2}\\u_{x_1}&u_{x_2}&0\end{pmatrix},\qquad
|T^{\mathrm{lin}}|^2=2\mu^2|\nabla u|^2.
$$

Ahead of the tip, $\theta_s=0$, the singular [gradient](../../../../gradient.md) is $(0,k_s/(2\sqrt{R_s}))$. Thus

$$
\boxed{|T^{\mathrm{lin}}|_{\theta_s=0}
=\frac{\mu|k_s|}{\sqrt2}R_s^{-1/2}+o(R_s^{-1/2}).}
$$

This is stronger than the printed remainder $o(R_s^{-1})$. If $k_s$ denotes a nonnegative intensity, it has the printed leading coefficient; for a signed singular coefficient its absolute value is essential because the left side is a [norm](../../../../norm.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
