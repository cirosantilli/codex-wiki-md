<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $Y(\theta)=y(\cos\theta)$ for $0\leq\theta\leq\pi$. The [chain rule](../../../../../../chain-rule.md) gives

$$
y'=-\frac{Y'}{\sin\theta},\qquad y''=\frac{Y''}{\sin^2\theta}-\frac{\cos\theta}{\sin^3\theta}Y'.
$$

Substitution cancels the first-derivative terms and leaves $-Y''=n^2Y$. The endpoint conditions become $Y(0)=Y(\pi)=0$. For $n\ne0$, the first condition selects $Y=A\sin(n\theta)$, and the second requires $\sin(n\pi)=0$. Thus a nonzero solution requires an integer $n$. The case $n=0$ gives $Y=A+B\theta$ and both conditions force it to vanish. Negative integers give the same eigenvalues and eigenfunctions up to sign, so take $n=1,2,\ldots$.

For [vector normalization](../../../../../../vector-normalization.md), use $w(x)dx=-d\theta$:

$$
1=\int_{-1}^1w(x)|y_n(x)|^2dx=|A|^2\int_0^\pi\sin^2(n\theta)d\theta=|A|^2\frac\pi2.
$$

Choosing a positive real normalization constant gives

$$
\boxed{y_n(x)=\sqrt{\frac2\pi}\sin(n\arccos x)=\sqrt{\frac2\pi}\sqrt{1-x^2}\,U_{n-1}(x),\qquad\lambda_n=n^2.}
$$

Here $U_{n-1}$ is the [Chebyshev polynomial of the second kind](../../../../../../chebyshev-polynomial-of-the-second-kind.md). The factors $\sqrt{1-x^2}$ make both endpoint values zero. The derivatives need not stay finite there; instead $py_n'=-n\sqrt{2/\pi}\cos(n\theta)$ has finite endpoint limits, ensuring that the relevant boundary form vanishes.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
