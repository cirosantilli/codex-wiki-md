<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

The [monomials](../../../../../monomial.md) $1,x,\ldots,x^n$ are linearly independent and span, so $\boxed{\dim_{\mathbb C}V=n+1}$. Use the [factorial monomial basis for polynomial differentiation](../../../../../factorial-monomial-basis-for-polynomial-differentiation.md) $p_j(x)=x^j/j!$, $0\leq j\leq n$. Direct differentiation gives $e_i(p_j)=\delta_{ij}$. Hence

$$
\boxed{(e_0,e_1,\ldots,e_n)\text{ is a basis of }V^*,\qquad(p_0,p_1,\ldots,p_n)\text{ is its dual basis in }V.}
$$

Indeed every $\phi\in V$ has the Taylor expansion $\phi=\sum_{j=0}^ne_j(\phi)p_j$; evaluation on the $p_j$ proves independence of the functionals. Derivative orders include zero. If one uses a convention excluding zero from $\mathbb N$, $e_0$ must explicitly be included, since all positive-order derivatives annihilate constants and cannot span the [dual space](../../../../../dual-space.md).

Differentiation satisfies $Dp_0=0$ and $Dp_j=p_{j-1}$ for $j\geq1$. With column vectors of coefficients, its [matrix](../../../../../matrix.md) $A$ has entries $A_{ij}=1$ if $j=i+1$ and zero otherwise, for indices $0\leq i,j\leq n$:

$$
\boxed{[D]=\begin{pmatrix}0&1&0&\cdots&0\\0&0&1&\cdots&0\\\vdots&\vdots&\ddots&\ddots&\vdots\\0&0&\cdots&0&1\\0&0&\cdots&0&0\end{pmatrix}.}
$$

The [dual map](../../../../../transpose-of-a-linear-map.md) is $D^*(\ell)=\ell\circ D$, not a conjugate-linear adjoint. Thus $D^*e_i=e_{i+1}$ for $i<n$ and $D^*e_n=0$. Therefore $\boxed{[D^*]=[D]^T}$ in the corresponding [dual basis](../../../../../dual-basis.md). For $n=0$ both matrices are the one-by-one zero [matrix](../../../../../matrix.md).

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
