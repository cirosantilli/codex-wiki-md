<h1 id="b/7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $g(v)=-\cos(\pi v/2)$. For the stipulated $0<\delta<1$, the displayed tent is continuous at its junction, has zero endpoint values, and its slopes are $\delta$ and $\delta-4$. At both slopes $g'$ has the same value $c=(\pi/2)\sin(\pi\delta/2)>0$, and $g''=(\pi^2/4)\cos(\pi v/2)$ is strictly positive on common sufficiently small neighborhoods of them. [Taylor's theorem](../../../../../../taylor-s-theorem.md) gives, for small $\|\phi'\|_\infty$,

$$
I(u^\delta+\phi)-I(u^\delta)\geq c\int_0^1\phi'+c_0\int_0^1\phi'^2=c_0\int_0^1\phi'^2.
$$

Thus **$u^\delta$ is a strict [weak local minimizer of a variational integral](../../../../../../weak-local-minimizer-of-a-variational-integral.md)**. It is not a [strong local minimizer of a variational integral](../../../../../../strong-local-minimizer-of-a-variational-integral.md): the global supporting-tangent requirement at either slope has nonzero slope $c$, whereas $g$ is bounded. Letting the trial slope tend to positive infinity violates that requirement. The [Weierstrass necessary condition](../../../../../../weierstrass-necessary-condition.md) therefore fails.

The opening parameter range $\delta\in(0,1)$ is essential. The subsequent phrase “for each $\delta>0$” must be read within it; taken literally beyond that range it is false. At $\delta=2$ the tent slopes are $2,-2$, where $g=1$ and $g''<0$, so this is not a weak minimum.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [B](../../../../b.md)
5. [2007](../../../../../2007-split.md)
6. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../split.md)
7. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
