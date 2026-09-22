<h1 id="u/u2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $e_k=x_k-x_*$, with $f'(x_*)=0$, $f''(x_*)\ne0$. [Taylor expansion](../../../../../../taylor-expansion.md) gives

$$
f'(x_*+e)=f''(x_*)e+\tfrac12f^{(3)}(x_*)e^2+O(e^3),\qquad f''(x_*+e)=f''(x_*)+f^{(3)}(x_*)e+O(e^2).
$$

Division in the Newton update yields

$$
\boxed{e_{k+1}=\frac{f^{(3)}(x_*)}{2f''(x_*)}e_k^2+O(e_k^3).}
$$

Thus convergence is generically quadratic when that coefficient is nonzero. With a locally Lipschitz second [derivative](../../../../../../derivative.md) and nonzero $f''(x_*)$, the weaker estimate $|e_{k+1}|\le C|e_k|^2$ also proves local [quadratic convergence](../../../../../../quadratic-convergence.md).

**“Quadratic at best” is false as a universal upper bound.** If the displayed coefficient vanishes, the order can be higher. For example $f(x)=x^2/2+x^4/4$ has a [minimum](../../../../../../local-minimum.md) at zero, and its [Newton optimization](../../../../../../newton-root-finding-iteration.md) update is $x_{k+1}=2x_k^3/(1+3x_k^2)$, which has [cubic convergence](../../../../../../cubic-convergence.md). For a nondegenerate quadratic objective the method reaches the [stationary point](../../../../../../stationary-point.md) in one step. The expansion proves the standard generic quadratic statement while retaining and correcting the source's stronger wording explicitly.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [U2](../../../u2.md)
4. [U](../../../../u.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
