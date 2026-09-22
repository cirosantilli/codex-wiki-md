<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

For a fixed amount of simple compressible material, $dU=T,dS-p,dV$ and $G=U-TS+pV$ gives $dG=-S,dT+V,dp$. Equality of mixed partial derivatives of $G$ therefore yields the [Maxwell relation](../../../../../maxwell-relations.md)

$$
\boxed{\left(\frac{\partial S}{\partial p}\right)_T=-\left(\frac{\partial V}{\partial T}\right)_p.}
$$

In the insulated throttling process, piston work into the gas is $p_1V_1$ and work out is $p_2V_2$. Neglecting changes in macroscopic kinetic and gravitational energy, the first law gives $U_2-U_1=p_1V_1-p_2V_2$. Thus **$U_1+p_1V_1=U_2+p_2V_2$**, so [enthalpy](../../../../../enthalpy.md) is conserved. The irreversible process is not assumed isentropic.

Since $dH=T,dS+V,dp$ and $dS=(C_p/T)dT-(\partial V/\partial T)_pdp$, one has $dH=C_p,dT+[V-T(\partial V/\partial T)_p]dp$. Therefore the [Joule-Thomson coefficient](../../../../../joule-thomson-coefficient.md) is

$$
\boxed{\mu_{JT}=\left(\frac{\partial T}{\partial p}\right)_H
=\frac{T(\partial V/\partial T)_p-V}{C_p}=\frac{V(\alpha T-1)}{C_p}.}
$$

For an [ideal gas](../../../../../ideal-gas.md), $V\propto T$ at fixed pressure and $\alpha=1/T$, so **$\mu_{JT}=0$**. A pressure drop has $dp<0$, so cooling, $dT<0$, requires **$\mu_{JT}>0$** in the operating range.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
