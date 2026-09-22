<h1 id="section-b/b3/solution">Solution</h1>

↑ **Parent:** [B3](../b3.md)

With microstate energies held fixed when differentiating,

$$
\boxed{\langle E\rangle=-\frac{Z'}Z=-\partial_\beta\ln Z,\qquad
\langle E^2\rangle=\frac{Z''}Z,\qquad
\sigma_E^2=\partial_\beta^2\ln Z.}
$$

Since $d\beta/dT=-1/(k_BT^2)$,

$$
\boxed{\sigma_E^2=k_BT^2C_V.}
$$

The [canonical ensemble](../../../../../canonical-ensemble-split.md) fixes [volume](../../../../../volume.md) and [particle number](../../../../../particle-number.md), and any other external [Hamiltonian](../../../../../hamiltonian.md) parameters. Thus the derivative is $C_V$; pressure-fixed fluctuations would naturally involve [enthalpy](../../../../../enthalpy-split.md) in a different ensemble.

The [translational and two-level energy variance](../../../../../translational-and-two-level-energy-variance.md) follows because translation and internal states factorize for this dilute classical gas:

$$
Z=Z_{\rm tr}(1+e^{-\beta\epsilon})^N,\qquad
\ln Z_{\rm tr}=\text{constant}-\frac{3N}{2}\ln\beta.
$$

Differentiating twice yields

$$
\boxed{\sigma_E^2=\frac32N(k_BT)^2+
N\epsilon^2\frac{e^{\epsilon/(k_BT)}}{[1+e^{\epsilon/(k_BT)}]^2}.}
$$

The terms are independent translational and two-level binomial [variances](../../../../../variance-split.md). At $k_BT\ll\epsilon$, excitation freezes out exponentially and translation dominates. At $k_BT\gg\epsilon$, the internal [variance](../../../../../variance-split.md) tends to $N\epsilon^2/4$ while the translational [variance](../../../../../variance-split.md) grows as $T^2$; the internal [heat capacity](../../../../../heat-capacity.md) consequently tends to zero. Fractional total-energy fluctuations are of order $N^{-1/2}$ for large $N$. The low-temperature statement presumes translation is still nondegenerate; at strictly zero [temperature](../../../../../temperature-split.md) the classical-gas model fails.

## ↑ Ancestors (13)

1. [B3](../b3.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2012](../../../split.md)
5. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
