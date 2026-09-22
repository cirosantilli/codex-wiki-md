<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Here $I(0)=1/2$. First restrict $\|u'\|_\infty\leq\pi/12$. On that slope interval, the second derivative of $h(p)=1-\cos(\pi/3+p)$ is $\cos(\pi/3+p)\geq\cos(5\pi/12)>1/4$. [Taylor's theorem](../../../../../taylor-s-theorem.md) gives

$$
h(p)\geq h(0)+h'(0)p+\tfrac18p^2.
$$

The linear term integrates to zero because $\int_0^1u'=0$. Since $x^3\leq1$, the [Poincaré inequality](../../../../../poincare-inequality.md) yields

$$
I(u)-I(0)\geq\frac18\int_0^1(u')^2-\int_0^1u^2
\geq\left(\frac18-\frac1{\pi^2}\right)\int_0^1(u')^2.
$$

The coefficient is positive. Thus **zero is a strict weak local minimizer**.

For failure of strong minimality, take a triangular bump supported on $[1/2-\varepsilon,1/2+\varepsilon]$, with slopes $+2\pi$ and $-2\pi$, and zero outside. Its height is $2\pi\varepsilon\to0$. [Almost everywhere](../../../../../almost-everywhere.md) its slope is $0$ or $\pm2\pi$, so the cosine term has exactly its zero-function value everywhere. The potential term is strictly negative on the bump. Therefore

$$
I(u_\varepsilon)-I(0)=-\int_0^1x^3u_\varepsilon^2\,dx<0,
\qquad\|u_\varepsilon\|_\infty\to0.
$$

Hence **it is not a strong local minimizer**. The derivatives of these bumps stay large, so they do not contradict weak local minimality.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the calculus of variations course of the University of Oxford](../../../../split.md)
6. [Calculus of variations course of the University of Oxford](../../../../../calculus-of-variations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
