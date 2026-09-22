<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $\boxed{p(x)=x(L-x)}$. It vanishes at both endpoints. Its [odd periodic extension](../../../../../../odd-periodic-extension.md) is continuously differentiable across the joins, whereas its [even extension](../../../../../../even-extension.md) has corners because $p'(0)=L$ and $p'(L)=-L$ are nonzero.

Two [integrations by parts](../../../../../../integration-by-parts.md), with $q=n\pi/L$, give

$$
\int_0^Lp(x)\sin(qx)\,dx=\frac{2[1-(-1)^n]}{q^3},\qquad
\int_0^Lp(x)\cos(qx)\,dx=-\frac{L[1+(-1)^n]}{q^2}.
$$

The [Fourier coefficients](../../../../../../fourier-coefficient.md) are therefore

$$
\boxed{b_n=\frac{4L^2[1-(-1)^n]}{n^3\pi^3},\qquad
 a_0=\frac{L^2}{3},\qquad
 a_n=-\frac{2L^2[1+(-1)^n]}{n^2\pi^2}.}
$$

The [Fourier sine series](../../../../../../fourier-sine-series.md) has a uniform absolute tail $O(N^{-2})$, and each of its [partial sums](../../../../../../partial-sum.md) satisfies both zero [boundary values](../../../../../../boundary-value.md) exactly. The [Fourier cosine series](../../../../../../fourier-cosine-series.md) has an absolute tail bound $O(N^{-1})$; at $x=0$ its omitted even-index [Fourier coefficients](../../../../../../fourier-coefficient.md) have the same sign and yield an error of order $N^{-1}$. This verifies a strictly faster uniform error bound for the sine approximation in this example.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
