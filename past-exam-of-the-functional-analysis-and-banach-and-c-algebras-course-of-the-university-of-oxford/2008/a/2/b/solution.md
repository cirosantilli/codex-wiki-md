<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $x-Sx$, choose the consecutive shifts $j_r=r$, $1\leq r\leq k$. The average telescopes:

$$
\frac1k\sum_{r=1}^k(\alpha_{n+r}-\alpha_{n+r+1})=\frac{\alpha_{n+1}-\alpha_{n+k+1}}k.
$$

Its absolute value is at most $2\|x\|_\infty/k$. Taking the [limit superior](../../../../../limit-superior.md) and then the infimum over $k$ proves **$q(x-Sx)\leq0$**.

For the requested functional, use the allowed sublinearity of $q$. On convergent sequences, every finite shifted average has the same limiting value, so $q$ equals the ordinary limit there. Hahn-Banach extends this limit to a linear $\psi$ satisfying $\psi\leq q\leq p$. Apply domination to $x-Sx$ and to $(-x)-S(-x)$ to obtain respectively $\psi(x-Sx)\leq0$ and $-\psi(x-Sx)\leq0$. Hence

$$
\boxed{\psi(x)=\psi(Sx),\qquad\psi(x)\leq\limsup_n\alpha_n.}
$$

This is a [Banach limit](../../../../../banach-limit.md); the two-sided limit bounds also show positivity, [norm](../../../../../norm.md) one, and agreement with ordinary limits.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
