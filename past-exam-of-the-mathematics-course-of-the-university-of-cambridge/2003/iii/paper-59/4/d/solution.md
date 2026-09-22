<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the perturbed amplitude equations, direct differentiation of the [first integral](../../../../../../first-integral.md) gives

$$
F'=-\varepsilon u(\lambda_1+v^2)(\lambda_2+u^2+v^2).
$$

The axis connection contributes zero since $u=0$. On the unperturbed interior [heteroclinic orbit](../../../../../../heteroclinic-orbit.md), $u=\sqrt{3(a^2-v^2)}$ and $v'=2(a^2-v^2)$, so the first-order change is

$$
\Delta F=-\varepsilon\sqrt3\int_{-a}^a(\lambda_1+v^2)\sqrt{a^2-v^2}\,dv+O(\varepsilon^2).
$$

The substitution $v=a\cos\phi$ gives

$$
\int_{-a}^a\sqrt{a^2-v^2}\,dv=\frac{\pi a^2}{2},\qquad
\int_{-a}^av^2\sqrt{a^2-v^2}\,dv=\frac{\pi a^4}{8}.
$$

Consequently

$$
\Delta F=-\frac{\varepsilon\pi\sqrt3a^2}{2}(\lambda_1+a^2/4)+O(\varepsilon^2).
$$

The simple zero of this [Melnikov energy-balance method](../../../../../../melnikov-energy-balance-method.md) calculation gives the [heteroclinic splitting of a fold-Hopf amplitude cycle](../../../../../../heteroclinic-splitting-of-a-fold-hopf-amplitude-cycle.md):

$$
\boxed{\lambda_1=\lambda_2/4+O(\varepsilon),\qquad
\mu_1=\mu_2/4+O(|\mu_2|^{3/2}),\quad\mu_2<0.}
$$

This is a leading persistence curve, not an exact parameter equality for the perturbed orbit. It lies between the two primary [Hopf bifurcation](../../../../../../hopf-bifurcation.md) curves near the origin and on the negative-$\mu_1$ side of the secondary torus curve $\mu_1=0$. With the added term the primary [Hopf bifurcation](../../../../../../hopf-bifurcation.md) curves themselves shift to $\mu_1=\pm2\sqrt{-\mu_2}+\mu_2$.

The sign of the amplitude balance also identifies the local torus branch. Over a small closed limiting contour, $\Delta F=-\varepsilon\oint u(\lambda_1+v^2)\,dv$. Its enclosed-area form sets $\lambda_1$ equal to minus the area-average of $v^2$. This average tends to zero at the centre and to $a^2/4$ at the [heteroclinic cycle](../../../../../../heteroclinic-cycle.md). Near the centre, negative $\lambda_1$ attracts trajectories toward the stable amplitude equilibrium; outside a zero-balance contour, $F$ decreases and the amplitude excursion grows. Thus the secondary bifurcation creates an unstable invariant [torus](../../../../../../torus.md) on the stable-periodic-orbit side. Its continuation reaches the global connection as the balance tends to $\lambda_1=-a^2/4$. The [bifurcation diagram](../../../../../../bifurcation-diagram.md) distinguishes this perturbed connection from the entire degenerate family present in the unperturbed system.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
