<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Construct the vectors inductively by the [Gram-Schmidt process](../../../gram-schmidt-process.md), proving its needed properties directly. Suppose $w_1,\ldots,w_{j-1}$ form an [orthonormal basis](../../../orthonormal-basis.md) of $U_{j-1}$, and put

$$
r_j=u_j-\sum_{k<j}\langle u_j,w_k\rangle w_k.
$$

For every $i<j$, taking an [inner product](../../../inner-product-split.md) with $w_i$ gives $\langle r_j,w_i\rangle=0$. Also $r_j\ne0$, because otherwise $u_j$ would lie in the [linear span](../../../linear-span.md) of its predecessors, contrary to [linear independence](../../../linear-independence.md). Define

$$
\boxed{w_j=r_j/\|r_j\|.}
$$

It lies in $U_j$, has unit [norm](../../../norm.md), and is orthogonal to every $u_i$ with $i<j$, since those vectors lie in $U_{j-1}$. Writing $u_j=r_j+\sum_{k<j}\langle u_j,w_k\rangle w_k$ gives $\langle w_j,u_j\rangle=\|r_j\|>0$. The same identity shows that $w_1,\ldots,w_j$ span $U_j$, completing the induction, including the empty sum at $j=1$.

For uniqueness, any candidate $w\in U_j$ expands in the basis $w_1,\ldots,w_{j-1},r_j$. Orthogonality to every earlier $u_i$, hence to every earlier $w_i$, makes its first $j-1$ coefficients zero. Thus $w=tr_j$. Unit norm forces $t=\pm1/\|r_j\|$, and $\langle w,u_j\rangle>0$ forces the positive sign. This proves [uniqueness in the Gram-Schmidt process with positive normalization](../../../uniqueness-in-the-gram-schmidt-process-with-positive-normalization.md) without assuming a projection theorem or any other major orthogonalization result.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2006](../../2006-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
