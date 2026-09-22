<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [principal-value reciprocal distribution](../../../../../../principal-value-reciprocal-distribution.md) is

$$
\left\langle\operatorname{pv}\frac1x,\varphi\right\rangle
=\lim_{\varepsilon\downarrow0}\int_{|x|>\varepsilon}\frac{\varphi(x)}x\,dx.
$$

The limit exists because the constant part of the numerator cancels symmetrically at zero. Multiplying by $x$ gives $x\operatorname{pv}(1/x)=1$.

If $v$ is any other solution, $w=v-\operatorname{pv}(1/x)$ obeys $xw=0$. To identify this [kernel of multiplication by a coordinate](../../../../../../kernel-of-multiplication-by-a-coordinate.md), choose a [cutoff function](../../../../../../cutoff-function.md) $\eta$ equal to one near zero. Every test function has the form $\varphi=\varphi(0)\eta+x\psi$ with $\psi\in\mathcal D$. Thus $\langle w,\varphi\rangle=\varphi(0)\langle w,\eta\rangle$, proving $w=c\delta_0$. Therefore

$$
\boxed{v=\operatorname{pv}\frac1x+c\delta_0,\qquad c\in\mathbb C.}
$$

For real distributions the constants are real.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
