<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\rho=m^2\Lambda^{-2}$ for the PDF's signed mass coordinate $u^2$, and $K_D=\Omega_D/(2\pi)^D$. The superscript on $u^2$ is notation here, not a restriction to positive mass. In a [momentum-shell renormalization group](../../../../../../momentum-shell-renormalization-group.md) step, remove momenta $\Lambda e^{-d\ell}<|p|<\Lambda$ and set $\ell=\log(\Lambda_0/\Lambda)$, the PDF's $b$. Split the [scalar field](../../../../../../scalar-field.md) into a slow field $\varphi$ and a fast field $\eta$, whose [Gaussian shell covariance](../../../../../../gaussian-shell-covariance.md) is $(p^2+m^2)^{-1}$. The shell must have a positive quadratic kernel; $1+\rho>0$ near the fixed point meets this requirement.

Expand the coarse action by the [cumulant expansion of a coarse-grained free energy](../../../../../../cumulant-expansion-of-a-coarse-grained-free-energy.md). In the first cumulant of $V=g\int(\varphi+\eta)^4/4!$, the term with two fast fields is $(g/4)\int\varphi^2\langle\eta^2\rangle$. Thus the [one-loop shell mass renormalization in scalar quartic theory](../../../../../../one-loop-shell-mass-renormalization-in-scalar-quartic-theory.md) is

$$
\delta m^2=\frac g2 I_1,\qquad I_1=\int_{\rm shell}\frac{d^Dp}{(2\pi)^D}\frac1{p^2+m^2}.
$$

For the quartic correction, the two-fast-field vertex is $(g/4)\int\varphi^2\eta^2$. Its connected second cumulant has a minus sign and uses $\langle\eta^2(x)\eta^2(y)\rangle_c=2G_>(x-y)^2$. It gives

$$
-\frac{g^2}{16}\int d^Dx\,d^Dy\,\varphi^2(x)\varphi^2(y)G_>(x-y)^2.
$$

Taking the local zero-external-momentum quartic part produces $\delta g=-3g^2I_2/2$, where $I_2=\int_{\rm shell}d^Dp\,(2\pi)^{-D}(p^2+m^2)^{-2}$. This derives the combinatorial factors in the [one-loop shell quartic renormalization](../../../../../../one-loop-shell-quartic-renormalization.md). The mass tadpole is independent of external momentum; kinetic normalization changes only at higher order for the leading epsilon calculation.

For an infinitesimal spherical shell, radial integration gives

$$
I_1=K_D\frac{\Lambda^{D-2}}{1+\rho}\,d\ell,
\qquad I_2=K_D\frac{\Lambda^{D-4}}{(1+\rho)^2}\,d\ell.
$$

Lowering the cutoff adds the engineering terms $2\rho$ and $\epsilon\lambda$ to the running dimensionless couplings. Since $g=\lambda\Lambda^\epsilon$ and $D=4-\epsilon$, the remaining cutoff powers cancel exactly. Therefore

$$
\boxed{\frac{d\rho}{d\ell}=2\rho+\frac{K_D}{2}\frac{\lambda}{1+\rho},\qquad
\frac{d\lambda}{d\ell}=\epsilon\lambda-\frac{3K_D}{2}\frac{\lambda^2}{(1+\rho)^2}.}
$$

These are the requested flows, to the stated one-loop order. They implement cutoff independence of long-wavelength observables after changing the couplings and retaining the generated constant and other effective operators to the relevant approximation order. They are not an exact closure of the complete effective action.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
