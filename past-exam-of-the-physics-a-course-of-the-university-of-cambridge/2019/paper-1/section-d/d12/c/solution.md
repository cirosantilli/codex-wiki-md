<h1 id="section-d/d12/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Any direct-current component of the input produces an output ramp. The [input offset voltage](../../../../../../input-offset-voltage.md) and [input bias currents](../../../../../../input-bias-current.md) of a real [operational amplifier](../../../../../../operational-amplifier.md) therefore charge the feedback [capacitor](../../../../../../capacitor.md) until the output saturates. Even the desired signal can exceed the available output swing when integrated for too long. Initial [capacitor](../../../../../../capacitor.md) charge also introduces an unknown integration constant.

Place a large [resistor](../../../../../../resistor.md) $R_f$ in parallel with the feedback [capacitor](../../../../../../capacitor.md). The idealized [transfer function](../../../../../../transfer-function.md) then becomes

$$
\boxed{H(s)=-\frac{R_f/R}{1+sR_fC}.}
$$

Its finite direct-current gain $-R_f/R$ supplies a return path and bounds the response to a small offset; it approximates $-1/(sRC)$ when $\omega R_fC\gg1$. The chosen gain must still keep offsets within the output range. A reset switch across the [capacitor](../../../../../../capacitor.md) can set the initial charge, while low-offset amplifiers, bias compensation and input offset adjustment reduce drift. Useful integration also requires frequencies below the amplifier's own response limit.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D12](../../d12.md)
3. [Section D](../../../section-d.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
