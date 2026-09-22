<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Statistical homogeneity](../../../../../../statistical-homogeneity.md) makes the two-point [correlation](../../../../../../pearson-correlation-coefficient.md) depend on the displacement $\mathbf u=\mathbf r-\mathbf r'$. Substituting the [Fourier transforms](../../../../../../fourier-transform.md) and changing variables from $(\mathbf r,\mathbf r')$ to $(\mathbf u,\mathbf r')$ gives

$$
\begin{aligned}
\mathbb E[\widehat B_i(\mathbf k)\widehat B_j(\mathbf k')]
&=\int d^3u\,d^3r'\,C_{ij}(\mathbf u)e^{-i\mathbf k\cdot\mathbf u}e^{-i(\mathbf k+\mathbf k')\cdot\mathbf r'}\\
&=\widehat C_{ij}(\mathbf k)\int d^3r'\,e^{-i(\mathbf k+\mathbf k')\cdot\mathbf r'}.
\end{aligned}
$$

The last [integral](../../../../../../integral.md) is a [Dirac delta function](../../../../../../dirac-delta-function.md), so

$$
\boxed{\mathbb E[\widehat B_i(\mathbf k)\widehat B_j(\mathbf k')]=(2\pi)^3\delta(\mathbf k+\mathbf k')\widehat C_{ij}(\mathbf k).}
$$

The plus sign occurs because neither [Fourier transform](../../../../../../fourier-transform.md) has undergone [complex conjugation](../../../../../../complex-conjugation.md). For a real [magnetic field](../../../../../../magnetic-field.md), the version with $\widehat B_j(\mathbf k')^*$ instead has $\delta(\mathbf k-\mathbf k')$. Homogeneity determines dependence on the displacement vector; dependence only on its [norm](../../../../../../norm.md) needs [statistical isotropy](../../../../../../statistical-isotropy.md) as well.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
