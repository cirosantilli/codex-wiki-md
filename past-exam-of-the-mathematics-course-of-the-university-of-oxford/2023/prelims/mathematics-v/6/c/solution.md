<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The lowest positive root belongs to the symmetric family and lies in $(0,\pi/2)$; all antisymmetric roots are at least $\pi$. Let $\alpha=m/(2\rho\ell)\gg1$. The equation $\cot z=\alpha z$ forces its first root to tend to zero: for any fixed $\varepsilon>0$, the right side eventually exceeds $\cot\varepsilon$ at $z=\varepsilon$, so the decreasing-minus-increasing difference has its zero below $\varepsilon$.

The [Taylor series](../../../../../../taylor-series.md) $\cot z=z^{-1}-z/3+O(z^3)$ then gives

$$
1=\left(\alpha+\frac13\right)z^2+O(z^4),\qquad
z\sim\alpha^{-1/2}=\sqrt{\frac{2\rho\ell}{m}}.
$$

Since $\omega=cz/\ell$ and $c=\sqrt{T/\rho}$, the lowest [angular frequency](../../../../../../angular-frequency.md) is

$$
\boxed{\omega\sim\frac1\ell\sqrt{\frac T\rho}\sqrt{\frac{2\rho\ell}{m}}
=\sqrt{\frac{2T}{m\ell}}=\omega_0.}
$$

Physically, at such a low [frequency](../../../../../../frequency.md) each half-string is nearly straight. If the mass moves up by $Y$, the two slopes are approximately $Y/\ell$ and $-Y/\ell$, so the restoring [force](../../../../../../force-split.md) is $-2TY/\ell$. The resulting [harmonic oscillator equation](../../../../../../simple-harmonic-motion.md), $m\ddot Y+(2T/\ell)Y=0$, has exactly the leading [angular frequency](../../../../../../angular-frequency.md) above. The next correction from the same expansion is $\omega/\omega_0=1-\rho\ell/(3m)+O((\rho\ell/m)^2)$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
