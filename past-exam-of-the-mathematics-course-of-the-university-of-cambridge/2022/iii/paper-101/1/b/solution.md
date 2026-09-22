<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume first that $f\ne0$ and let

$$
d=\operatorname{ord}_{(x,y)}f
$$

be the least total degree of a nonzero homogeneous part of $f$. The [associated graded ring](../../../../../../associated-graded-ring.md) is

$$
\operatorname{gr}_{\mathfrak m}A
\simeq k[x,y]/(f_d),
$$

where $f_d$ is the initial homogeneous form. Multiplication by the nonzero polynomial $f_d$ is injective in $k[x,y]$, so the degree-$j$ component has dimension

$$
\dim_k(\operatorname{gr}_{\mathfrak m}A)_j
=\begin{cases}j+1,&j<d,\\d,&j\geq d.\end{cases}
$$

Summing the components of degrees below $n$ gives

$$
\boxed{
\chi(A,\mathfrak m;n)=
\begin{cases}
n(n+1)/2,&n\leq d,\\
dn-d(d-1)/2,&n\geq d.
\end{cases}}
$$

Thus the [Hilbert polynomial](../../../../../../hilbert-polynomial.md) is

$$
\boxed{P(n)=dn-\frac{d(d-1)}2.}
$$

Its leading coefficient is the order of vanishing, or multiplicity, of the plane curve $f=0$ at the origin. If $f=0$, no relation is imposed and $\chi=n(n+1)/2$ for every $n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
