<h1 id="p/p3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If the error is [orthogonal](../../../../../orthogonal-vectors.md) to $\Pi_n$, then for any $q\in\Pi_n$,

$$
\|u-q\|^2=\|u-p_n\|^2+\|p_n-q\|^2\geq\|u-p_n\|^2,
$$

proving sufficiency. Conversely, if $p_n$ minimizes, perturb it to $p_n+tq$ for any real $t$. The squared error becomes

$$
\|u-p_n\|^2-2t(u-p_n,q)+t^2\|q\|^2.
$$

A minimum at $t=0$ forces the linear coefficient to vanish, proving necessity.

For existence, choose the [basis](../../../../../basis.md) $1,x,\ldots,x^n$. Its [Gram matrix](../../../../../gram-matrix.md) $G$ is positive definite because $c^TGc$ is the squared [norm](../../../../../norm.md) of the nonzero [polynomial](../../../../../polynomial-split.md) with coefficients $c$. Thus $G$ is invertible, and the normal equations $Gc=((u,x^j))_{j=0}^n$ have a solution, giving an [orthogonal](../../../../../orthogonal-vectors.md) residual and therefore a minimizer. The Pythagorean identity shows any other minimizer differs by a [polynomial](../../../../../polynomial-split.md) of zero [norm](../../../../../norm.md), so it is equal to the first. Hence the best [polynomial](../../../../../polynomial-split.md) exists and is unique.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [P3](../../p3.md)
3. [P](../../../p.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
