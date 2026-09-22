<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

For real $b\ne0$, the integrand depends only on $b^2$, so first take $b>0$. Integrate $e^{iz}/(z^2-b^2)$ over the upper-half-plane semicircle, indenting above both real poles with small clockwise semicircles. The large arc tends to zero by [Jordan lemma](../../../../../jordan-s-lemma.md). Each indentation contributes $-i\pi$ times its [residue](../../../../../residue.md), and there are no enclosed poles. Thus the [Cauchy principal value](../../../../../cauchy-principal-value.md) on the whole real axis is

$$
\operatorname{PV}\int_{-\infty}^{\infty}\frac{e^{iu}}{u^2-b^2}\,du=i\pi\left(\frac{e^{ib}}{2b}-\frac{e^{-ib}}{2b}\right)=-\frac{\pi\sin b}{b}.
$$

The imaginary part is odd and the real part even. Taking the real part and halving gives

$$
\boxed{\operatorname{PV}\int_0^\infty\frac{\cos u}{u^2-b^2}\,du=-\frac{\pi\sin b}{2b}.}
$$

The right-hand side is even in $b$, completing the negative-$b$ case as well.

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
