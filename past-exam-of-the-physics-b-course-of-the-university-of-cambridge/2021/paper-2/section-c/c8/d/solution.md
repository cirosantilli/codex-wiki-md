<h1 id="section-c/c8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Taking a [derivative](../../../../../../derivative.md) of the logarithmic form gives a direct way to use the plot's base-ten vertical axis:

$$
\boxed{L\simeq R\ln10\,T^2\frac{d\log_{10}(p/\mathrm{Pa})}{dT}.}
$$

Alternatively, use two nearby readings and eliminate the unknown $p_0$:

$$
L\simeq R\ln10\,
\frac{\log_{10}(p_b/\mathrm{Pa})-\log_{10}(p_a/\mathrm{Pa})}{T_a^{-1}-T_b^{-1}}.
$$

Reading the original PDF graph approximately gives $\log_{10}(p/\mathrm{Pa})\simeq-0.6$ at $300\,\mathrm K$ and $\simeq3.8$ at $500\,\mathrm K$. These bracket the requested [temperature](../../../../../../temperature-split.md) and give an average [latent heat](../../../../../../latent-heat.md) near $400\,\mathrm K$:

$$
L\simeq(8.31\,\mathrm{J\,K^{-1}\,mol^{-1}})(2.3026)
\frac{4.4}{1/300-1/500}\,\mathrm K
\simeq6.3\times10^4\,\mathrm{J\,mol^{-1}}.
$$

Thus a suitable graph-based estimate is

$$
\boxed{L(400\,\mathrm K)\approx6\times10^4\,\mathrm{J\,mol^{-1}}\quad\text{(roughly }60\text{--}65\,\mathrm{kJ\,mol^{-1}}\text{).}}
$$

The graph does not warrant several significant figures; a local tangent or different reasonable nearby readings give a comparable estimate. The factor $\ln10$ is essential when using a base-ten logarithmic axis.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [C8](../../c8.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
