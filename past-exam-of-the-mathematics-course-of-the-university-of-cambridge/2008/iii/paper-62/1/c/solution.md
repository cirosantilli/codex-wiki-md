<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Dropping [radiation in cosmology](../../../../../../radiation-in-cosmology.md) in the [Friedmann equation](../../../../../../friedmann-equations.md) gives

$$
\tau_0\simeq H_0^{-1}\int_0^1\frac{da}{\sqrt{\Omega_m a+\Omega_\Lambda a^4}}.
$$

To evaluate this [matter-vacuum conformal age integral](../../../../../../matter-vacuum-conformal-age-integral.md), put $a=(\Omega_m/\Omega_\Lambda)^{1/3}y$. The square root in the denominator becomes $\Omega_m^{2/3}\Omega_\Lambda^{-1/6}\sqrt{y(1+y^3)}$, whereas $da=\Omega_m^{1/3}\Omega_\Lambda^{-1/3}dy$. Therefore

$$
\boxed{\tau_0\simeq H_0^{-1}\Omega_m^{-1/3}\Omega_\Lambda^{-1/6}
\int_0^{(\Omega_\Lambda/\Omega_m)^{1/3}}\frac{dy}{\sqrt{y(1+y^3)}}.}
$$

The radiation-free approximation is not valid arbitrarily close to the lower limit. Its extension to zero nevertheless gives a good leading [conformal time](../../../../../../conformal-time.md) estimate: the early-time correction has size $O(H_0^{-1}\sqrt{\Omega_r}/\Omega_m)$, small compared with the total age when [matter-radiation equality](../../../../../../matter-radiation-equality.md) occurs sufficiently early. The apparent $y^{-1/2}$ endpoint singularity is integrable.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
