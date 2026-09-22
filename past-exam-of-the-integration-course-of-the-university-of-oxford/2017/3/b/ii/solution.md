<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Because $f$ is [continuous](../../../../../continuous-function.md), $g(x,y)=e^{-x^2}f(e^{-x^2/2}y)$ is continuous on $\mathbb R^2$, so $|g|$ is a nonnegative measurable function. Apply [Tonelli's theorem](../../../../../tonelli-theorem.md) before assuming integrability. For each fixed $x$, set $z=e^{-x^2/2}y$, so $dy=e^{x^2/2}\,dz$. [Lebesgue substitution on an interval](../../../../../lebesgue-substitution-on-an-interval.md) gives

$$
\int_{\mathbb R}|g(x,y)|\,dy
=e^{-x^2/2}\int_{\mathbb R}|f(z)|\,dz.
$$

Therefore the [Gaussian integral](../../../../../gaussian-integral.md) yields

$$
\boxed{\iint_{\mathbb R^2}|g(x,y)|\,dx\,dy
=\sqrt{2\pi}\int_{\mathbb R}|f(z)|\,dz<\infty.}
$$

This proves that $g$ is [Lebesgue integrable](../../../../../lebesgue-integrable-function.md) on $\mathbb R^2$. [Fubini's theorem](../../../../../fubini-s-theorem.md) now permits changing the order for $g$ itself. The same substitution without absolute values gives the stronger exact identity

$$
\int_{\mathbb R}\int_{\mathbb R}g(x,y)\,dx\,dy
=\sqrt{2\pi}\int_{\mathbb R}f(z)\,dz.
$$

Taking absolute values and using the [triangle inequality for an integral](../../../../../integral-triangle-inequality.md) proves

$$
\boxed{\left|\int_{\mathbb R}\int_{\mathbb R}g(x,y)\,dx\,dy\right|
\leq\sqrt{2\pi}\int_{\mathbb R}|f(z)|\,dz.}
$$

The constant is sharp: any nonzero nonnegative continuous integrable $f$ gives equality. This is a [weighted dilation kernel](../../../../../weighted-dilation-kernel.md) with $a(x)=e^{-x^2}$ and $b(x)=e^{-x^2/2}$. The inner $x$ integral in the requested order is guaranteed to be integrable for almost every $y$, which is all the iterated integral requires.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
