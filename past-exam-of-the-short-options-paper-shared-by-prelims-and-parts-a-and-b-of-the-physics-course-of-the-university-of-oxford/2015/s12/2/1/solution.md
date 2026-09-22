<h1 id="s12/2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let the interface be $y=0$, with glass at $y<0$ and water at $y>0$, and choose $x$ parallel to the incident beam's tangential component. Define $k=\omega/c$ as the vacuum [wavenumber](../../../../../wavenumber.md), with glass and water [refractive indices](../../../../../refractive-index.md) $n_g$ and $n_w$. Continuity of [phase](../../../../../phase-waves.md) along the interface fixes $k_x=kn_g\sin\theta$. In water, the [dispersion relation](../../../../../dispersion-relation-split.md) is $k_x^2+k_y^2=k^2n_w^2$, so above the [critical angle](../../../../../critical-angle-for-total-internal-reflection.md),

$$
k_y^2=-k^2(n_g^2\sin^2\theta-n_w^2),\qquad k_y=i\kappa,\qquad \kappa=k\sqrt{n_g^2\sin^2\theta-n_w^2}>0.
$$

Choose the positive imaginary part because a field growing exponentially into the water would be unphysical. The [evanescent field in total internal reflection](../../../../../evanescent-field-in-total-internal-reflection.md) is therefore

$$
\boxed{E(x,y,t)=E_0\exp[i(kn_g\sin\theta\,x-\omega t)]\exp[-k\sqrt{n_g^2\sin^2\theta-n_w^2}\,y].}
$$

It propagates in phase parallel to the interface but decays normally. Here $E_0$ is the transmitted field amplitude at the interface; relating it to the incident amplitude requires the appropriate polarization-dependent [Fresnel equations](../../../../../fresnel-equations.md). If the symbol $k$ instead denotes the incident glass [wavenumber](../../../../../wavenumber.md), replace every vacuum $k$ in the formula by $k/n_g$; equivalently $k_x=k\sin\theta$ and $\kappa=k\sqrt{\sin^2\theta-(n_w/n_g)^2}$. This states the wavenumber convention left implicit in the source.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [2](../../2.md)
3. [S12](../../../s12.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
