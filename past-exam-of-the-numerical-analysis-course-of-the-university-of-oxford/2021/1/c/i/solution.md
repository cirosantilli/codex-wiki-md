<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $L_{n+1}$ denote the conventional [Legendre polynomial](../../../../../legendre-polynomial.md), normalized by $L_{n+1}(1)=1$. The $n+1$ [quadrature nodes](../../../../../quadrature-node.md) are its distinct [polynomial roots](../../../../../root-of-a-polynomial.md) in $(-1,1)$. For these nodes form the [Lagrange cardinal polynomials](../../../../../lagrange-cardinal-polynomial.md)

$$
\ell_i(x)=\prod_{\substack{0\leq j\leq n\\j\ne i}}
\frac{x-x_j}{x_i-x_j}
=\frac{L_{n+1}(x)}{(x-x_i)L_{n+1}'(x_i)}.
$$

Choose the [quadrature weights](../../../../../quadrature-weight.md) by integrating these [polynomials](../../../../../polynomial-split.md):

$$
\boxed{w_i=\int_{-1}^1\ell_i(x)\,dx,\qquad
\widehat I_n(f)=\sum_{i=0}^nw_if(x_i).}
$$

An equivalent standard formula is

$$
\boxed{w_i=\frac{2}{(1-x_i^2)[L_{n+1}'(x_i)]^2}.}
$$

The reason for selecting these [quadrature nodes](../../../../../quadrature-node.md) is the resulting [degree of precision of a quadrature rule](../../../../../degree-of-precision-of-a-quadrature-rule.md). For any [polynomial](../../../../../polynomial-split.md) $p$ of [polynomial degree](../../../../../degree-of-a-polynomial.md) at most $2n+1$, [polynomial division](../../../../../polynomial-division.md) gives

$$
p=L_{n+1}s+r,\qquad \deg s\leq n,\quad\deg r\leq n.
$$

The [orthogonality](../../../../../orthogonal-vectors.md) of the [Legendre polynomial](../../../../../legendre-polynomial.md) makes $\int_{-1}^1L_{n+1}s=0$, while $p(x_i)=r(x_i)$ at each [quadrature node](../../../../../quadrature-node.md). The definition of the [quadrature weights](../../../../../quadrature-weight.md) integrates $r$ exactly, so

$$
\boxed{\widehat I_n(p)=\int_{-1}^1p(x)\,dx\qquad(\deg p\leq2n+1).}
$$

In particular, $\sum_iw_i=2$. Applying this exactness to $\ell_i^2$ also proves $w_i=\int_{-1}^1\ell_i(x)^2dx>0$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
