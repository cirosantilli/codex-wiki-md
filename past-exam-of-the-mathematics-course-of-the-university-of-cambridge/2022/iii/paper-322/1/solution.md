<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In a circular [binary star](../../../../../binary-star.md), the distances from the centre of mass are $a_1=aM_2/M$ and $a_2=aM_1/M$. Summing the two orbital angular momenta gives

$$
J=M_1a_1^2\Omega+M_2a_2^2\Omega
=\boxed{\frac{M_1M_2}{M}a^2\Omega}.
$$

Equivalently, $J=\mu\sqrt{GMa}$ by [Kepler third law](../../../../../kepler-s-third-law.md).

First consider a rapid conservative perturbation. Both $M=M_1+M_2$ and $J$ are fixed, while $dM_1=-dM_2$. With $q=M_2/M_1$,

$$
0=d\log J=(1-q)d\log M_2+\frac12d\log a,
$$

so

$$
\frac{d\log a}{d\log M_2}=2(q-1).
$$

The [Roche lobe](../../../../../roche-lobe.md) formula then gives its mass-radius exponent

$$
\zeta_L=\frac{d\log R_L}{d\log M_2}
=\frac13+2(q-1)=2q-\frac53.
$$

After mass loss, [dynamical stability of binary mass transfer](../../../../../dynamical-stability-of-binary-mass-transfer.md) requires the donor to shrink relative to its lobe. Since $d\log M_2<0$, this means $\zeta_{\rm ad}>\zeta_L$, or

$$
\boxed{q<\frac{3\zeta_{\rm ad}+5}{6}}.
$$

For stable secular [conservative binary mass transfer](../../../../../conservative-binary-mass-transfer.md), put $m=\dot M_2/M_2$. The angular-momentum and contact conditions are

$$
-\alpha=(1-q)m+\frac12\frac{\dot a}{a},
\qquad
\beta=\frac13m+\frac{\dot a}{a}.
$$

Elimination of $\dot a/a$ gives

$$
\boxed{-\frac{\dot M_2}{M_2}
=\frac{3(2\alpha+\beta)}{5-6q}}.
$$

Here [magnetic braking of a binary star](../../../../../magnetic-braking-of-a-binary-star.md) removes orbital angular momentum, while the donor's expansion maintains [Roche-lobe overflow](../../../../../roche-lobe-overflow.md).

In a [cataclysmic variable](../../../../../cataclysmic-variable.md), hydrogen-rich material accumulates on a degenerate white dwarf. Degeneracy prevents initial expansion from regulating its temperature, so nuclear ignition produces the [thin-shell instability](../../../../../thin-shell-instability.md) and a [classical nova](../../../../../classical-nova.md). Nuclear burning of hydrogen to helium releases about $0.007mc^2$, whereas the binding energy at a white-dwarf surface is only of order $GM_1m/R_1$, typically a few $10^{-4}mc^2$. Even modest coupling can therefore eject all the newly accreted envelope without disrupting the white dwarf.

Finally suppose every transferred mass element is expelled by [isotropic re-emission from a binary star](../../../../../isotropic-re-emission-from-a-binary-star.md). Then $\dot M_1=0$, $\dot M=\dot M_2$, and expelled matter carries the white dwarf's specific angular momentum $j_1=(M_2/M)^2a^2\Omega$. Hence

$$
\frac{\dot J}{J}=-\alpha+\frac{q^2}{1+q}m.
$$

On the other hand, logarithmic differentiation of $J=M_1M_2M^{-1/2}G^{1/2}a^{1/2}$ and of the Roche-lobe radius gives

$$
\frac{\dot J}{J}
=\left(1-\frac{q}{2(1+q)}\right)m
+\frac12\frac{\dot a}{a},
\qquad
\beta=\frac{m}{3(1+q)}+\frac{\dot a}{a}.
$$

Eliminating the separation produces

$$
\boxed{-\frac{\dot M_2}{M_2}
=\frac{3(1+q)(2\alpha+\beta)}
{5+3q-6q^2}}.
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 322](../../paper-322-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
