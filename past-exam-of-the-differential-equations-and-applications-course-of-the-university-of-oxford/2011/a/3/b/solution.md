<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

There is a normalization conflict in the source: the printed [Rodrigues' formula](../../../../../rodrigues-formula.md) gives the standard [Generalized Laguerre polynomial](../../../../../generalized-laguerre-polynomial.md) $P_n=L_n^{(m)}$ with $P_n(0)=\binom{n+m}{n}$, which is generally not one. The norm requested here corresponds to that Rodrigues normalization. A solution normalized to one at zero is $\widehat P_n=P_n/\binom{n+m}{n}$.

Set $w=x^me^{-x}$ and $p=x^{m+1}e^{-x}$. The equation becomes $(pP_n')'+nwP_n=0$. Multiply the equations for $P_n,P_k$ by the opposite [polynomial](../../../../../polynomial-split.md), subtract and integrate. The boundary term $p(P_n'P_k-P_k'P_n)$ vanishes at zero and infinity, so

$$
(n-k)\int_0^\infty wP_nP_k\,dx=0.
$$

This proves [orthogonality](../../../../../orthogonal-vectors.md) for $k\ne n$ under either normalization.

For the squared norm, use the printed [Rodrigues' formula](../../../../../rodrigues-formula.md) and integrate by parts $n$ times:

$$
\int_0^\infty wP_n^2\,dx
=\frac1{n!}\int_0^\infty P_nD^n(x^{n+m}e^{-x})\,dx
=\frac{(-1)^n}{n!}\int_0^\infty P_n^{(n)}x^{n+m}e^{-x}\,dx.
$$

All boundary terms vanish: the required derivatives have a positive power of $x$ at zero and exponential decay at infinity. The leading coefficient is $(-1)^n/n!$, so $P_n^{(n)}=(-1)^n$. The [Gamma function](../../../../../gamma-function.md) integral gives

$$
\boxed{\int_0^\infty x^me^{-x}P_n(x)^2\,dx=\frac{(n+m)!}{n!}.}
$$

For the source's alternative unit-at-zero normalization the correct answer instead is

$$
\boxed{\int_0^\infty x^me^{-x}\widehat P_n(x)^2\,dx=\frac{(n+m)!}{n!\binom{n+m}{n}^2}.}
$$

Both cannot equal the printed norm when $m,n>0$. This distinction is the [normalization of generalized Laguerre polynomials](../../../../../normalization-of-generalized-laguerre-polynomials.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
