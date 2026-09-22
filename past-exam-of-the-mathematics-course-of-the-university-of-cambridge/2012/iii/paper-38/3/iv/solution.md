<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $x>\mu$, the corresponding smaller root is $\mu^2/x$. The [conditional probability](../../../../../../conditional-probability.md) of selecting the larger root is

$$
1-\frac{\mu}{\mu+\mu^2/x}
=\frac{\mu}{\mu+x}.
$$

It is the same weight as a function of the actual selected value $x$. Hence

$$
p_+(x)=\frac{\mu}{\mu+x}\,g(h(x))\,|h'(x)|
=\sqrt{\frac{\lambda}{2\pi x^3}}
\exp\!\left(-\frac{\lambda(x-\mu)^2}{2\mu^2x}\right).
$$

Combining the two open intervals proves **the output has the [Inverse Gaussian distribution](../../../../../../inverse-gaussian-distribution.md) $IG(\mu,\lambda)$**. The event $Y=0$ has probability zero, so no atom occurs at $\mu$; the limiting density there is finite. The algorithm always selects one of its positive roots, so these branch densities exhaust its [probability distribution](../../../../../../probability-distribution.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
