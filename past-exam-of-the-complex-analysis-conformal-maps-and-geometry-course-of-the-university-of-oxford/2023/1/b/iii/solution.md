<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For an [injective](../../../../../injective-function.md) [holomorphic function](../../../../../holomorphic-function-split.md), the real [Jacobian determinant](../../../../../jacobian-determinant.md) is $|h'|^2$. The [area formula for a univalent power series](../../../../../area-formula-for-a-univalent-power-series.md), obtained by [change of variables](../../../../../change-of-variables-formula.md), is therefore

$$
\operatorname{Area}(h(r\mathbb D))=\int_{|z|<r}|h'(z)|^2\,dA(z)=\boxed{\pi\sum_{n\geq1}n|c_n|^2r^{2n}}.
$$

Indeed, insert $h'(\rho e^{i\theta})=\sum_{n\geq1}nc_n\rho^{n-1}e^{i(n-1)\theta}$. [Orthogonality](../../../../../orthogonal-vectors.md) eliminates the cross terms in the angular [integral](../../../../../integral-split.md), and radial integration gives $2\pi n^2\int_0^r\rho^{2n-1}d\rho=\pi n r^{2n}$. The [power series](../../../../../power-series.md) converges uniformly on each smaller [closed disk](../../../../../closed-disc.md), justifying the calculation for every $r<1$.

Since $|h(z)|^2=|\phi(z^2)|$, the [Koebe growth theorem](../../../../../koebe-growth-theorem.md) gives $|h(z)|\leq|z|/(1-|z|^2)$. Hence $h(r\mathbb D)$ lies in the [disk](../../../../../disk-mathematics.md) of radius $r/(1-r^2)$, so

$$
\boxed{\operatorname{Area}(h(r\mathbb D))\leq\frac{\pi r^2}{(1-r^2)^2}}.
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the complex analysis: conformal maps and geometry course of the University of Oxford](../../../../split.md)
6. [Complex analysis: conformal maps and geometry course of the University of Oxford](../../../../../complex-analysis-conformal-maps-and-geometry-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
