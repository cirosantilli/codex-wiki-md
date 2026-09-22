<h1 id="12f/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Since the common [radius of convergence](../../../../../../../radius-of-convergence.md) is infinite, the [termwise differentiation of a power series](../../../../../../../termwise-differentiation-of-a-power-series.md) theorem applies on the entire real line. For the even series, differentiation and the index change $m=n-1$ give

$$
f'(x)=\sum_{n=1}^\infty(-1)^n\frac{x^{2n-1}}{(2n-1)!}
=-\sum_{m=0}^\infty(-1)^m\frac{x^{2m+1}}{(2m+1)!}=-g(x).
$$

The odd series similarly gives $g'(x)=\sum_{n=0}^\infty(-1)^n x^{2n}/(2n)!=f(x)$. Thus **$\boxed{f'=-g,\qquad g'=f}$** everywhere. By the [product rule](../../../../../../../product-rule.md),

$$
\frac d{dx}(f^2+g^2)=2ff'+2gg'=-2fg+2gf=0.
$$

The [mean value theorem](../../../../../../../mean-value-theorem.md) implies that a differentiable function with zero derivative is constant on the real line. At zero, the series give $f(0)=1$ and $g(0)=0$. Consequently **$\boxed{f(x)^2+g(x)^2=1\text{ for every }x\in\mathbb R}$**. This derives the identity from the [power series](../../../../../../../power-series.md) without assuming a trigonometric identity in advance.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [12F](../../../12f.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
