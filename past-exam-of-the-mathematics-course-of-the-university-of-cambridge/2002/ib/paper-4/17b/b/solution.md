<h1 id="17b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Integrate $e^{iz}/z$ around the positively oriented indented upper-half-plane contour. The outer semicircle runs from $R$ to $-R$; the inner semicircle runs clockwise from $-r$ to $r$, excluding zero. The integrand is holomorphic inside this region, so [Cauchy's integral theorem](../../../../../../cauchy-s-integral-theorem.md) gives total [integral](../../../../../../integral.md) zero.

The outer arc tends to zero by part (a) with $f(z)=1/z$ and $\lambda=1$. On the inner arc $z=re^{i\theta}$, $\theta$ decreases from $\pi$ to zero, and

$$
\int_{\rm inner}\frac{e^{iz}}z\,dz=i\int_\pi^0e^{ire^{i\theta}}d\theta\longrightarrow-i\pi.
$$

The two real segments combine as

$$
\int_{-R}^{-r}\frac{e^{ix}}x\,dx+\int_r^R\frac{e^{ix}}x\,dx=2i\int_r^R\frac{\sin x}{x}\,dx.
$$

Passing to the limits gives $2iI-i\pi=0$, and hence the [Dirichlet integral](../../../../../../dirichlet-integral.md)

$$
\boxed{\int_0^\infty\frac{\sin x}{x}\,dx=\frac\pi2.}
$$

This is an ordinary conditionally convergent improper [integral](../../../../../../integral.md): the integrand tends to one at zero, and integration by parts gives a tail bounded by $2/A$ beyond $A$. The clockwise indentation sign is essential.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [17B](../../17b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
