<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

Apply [Faraday's law](../../../../../faraday-s-law-of-induction.md) to a shrinking rectangular loop crossing the interface. For bounded fields the magnetic-flux term vanishes with its area, giving $\mathbf E_{t,+}=\mathbf E_{t,-}$. A shrinking [Gaussian pillbox](../../../../../gaussian-pillbox.md) similarly gives $D_{n,+}-D_{n,-}=\sigma_{\rm free}$. Thus **normal $D$ is continuous when no free surface charge is present**, even though a bound polarization charge may remain. These are the assumptions needed for the stated [dielectric-interface boundary conditions](../../../../../dielectric-interface-boundary-conditions.md).

Write $\epsilon=\epsilon_r\epsilon_0$, $r_+=\sqrt{(x-a)^2+y^2+z^2}$ and $r_-=\sqrt{(x+a)^2+y^2+z^2}$. Use each region's own [permittivity](../../../../../permittivity-split.md) in its [Coulomb potential](../../../../../coulomb-potential-energy.md):

$$
\phi_- =\frac{Q+Q'}{4\pi\epsilon r_+},\qquad
\phi_+=\frac1{4\pi\epsilon_0}\left(\frac Q{r_+}+\frac{Q''}{r_-}\right).
$$

At $x=0$, [continuity](../../../../../continuous-function.md) of potential and normal displacement gives

$$
\frac{Q+Q'}{\epsilon_r}=Q+Q'',\qquad Q+Q'=Q-Q''.
$$

Solving,

$$
\boxed{Q'=\frac{\epsilon_r-1}{\epsilon_r+1}Q,\qquad
Q''=-\frac{\epsilon_r-1}{\epsilon_r+1}Q.}
$$

This [permittivity convention for transmitted image charges](../../../../../permittivity-convention-for-transmitted-image-charges.md) matters: if the vacuum Coulomb prefactor is used even for $\phi_-$, its combined effective source is $2Q/(1+\epsilon_r)$ instead. The physical potential is the same. The two numbered leaves identify how these sources satisfy the equations in their respective regions.

The real charge feels only the image contribution after removing its own singular self-field. The image at $(-a,0,0)$ is separated from it by $2a$, so

$$
\boxed{\mathbf F=\left(-\frac{\epsilon_r-1}{\epsilon_r+1}\frac{Q^2}{16\pi\epsilon_0a^2},0,0\right).}
$$

For the [bound charge](../../../../../bound-charge.md), the outward normal of the [dielectric](../../../../../dielectric.md) is $+\hat x$ and $\mathbf P=\epsilon_0(\epsilon_r-1)\mathbf E_-$. Differentiating $\phi_-$ at $x=0$ gives $E_{-,x}=-a(Q+Q')/[4\pi\epsilon(a^2+y^2+z^2)^{3/2}]$. Therefore

$$
\boxed{\sigma_b=\mathbf P\cdot\hat x=-\frac{\epsilon_r-1}{\epsilon_r+1}\frac{aQ}{2\pi(a^2+y^2+z^2)^{3/2}}.}
$$

Its [integral](../../../../../integral-split.md) over the plane is $Q''$, consistent with the external image representation. For $\epsilon_r=1$ both the image force and induced surface charge vanish.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
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
