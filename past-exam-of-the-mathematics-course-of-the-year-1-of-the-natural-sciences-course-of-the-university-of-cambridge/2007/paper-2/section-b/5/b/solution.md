<h1 id="section-b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Holding $y$ fixed, the [chain rule](../../../../../../chain-rule.md) gives

$$
\boxed{\left(\frac{\partial v}{\partial u}\right)_y\left(\frac{\partial u}{\partial x}\right)_y=\left(\frac{\partial v}{\partial x}\right)_y,}
$$

where the local change of variable from $x$ to $u$ is valid.

For the [internal energy](../../../../../../internal-energy-split.md) $U(S,V)$, its [exact differential](../../../../../../exact-differential.md) identifies $T=U_S$ and $p=-U_V$. The [Maxwell relation](../../../../../../maxwell-relations.md) from equality of mixed [partial derivatives](../../../../../../partial-derivative.md) is $T_V|_S=-p_S|_V$. At fixed [volume](../../../../../../volume-thermodynamics.md), the [constant-volume heat capacity](../../../../../../heat-capacity-at-constant-volume.md) satisfies

$$
C_V=\left(\frac{\partial U}{\partial T}\right)_V=T\left(\frac{\partial S}{\partial T}\right)_V,
$$

so $T_S|_V=T/C_V$, assuming nonzero $C_V$ and a locally invertible relation. Applying the [chain rule](../../../../../../chain-rule.md) to $p(T,V)$ gives the [isentropic temperature-volume derivative](../../../../../../isentropic-temperature-volume-derivative.md)

$$
\boxed{\left(\frac{\partial T}{\partial V}\right)_S=-\left(\frac{\partial p}{\partial T}\right)_V\left(\frac{\partial T}{\partial S}\right)_V=-\frac{T}{C_V}\left(\frac{\partial p}{\partial T}\right)_V.}
$$

For the stated one-mole [ideal gas](../../../../../../ideal-gas-split.md), the [equation of state](../../../../../../equation-of-state.md) gives $p_T|_V=R/V$ and $C_V=3R/2$, so the right side is $-2T/(3V)$. Along an [isentropic process](../../../../../../isentropic-process.md), $p\propto V^{-5/3}$ and $T=pV/R\propto V^{-2/3}$, giving the same left side:

$$
\boxed{\left(\frac{\partial T}{\partial V}\right)_S=-\frac{2T}{3V}.}
$$

## ↑ Ancestors (14)

1. [B](../b.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
