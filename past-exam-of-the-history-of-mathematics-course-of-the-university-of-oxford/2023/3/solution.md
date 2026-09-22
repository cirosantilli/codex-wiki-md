<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[Alexandre-Théophile Vandermonde](../../../alexandre-theophile-vandermonde.md) presents a programme in [elimination theory](../../../elimination-theory.md): remove [unknowns](../../../unknown.md) from simultaneous [polynomial equations](../../../polynomial-equation.md) in a way that works uniformly as the number of [equations](../../../equation.md) and their [polynomial degrees](../../../degree-of-a-polynomial.md) vary. The immediate achievement is narrower than that programme: a general construction for [linear equations](../../../linear-equation.md). The academy year 1772 used in the exam is not the printing date of the memoir, which appeared in 1776. Its compact indices distinguished the equation containing a [coefficient](../../../coefficient.md) from the [unknown](../../../unknown.md) it multiplied; they were not powers. That notational separation is crucial to interpreting the work.[Opening, printed pp. 516–517; academy year 1772, printed 1776](../../../memoire-sur-l-elimination-by-alexandre-theophile-vandermonde.md)[§2.1, discussion and reproduction of Vandermonde's coefficient notation; bibliography](../../../a-case-of-mathematical-eponymy-the-vandermonde-determinant-by-bernard-ycart.md)

In modern language take a [system of linear equations](../../../system-of-linear-equations.md) $A\mathbf{x}=\mathbf{b}$ with $n$ [unknowns](../../../unknown.md). Its [determinant](../../../determinant.md) is an alternating expression in the [coefficients](../../../coefficient.md):

$$
D=\det A=\sum_{\pi\in S_n}\operatorname{sgn}(\pi)\prod_{i=1}^n a_{i,\pi(i)}.
$$

Each [product](../../../product-of-numbers.md) selects one [coefficient](../../../coefficient.md) from each equation and each [unknown](../../../unknown.md)'s column. The [sign of a permutation](../../../sign-of-a-permutation.md) determines whether it is added or subtracted. This makes the number $n$ a genuine parameter of a general rule, rather than merely supplying separately memorised formulas for two or three [unknowns](../../../unknown.md). The notation here is modern, not a transcription of [Alexandre-Théophile Vandermonde](../../../alexandre-theophile-vandermonde.md)'s symbols.

For two [unknowns](../../../unknown.md), multiply $ax+by=u$ by $d$ and $cx+dy=v$ by $b$, then subtract. Similarly eliminate $x$. This gives

$$
(ad-bc)x=du-bv,\qquad(ad-bc)y=av-cu.
$$

The same principle in arbitrary size is [Cramer's rule](../../../cramer-s-rule.md). If $A_j(\mathbf{b})$ is obtained by replacing column $j$ of $A$ by $\mathbf{b}$, then

$$
\boxed{x_j=\frac{\det A_j(\mathbf{b})}{\det A}\quad\text{when }\det A\ne0.}
$$

An original verification uses the [multilinearity of the determinant](../../../multilinearity-of-the-determinant.md): replace $\mathbf{b}$ by the column combination $\sum_k x_k A_k$. Every resulting [determinant](../../../determinant.md) vanishes through repeated columns except the $k=j$ term, which is $x_j\det A$. This explains how an elimination expression isolates one [unknown](../../../unknown.md).

The condition $D\ne0$ is substantive. If $D=0$, multiplying by an expression which vanishes cannot justify division. For instance, $x+y=1$ and $2x+2y=3$ are inconsistent, whereas replacing $3$ by $2$ gives infinitely many solutions. Thus an elimination formula must distinguish exceptional [coefficients](../../../coefficient.md) and preserve the connection to the original [system of linear equations](../../../system-of-linear-equations.md). Nor does the displayed rule solve the much broader problem of arbitrary [nonlinear equations](../../../nonlinear-equation.md).

The passage's importance is **the move from particular elimination calculations towards a theory of alternating expressions**. It would be misleading to turn this into the claim that the familiar [Vandermonde determinant](../../../vandermonde-determinant.md), formed from powers of variables, is what this extract displays. A positional upper index and an exponent have different meanings; the history of that eponym requires separate evidence. Likewise, modern [matrix algebra](../../../matrix-algebra.md) is a useful explanatory language here, not the institutional or conceptual setting of an eighteenth-century memoir.[§§2.1–2.4, separating coefficient indices, difference-products and the later eponym](../../../a-case-of-mathematical-eponymy-the-vandermonde-determinant-by-bernard-ycart.md)

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2023](../../2023-split.md)
3. [Past exam of the history of mathematics course of the University of Oxford](../../split.md)
4. [History of mathematics course of the University of Oxford](../../../history-of-mathematics-course-of-the-university-of-oxford.md)
5. [Year 3 of the mathematics course of the University of Oxford](../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
