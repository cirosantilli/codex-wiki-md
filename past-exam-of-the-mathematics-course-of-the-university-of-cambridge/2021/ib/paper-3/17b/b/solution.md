<h1 id="17b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose $m<n$. The [Rodrigues' formula](../../../../../../rodrigues-formula.md) and $n$ integrations by parts give

$$
\begin{aligned}
\langle p_n,p_m\rangle
&=(-1)^n\int_0^\infty
p_m(x)\frac{d^n}{dx^n}
\left(x^{n+1/2}e^{-x}\right)dx\\
&=\int_0^\infty
p_m^{(n)}(x)x^{n+1/2}e^{-x}\,dx=0,
\end{aligned}
$$

because $p_m^{(n)}=0$. Every boundary term vanishes: the exponential controls infinity, while the remaining power of $x$ has positive exponent at zero. Symmetry of the [inner product](../../../../../../inner-product.md) gives orthogonality whenever $m\ne n$.

For the norm, monicity gives $p_n^{(n)}=n!$, so the same calculation yields

$$
\boxed{
\langle p_n,p_n\rangle
=n!\int_0^\infty x^{n+1/2}e^{-x}\,dx
=n!\,\Gamma\!\left(n+\frac32\right)
}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17B](../../17b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
