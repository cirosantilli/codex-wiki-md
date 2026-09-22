<h1 id="cauchy-binet-formula">Cauchy–Binet formula</h1>

↑ **Parent:** [Determinant](determinant.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cauchy–Binet_formula)

For [matrices](matrix.md) $A\in\mathbb R^{r\times m}$ and $B\in\mathbb R^{m\times r}$ with $r\leq m$,

$$
\det(AB)=\sum_{\substack{S\subseteq\{1,\ldots,m\}\\|S|=r}}\det A_{:,S}\det B_{S,:},
$$

where the indices of $S$ are taken in increasing order. To prove it, write the $j$th column of $AB$ as $\sum_q B_{qj}A_{:,q}$ and expand its [determinant](determinant.md) by multilinearity. Terms with a repeated $q$ vanish by alternation. For each remaining index set $S=\{s_1<\cdots<s_r\}$, collect all permutations $q_j=s_{\sigma(j)}$. The factor from $A$ is $\operatorname{sgn}(\sigma)\det A_{:,S}$; the sum of the products $\operatorname{sgn}(\sigma)\prod_j B_{s_{\sigma(j)},j}$ is $\det B_{S,:}$. This proves the formula. Applying it to selected rows and columns proves that a product of compatible [totally nonnegative matrices](total-nonnegativity-of-a-matrix.md) is totally nonnegative.

## ↑ Ancestors (7)

1. [Determinant](determinant.md)
2. [Multilinear algebra](multilinear-algebra.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-68/5/a/solution.md)
- [Total nonnegativity of a matrix](total-nonnegativity-of-a-matrix.md)
- [Total nonnegativity of B-spline collocation matrices](total-nonnegativity-of-b-spline-collocation-matrices.md)
