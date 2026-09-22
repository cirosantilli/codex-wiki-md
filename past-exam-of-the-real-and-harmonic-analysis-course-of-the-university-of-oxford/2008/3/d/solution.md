<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Fourier coefficient of a measure on the circle](../../../../fourier-coefficient-of-a-measure-on-the-circle.md) and [convolution of measures on the circle](../../../../convolution-of-measures-on-the-circle.md) use the angular group law:

$$
\widehat\mu(n)=\int_{\mathbb T}e^{-inx}\,d\mu(x),\qquad
(\mu*\nu)(E)=\int_{\mathbb T}\int_{\mathbb T}\mathbf1_E(x+y)\,d\mu(x)d\nu(y).
$$

Addition is modulo $2\pi$. This is the pushforward of the product [complex measure](../../../../complex-measure.md) under addition; equivalently its integral against a continuous $f$ is $\iint f(x+y)d\mu(x)d\nu(y)$. The integrands are bounded and the variation [measures](../../../../measure-split.md) finite, so Fubini applies. In particular,

$$
\widehat{\mu*\nu}(n)=\iint e^{-in(x+y)}d\mu(x)d\nu(y)=\left(\int e^{-inx}d\mu(x)\right)\left(\int e^{-iny}d\nu(y)\right).
$$

Thus **$\widehat{\mu*\nu}(n)=\widehat\mu(n)\widehat\nu(n)$**. These [measure](../../../../measure-split.md) coefficients use no additional Haar normalization factor: a [probability](../../../../probability.md) has zeroth coefficient one.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../split.md)
5. [Real and harmonic analysis course of the University of Oxford](../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
