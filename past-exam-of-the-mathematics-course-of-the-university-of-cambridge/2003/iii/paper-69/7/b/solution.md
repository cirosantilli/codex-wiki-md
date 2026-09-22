<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For distinct ordered knots, put $h_i=t_{i+1}-t_i>0$. The linear [B-spline](../../../../../../b-spline.md) $N_i$ is the triangular hat supported on $[t_i,t_{i+2}]$, equal to $(t-t_i)/h_i$ on its rising segment and $(t_{i+2}-t)/h_{i+1}$ on its falling segment. Its integral-normalized partner is $M_i=2N_i/(h_i+h_{i+1})$. Thus

$$
\int N_i^2=\frac{h_i+h_{i+1}}3,\qquad \int N_iN_{i-1}=\frac{h_i}6,\qquad \int N_iN_{i+1}=\frac{h_{i+1}}6.
$$

For example, the left overlap is $\int_0^{h_i}(u/h_i)(1-u/h_i)\,du=h_i/6$. Nonadjacent hats have disjoint interiors of their [supports](../../../../../../support.md), so their [inner product](../../../../../../inner-product.md) is zero. The [linear-spline mixed Gram matrix](../../../../../../linear-spline-mixed-gram-matrix.md) therefore has row

$$
\boxed{g_{ii}=\frac23,\quad g_{i,i-1}=\frac{h_i}{3(h_i+h_{i+1})},\quad g_{i,i+1}=\frac{h_{i+1}}{3(h_i+h_{i+1})},\quad g_{ij}=0\ (|i-j|\ge2)}.
$$

Retain only column indices in $1,\ldots,n$: the first or last row has no neighbor outside this range. Admissible repeated endpoint knots are obtained by a limit with zero spacings, provided $h_i+h_{i+1}>0$; a degenerate hat with zero support width is not a [basis](../../../../../../basis.md) element.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
