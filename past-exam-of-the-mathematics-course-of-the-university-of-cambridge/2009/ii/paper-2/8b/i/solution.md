<h1 id="8b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the sign convention in the question: the [Hilbert transform](../../../../../../hilbert-transform.md) kernel is $(y-x)^{-1}$, the negative of another common convention. A contour indentation at the origin gives

$$
\operatorname{pv}\int_{\mathbb R}\frac{e^{isy}}{y-x}\,dy=i\pi\operatorname{sgn}(s)e^{isx}.
$$

For $s>0$ close the contour in the upper half-plane; for $s<0$ close it below. Thus the transform of $\sin(sx)$ is $\cos(sx)$ for $s>0$. Since $(1-\cos x)/x=\int_0^1\sin(sx)\,ds$, integration of this multiplier identity, justified first with an Abel regularization, yields

$$
\boxed{\widehat f(x)=\frac{\sin x}{x},\qquad\widehat f(0)=1.}
$$

The value at zero also follows directly from $\pi^{-1}\int(1-\cos y)y^{-2}\,dy=1$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [8B](../../8b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
