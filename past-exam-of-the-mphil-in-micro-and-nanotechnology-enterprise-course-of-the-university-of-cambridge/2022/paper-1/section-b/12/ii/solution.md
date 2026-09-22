<h1 id="section-b/12/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A generator couple has a p-type and an n-type thermoelement joined electrically at the hot face, with their other ends connected through a load at the cold face. The legs are **electrically in series and thermally in parallel**. Electrically insulating, thermally conducting plates couple them to the hot source and cold sink; metal interconnects carry current. The [Seebeck effect](../../../../../../seebeck-effect.md) provides an open-circuit electromotive force $\mathcal E=\alpha_{np}\Delta T$, where the magnitude of $\alpha_{np}$ is the difference between the two leg Seebeck coefficients.

For fixed junction temperatures, constant properties and internal resistance $R$,

$$
P_L=I^2R_L=\frac{(\alpha_{np}\Delta T)^2R_L}{(R+R_L)^2}.
$$

Differentiate with respect to load resistance:

$$
\frac{dP_L}{dR_L}=(\alpha_{np}\Delta T)^2\frac{R-R_L}{(R+R_L)^3}.
$$

The derivative changes from positive to negative at $R_L=R$, so

$$
\boxed{R_L=R,\qquad I_{P_{\max}}=\frac{\alpha_{np}\Delta T}{2R},\qquad P_{\max}=\frac{(\alpha_{np}\Delta T)^2}{4R}.}
$$

The load voltage is then half the open-circuit voltage. The heat source and sink must sustain the temperature difference; an isolated hot object cools as energy is extracted. **Maximum power and maximum conversion efficiency are different operating points**: the efficiency-optimal load is generally larger than $R$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [12](../../12.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
