<h1 id="12f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $E_* =\inf_{\deg q\leq n}\|f-q\|_\infty$, and choose a minimizing sequence $p_m$ with $\|f-p_m\|_\infty\to E_*$. Since $E_*\leq\|f\|_\infty$, discarding finitely many terms ensures $\|p_m\|_\infty\leq2\|f\|_\infty+1$.

Fix $n+1$ distinct nodes $a_0,\ldots,a_n$. The [Lagrange interpolation](../../../../../../lagrange-polynomial.md) formula expresses

$$
p_m(x)=\sum_{j=0}^np_m(a_j)\ell_j(x),\qquad \ell_j(x)=\prod_{k\ne j}\frac{x-a_k}{a_j-a_k}.
$$

The vector of node values is bounded in $\mathbb R^{n+1}$, so the [Bolzano-Weierstrass theorem](../../../../../../bolzano-weierstrass-theorem.md) supplies a subsequence converging to $(v_0,\ldots,v_n)$. Put $p=\sum v_j\ell_j$, of degree at most $n$. Because the $\ell_j$ are fixed bounded functions,

$$
\|p_m-p\|_\infty\leq\sum_j|p_m(a_j)-v_j|\,\|\ell_j\|_\infty\longrightarrow0
$$

along that subsequence. The [reverse triangle inequality](../../../../../../reverse-triangle-inequality.md) implies $\|f-p\|_\infty=E_*$. Thus a [best uniform approximation](../../../../../../best-uniform-approximation.md) exists, with no appeal to an unproved abstract existence result.

Here $\mathcal P_n$ is the vector space of real polynomials of degree at most $n$.

$$
\boxed{\exists p\in\mathcal P_n:\quad\|f-p\|_\infty=\inf_{q\in\mathcal P_n}\|f-q\|_\infty.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [12F](../../12f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
