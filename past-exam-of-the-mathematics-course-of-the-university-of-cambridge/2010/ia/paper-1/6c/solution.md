<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

In an oriented orthonormal coordinate system, the [dot product](../../../../../dot-product.md) and [cross product](../../../../../cross-product.md) are

$$
a\cdot b=\sum_{k=1}^3a_kb_k,\qquad
 a\times b=(a_2b_3-a_3b_2,\ a_3b_1-a_1b_3,\ a_1b_2-a_2b_1).
$$

The [scalar triple product](../../../../../scalar-triple-product.md) is $a\cdot(b\times c)$; equivalently it is the [determinant](../../../../../determinant.md) of the [matrix](../../../../../matrix.md) whose columns are $a,b,c$. The three vectors have [linear independence](../../../../../linear-independence.md) when

$$
t_1a_1+t_2a_2+t_3a_3=0\ \Longrightarrow\ t_1=t_2=t_3=0.
$$

Let $U=(a_1\ a_2\ a_3)$ and $V=(b_1\ b_2\ b_3)$ be column [matrices](../../../../../matrix.md). Since $(U^TV)_{ij}=a_i\cdot b_j$, we have $S=U^TV$. Multiplicativity of the [determinant](../../../../../determinant.md) and its invariance under [matrix transpose](../../../../../transpose.md) yield

$$
\det S=\det(U^T)\det V=\det U\det V
=\boxed{\bigl(a_1\cdot(a_2\times a_3)\bigr)
\bigl(b_1\cdot(b_2\times b_3)\bigr)}.
$$

A square [matrix](../../../../../matrix.md) has maximal [matrix rank](../../../../../matrix-rank.md) exactly when its [determinant](../../../../../determinant.md) is nonzero, equivalently when its columns have [linear independence](../../../../../linear-independence.md). A product of two real numbers is nonzero exactly when both factors are nonzero. Hence $\boxed{\operatorname{rank}S=3\iff (a_i)_{i=1}^3\text{ and }(b_j)_{j=1}^3\text{ are both independent}}$.

The same argument works in every dimension. Set $U_n=(c_1\ \cdots\ c_n)$ and $V_n=(d_1\ \cdots\ d_n)$. Then

$$
T=U_n^TV_n,\qquad \det T=\det U_n\det V_n,
$$

so $\boxed{\operatorname{rank}T=n\iff(c_i)_{i=1}^n\text{ and }(d_j)_{j=1}^n\text{ are both independent}}$.

For the last construction, choose two [standard basis](../../../../../standard-basis.md) vectors $e_1,e_2$ in $\mathbb R^n$ and take $c_j=e_1+je_2$ for $j=1,\ldots,n$. If $\alpha c_i+\beta c_j=0$ with $i\ne j$, its first two coordinates give $\alpha+\beta=0$ and $i\alpha+j\beta=0$, hence $\alpha=\beta=0$. Every pair therefore has [linear independence](../../../../../linear-independence.md). Every triple lies in the two-dimensional [linear span](../../../../../linear-span.md) of $e_1,e_2$ and has [linear dependence](../../../../../linear-dependence.md). More explicitly, for distinct $i,j,k$,

$$
(j-k)c_i+(k-i)c_j+(i-j)c_k=0,
$$

a nontrivial dependence. Thus $\boxed{c_j=e_1+je_2\ (1\leq j\leq n)\text{ works for every }n>2}$.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
