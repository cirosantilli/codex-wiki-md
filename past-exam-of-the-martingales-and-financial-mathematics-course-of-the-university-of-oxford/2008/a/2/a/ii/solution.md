<h1 id="a/2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\mu_X$ be the distribution measure of $X$. The measurable change-of-variables rule for expectations gives

$$
\mathbb EX=\int_{\mathbb R}x\,\mu_X(dx)=\int_{\mathbb R}x\,dF(x).
$$

For the second equality, let $U$ be uniform on $(0,1)$ and $Q=F^\leftarrow$. The [quantile function](../../../../../../quantile-function.md) is measurable and satisfies

$$
Q(u)\leq x\quad\Longleftrightarrow\quad u\leq F(x).
$$

This equivalence uses monotonicity and right-continuity of $F$. Consequently $\mathbb P(Q(U)\leq x)=F(x)$: $Q(U)$ has the same distribution as $X$. In particular $\int_0^1|Q(u)|\,du=\mathbb E|X|<\infty$, so the signed integral is legitimate. Hence the [quantile expectation formula](../../../../../../quantile-expectation-formula.md) is

$$
\boxed{\mathbb EX=\int_{\mathbb R}x\,dF(x)
=\int_0^1F^\leftarrow(u)\,du.}
$$

No continuity or strict increase of the distribution function is required.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../../split.md)
7. [Martingales and financial mathematics course of the University of Oxford](../../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
