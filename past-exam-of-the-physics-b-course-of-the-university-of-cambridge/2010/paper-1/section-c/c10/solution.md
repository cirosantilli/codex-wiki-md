<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

For a fixed-composition [simple compressible system](../../../../../simple-compressible-system.md), $dG=-S\,dT+V\,dp$ gives $S=-(\partial G/\partial T)_p$ and $V=(\partial G/\partial p)_T$. Equality of mixed [derivatives](../../../../../derivative.md) yields $(\partial S/\partial p)_T=-(\partial V/\partial T)_p$. Therefore

$$
dS=-\left(\frac{\partial V}{\partial T}\right)_pdp
+\left(\frac{\partial S}{\partial T}\right)_pdT.
$$

For one mole of [ideal gas](../../../../../ideal-gas-split.md), $V_m=RT/p$, so $(\partial V_m/\partial T)_p=R/p$. Reversible [heat](../../../../../heat-split.md) at fixed [pressure](../../../../../pressure-split.md) gives $(\partial S_m/\partial T)_p=C_{mp}/T$, and consequently

$$
dS_m=-\frac Rp\,dp+\frac{C_{mp}}T\,dT.
$$

With constant positive [molar heat capacity](../../../../../molar-heat-capacity.md), integrate from a reference state $(p_0,T_0)$:

$$
\boxed{S_m=S_0-R\ln\frac p{p_0}+C_{mp}\ln\frac T{T_0}.}
$$

If [heat capacity](../../../../../heat-capacity.md) varies, the last term must instead be $\int_{T_0}^{T}C_{mp}(T')\,dT'/T'$. The reference ratios make the logarithms dimensionless. The following [classical ideal-gas entropy limits](../../../../../classical-ideal-gas-entropy-limits.md) test where the constant-heat-capacity expression remains applicable.

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
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
