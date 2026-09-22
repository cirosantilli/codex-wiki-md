<h1 id="d/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

[Fubini's theorem](../../../../fubini-s-theorem.md) states that an absolutely integrable measurable function on a product of two $\sigma$-finite [measure spaces](../../../../measure-space.md) has integrable sections almost everywhere, the corresponding iterated [integrals](../../../../integral-split.md) exist, and both orders equal its product [integral](../../../../integral-split.md). In particular, for $f\in L^1(\mathbb R^2)$,

$$
\iint f(x,y)\,dx\,dy=\int\left(\int f(x,y)\,dx\right)dy=\int\left(\int f(x,y)\,dy\right)dx.
$$

To establish integrability of the nonnegative function here, first use [Tonelli's theorem](../../../../tonelli-theorem.md): for a nonnegative measurable function the product [integral](../../../../integral-split.md) equals either iterated [integral](../../../../integral-split.md) with infinity allowed. This avoids assuming the conclusion needed for [Fubini's theorem](../../../../fubini-s-theorem.md).

If $\alpha\geq-1$, $\int_0^\infty(1+x+y)^\alpha dx=\infty$ for every fixed $y$. If $\alpha<-1$, it is

$$
\int_0^\infty(1+x+y)^\alpha dx=\frac{(1+y)^{\alpha+1}}{-\alpha-1}.
$$

The outer [integral](../../../../integral-split.md) is finite exactly when $\alpha+1<-1$, that is, $\alpha<-2$. In that case

$$
\boxed{\iint_{(0,\infty)^2}(1+x+y)^\alpha dx\,dy=\frac1{(-\alpha-1)(-\alpha-2)},\qquad f\in L^1\iff\alpha<-2.}
$$

For $-2\leq\alpha<-1$ the outer [integral](../../../../integral-split.md) diverges, including logarithmic divergence at $\alpha=-2$. Nonnegativity means finiteness of this [integral](../../../../integral-split.md) is exactly absolute integrability; after proving it, [Fubini's theorem](../../../../fubini-s-theorem.md) allows either order.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [D](../../d.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
