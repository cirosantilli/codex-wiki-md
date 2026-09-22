<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Steady [mass conservation](../../../../../../mass-conservation.md) gives $\dot m=-2\pi R\Sigma u_R$. With specific angular momentum $l=R^2\Omega$, multiply the angular-momentum equation by $2\pi$ and define the signed [viscous torque in an accretion disk](../../../../../../viscous-torque-in-an-accretion-disk.md)

$$
\mathcal G(R)=2\pi\nu\Sigma R^3\frac{d\Omega}{dR}.
$$

Then

$$
\frac{d\mathcal G}{dR}
=-\dot m\frac{dl}{dR}.
$$

Integration from $R_1$ to $R_2$ gives

$$
\boxed{
\mathcal G_2-\mathcal G_1=-\dot m(l_2-l_1)
}.
$$

The viscous power generated in an annulus is $2\pi R F_{\rm diss}\,dR=\mathcal G\,d\Omega$. Taking the inner torque to vanish and writing $l_{\rm in}=l(R_{\rm in})$ gives $\mathcal G=-\dot m(l-l_{\rm in})$, hence

$$
L_{\rm gen}
=-\dot m\int_{R_{\rm in}}^{R_{\rm out}}
(l-l_{\rm in})\frac{d\Omega}{dR}\,dR.
$$

[Integration by parts](../../../../../../integration-by-parts.md) yields

$$
L_{\rm gen}
=\dot m\left[
\int_{l_{\rm in}}^{l_{\rm out}}\Omega\,dl
-\Omega_{\rm out}(l_{\rm out}-l_{\rm in})
\right].
$$

For steady circular force balance, $de=\Omega\,dl$; equivalently, the stated equality of gravitational- and rotational-potential differences makes the integral $e_{\rm out}-e_{\rm in}$. Therefore

$$
\boxed{
L_{\rm gen}(R_{\rm in},R_{\rm out})
\simeq\dot m
\left[e_{\rm out}-e_{\rm in}
-\Omega_{\rm out}(l_{\rm out}-l_{\rm in})\right]
}.
$$

When $R_{\rm out}\gg R_{\rm in}$, the outer energy and boundary term vanish. For an approximately Keplerian inner orbit, $e_{\rm in}=-R_{\rm in}^2\Omega_{\rm in}^2/2$, so

$$
L_{\rm gen}\simeq
\frac12\dot mR_{\rm in}^2\Omega_{\rm in}^2.
$$

Comparison with part (c) gives

$$
\boxed{
\frac{L_{\rm gen}}{L_{\rm thin}}
\simeq
\left(\frac{\Omega_{\rm in}}{\Omega_{K,\rm in}}\right)^2
}.
$$

A Keplerian inner flow generates the standard thin-disk power. A pressure-supported sub-Keplerian slim disk generates less through shear, and its emergent luminosity can be smaller still because [photon trapping in an accretion flow](../../../../../../photon-trapping-in-an-accretion-flow.md) carries part of that generated energy through the inner edge.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
