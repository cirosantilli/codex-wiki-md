<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Both neutral curves can be written with $x=k^2$ and $p=\pi^2$ as

$$
R(x)=C\frac{(x+p)^3}{x}+DQp\frac{x+p}{x}.
$$

For steady convection, $(C,D)=(1,1)$; for oscillatory convection,

$$
C_o=\frac{(\sigma+\zeta)(1+\zeta)}\sigma,\qquad D_o=\frac{\zeta(\sigma+\zeta)}{1+\sigma},\qquad \frac{D_o}{C_o}=\frac{\sigma\zeta}{(1+\sigma)(1+\zeta)}.
$$

The oscillatory result is physically relevant only with positive frequency; for fixed $0<\zeta<1$ and fixed positive $\sigma$, that holds at the minimizing [wavenumber](../../../../../../wavenumber.md) for sufficiently large $Q$.

Differentiation gives the exact minimization condition

$$
\boxed{x^2(2x+3p)=p^3+\frac DCQp^2.}
$$

Its left side is strictly increasing for $x>0$, so the minimum is unique. Define $h=[Dp^2Q/(2C)]^{1/3}$. An [asymptotic expansion](../../../../../../asymptotic-expansion.md) gives

$$
\boxed{k_*^2=h-\frac p2+\frac{p^2}{4h}+O(h^{-2}),\qquad k_*\sim\left(\frac{Dp^2}{2C}\right)^{1/6}Q^{1/6}.}
$$

Substituting back, the leading magnetic term is order $Q$, while the two balanced terms $Cx^2$ and $DQp^2/x$ sum to $3Ch^2$. Hence, through order $Q^{2/3}$,

$$
\boxed{R_{\rm min}=DpQ+3C^{1/3}\left(\frac{Dp^2Q}{2}\right)^{2/3}+O(Q^{1/3}).}
$$

In particular,

$$
\boxed{R^{(e)}_c=\pi^2Q+3\left(\frac{\pi^4Q}{2}\right)^{2/3}+O(Q^{1/3}),\qquad (k_*^{(e)})^2=\left(\frac{\pi^4Q}{2}\right)^{1/3}-\frac{\pi^2}{2}+O(Q^{-1/3}),}
$$

while the same boxed general formulas with $(C_o,D_o)$ give the oscillatory minimum and critical [wavenumber](../../../../../../wavenumber.md). Thus [strong-field wavenumber selection in magnetoconvection](../../../../../../strong-field-wavenumber-selection-in-magnetoconvection.md) has $k\propto Q^{1/6}$ for both types, with different parameter-dependent constants.

For the exact steady result at arbitrary $Q\ge0$, the stationarity equation with $C=D=1$ lets us eliminate $Q$ from $R^{(e)}$. It gives

$$
R_c=\frac{2(x+p)^3}{p},\qquad Qp=R_c-3(x+p)^2.
$$

At $Q=0$, $x=p/2$ and $R_0=27p^2/4$. Consequently

$$
\boxed{Q\pi^2=R_c-R_c^{2/3}R_0^{1/3},\qquad k_c^2=\pi^2\left[\frac32\left(\frac{R_c}{R_0}\right)^{1/3}-1\right].}
$$

This [exact critical Rayleigh relation for vertical-field magnetoconvection](../../../../../../exact-critical-rayleigh-relation-for-vertical-field-magnetoconvection.md) includes the nonmagnetic minimum, with $R_c\ge R_0$ and $k_c^2\ge\pi^2/2$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Section III](../../section-iii.md)
4. [Paper 77](../../../paper-77-split.md)
5. [Iii](../../../split.md)
6. [2012](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
