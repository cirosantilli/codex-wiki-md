<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate $H=U+pV$ at fixed [pressure](../../../../../pressure-split.md) and subtract the [heat capacity at constant volume](../../../../../heat-capacity-at-constant-volume.md):

$$
C_p-C_V=\left(\frac{\partial U}{\partial T}\right)_p+p\left(\frac{\partial V}{\partial T}\right)_p-\left(\frac{\partial U}{\partial T}\right)_V.
$$

Now use $U=U(T,V)$ and the [multivariable chain rule](../../../../../multivariable-chain-rule.md) along a constant-pressure path:

$$
\left(\frac{\partial U}{\partial T}\right)_p=\left(\frac{\partial U}{\partial T}\right)_V+\left(\frac{\partial U}{\partial V}\right)_T\left(\frac{\partial V}{\partial T}\right)_p.
$$

Substitution cancels the fixed-volume [derivative](../../../../../derivative.md) and gives the [volume derivative form of the heat-capacity difference](../../../../../volume-derivative-form-of-the-heat-capacity-difference.md),

$$
\boxed{C_p-C_V=\left[\left(\frac{\partial U}{\partial V}\right)_T+p\right]\left(\frac{\partial V}{\partial T}\right)_p.}
$$

For the [ideal gas](../../../../../ideal-gas-split.md), the first term in brackets vanishes and $V=NkT/p$, so $(\partial V/\partial T)_p=Nk/p$. Consequently $\boxed{C_p-C_V=Nk}$ for the entire gas, with fixed particle number $N$. The extra [heat capacity](../../../../../heat-capacity.md) accounts for expansion [work](../../../../../work.md) at constant [pressure](../../../../../pressure-split.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [9](../../9.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
