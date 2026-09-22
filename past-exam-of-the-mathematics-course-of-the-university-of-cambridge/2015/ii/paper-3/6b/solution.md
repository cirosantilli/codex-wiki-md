<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

Use equal small excisions on the two sides of each real pole. The [Cauchy principal value](../../../../../cauchy-principal-value.md) is

$$
\lim_{R\to\infty}\lim_{\epsilon\downarrow0}\left(\int_{-R}^{-a-\epsilon}+\int_{-a+\epsilon}^{a-\epsilon}+\int_{a+\epsilon}^{R}\right)\frac{\cos x}{x^2-a^2}\,dx.
$$

For $e^{iz}/(z^2-a^2)$, close the [complex contour](../../../../../complex-contour.md) in the upper half-plane and indent above $\pm a$, leaving the poles outside the contour. The [residue theorem](../../../../../residue-theorem.md) and the vanishing of the large semicircle integral give the principal-value integral as $i\pi$ times the sum of the two real-pole [residues](../../../../../residue.md). Each clockwise indentation contributes $-i\pi$ times its residue. Since

$$
\operatorname{Res}_{a}\frac{e^{iz}}{z^2-a^2}=\frac{e^{ia}}{2a},\qquad \operatorname{Res}_{-a}\frac{e^{iz}}{z^2-a^2}=-\frac{e^{-ia}}{2a},
$$

the sum is $i\sin a/a$. Taking the real part yields **the answer**

$$
\boxed{\operatorname{PV}\int_{-\infty}^{\infty}\frac{\cos x}{x^2-a^2}\,dx=-\frac{\pi\sin a}{a}.}
$$

The decay on the large arc follows directly from $|e^{iz}|\leq1$ and the quadratic denominator.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
