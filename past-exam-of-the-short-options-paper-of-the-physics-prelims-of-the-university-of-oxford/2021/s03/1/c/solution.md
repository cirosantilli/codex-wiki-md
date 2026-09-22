<h1 id="s03/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $x=h\nu/(k_BT)=hc/(\lambda k_BT)$. In the long-[wavelength](../../../../../wavelength.md) limit $x\ll1$, the [Taylor expansion](../../../../../taylor-expansion.md) $e^x-1=x+O(x^2)$ in [Planck's law](../../../../../planck-s-law.md) gives the [Rayleigh-Jeans law](../../../../../rayleigh-jeans-law.md),

$$
\boxed{U_\nu\simeq\frac{8\pi k_BT}{c^3}\nu^2.}
$$

This is the classical [equipartition theorem](../../../../../equipartition-theorem.md) result: each electromagnetic mode carries mean [energy](../../../../../energy-split.md) $k_BT$. Extending it to arbitrarily high [frequency](../../../../../frequency.md) would make the total [energy density](../../../../../energy-density.md) diverge, the [ultraviolet catastrophe](../../../../../ultraviolet-catastrophe.md).

In the short-[wavelength](../../../../../wavelength.md) limit $x\gg1$, $e^x-1\simeq e^x$, giving the [Wien approximation](../../../../../wien-approximation.md),

$$
\boxed{U_\nu\simeq\frac{8\pi h}{c^3}\nu^3e^{-h\nu/(k_BT)}.}
$$

Large [photon energies](../../../../../photon-energy.md) are thermally suppressed, removing the classical high-[frequency](../../../../../frequency.md) divergence.

If the requested “form” is expressed per unit [wavelength](../../../../../wavelength.md), the change of variables includes its [Jacobian determinant](../../../../../jacobian-determinant.md): $U_\lambda=U_\nu|d\nu/d\lambda|=U_\nu c/\lambda^2$. Thus

$$
U_\lambda=\frac{8\pi hc}{\lambda^5}\frac1{e^{hc/(\lambda k_BT)}-1},\qquad
\boxed{U_\lambda\simeq\begin{cases}8\pi k_BT/\lambda^4,&x\ll1,\\8\pi hc\,e^{-x}/\lambda^5,&x\gg1.\end{cases}}
$$

Substituting $\nu=c/\lambda$ without the [Jacobian determinant](../../../../../jacobian-determinant.md) would give an incorrect spectral density.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [S03](../../../s03.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
