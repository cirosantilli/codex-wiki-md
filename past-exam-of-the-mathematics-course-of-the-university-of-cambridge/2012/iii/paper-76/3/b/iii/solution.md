<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The locally integrable [logarithm](../../../../../../../logarithm.md) has [distributional derivative](../../../../../../../distributional-derivative.md) $(\log|x|)'=\operatorname{PV}(1/x)$. By the [Fourier transform of a derivative](../../../../../../../fourier-transform-of-a-derivative.md) and the previous result,

$$
ik\widehat{\log|x|}(k)=-i\pi\operatorname{sgn}k.
$$

For $k\ne0$, this gives $-\pi/|k|$. At zero the expression must be extended as a [Hadamard finite-part integral](../../../../../../../hadamard-finite-part-integral.md), not treated as a locally integrable function. For example, define the [finite-part inverse-absolute-value distribution](../../../../../../../finite-part-inverse-absolute-value-distribution.md) by

$$
\langle T,\varphi\rangle=\int_{|k|<1}\frac{\varphi(k)-\varphi(0)}{|k|}\,dk+\int_{|k|\ge1}\frac{\varphi(k)}{|k|}\,dk.
$$

Then $kT=\operatorname{sgn}k$. Different reference cutoffs change $T$ only by a multiple of the [Dirac delta distribution](../../../../../../../dirac-delta-function.md). The general solution of the transform equation is consequently

$$
\boxed{\widehat{\log|x|}(k)=-\pi\operatorname{Pf}\frac1{|k|}+C\delta(k).}
$$

Indeed multiplication by $k$ annihilates only a delta term among distributions supported at zero; delta derivatives would generate additional nonzero terms. This supplies the precise interpretation of the paper's formula, and the convention-dependent constant $C$ need not be found.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 76](../../../../paper-76-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
