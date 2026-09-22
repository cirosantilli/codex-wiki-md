<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For the unrestricted zero sequence, introduce the [Weierstrass elementary factors](../../../../../weierstrass-elementary-factor.md)

$$
E_p(u)=(1-u)\exp\left(u+\frac{u^2}{2}+\cdots+\frac{u^p}{p}\right).
$$

For $|u|\le1/2$, cancellation of the first $p$ terms of the logarithm [power series](../../../../../power-series.md) gives a [holomorphic logarithm](../../../../../holomorphic-logarithm.md) of the factor:

$$
\log E_p(u)=-\sum_{j=p+1}^\infty\frac{u^j}{j},\qquad
|\log E_p(u)|\le2|u|^{p+1}.
$$

Define the [canonical product](../../../../../canonical-product.md)

$$
f(z)=\prod_{n=1}^\infty E_n(z/z_n).
$$

Fix any compact disc $|z|\le R$. Since $|z_n|\to\infty$, eventually $|z/z_n|\le1/2$ uniformly on this disc. The tail logarithms are then bounded by $2(1/2)^{n+1}$, a summable bound independent of $z$. Their sum is [holomorphic](../../../../../complex-differentiability-at-a-point.md) by [locally uniform convergence of holomorphic functions](../../../../../locally-uniform-convergence-of-holomorphic-functions.md), and its exponential is nowhere zero. Multiplication by the finite initial product therefore gives an [entire function](../../../../../entire-function.md). Each factor has a [simple zero](../../../../../simple-zero.md) exactly at its specified $z_n$, the exponential factor has none, and a tail beginning beyond any given compact disc is nonvanishing there. Thus **$f$ has precisely the prescribed zeros and no others**, each simple, and $f(0)=1$. This proves the required existence without an assumption on $\sum_n|z_n|^{-1}$.

For the final, unheaded product request, suppose now that $\sum_n|z_n|^{-1}<\infty$. On $|z|\le R$, all sufficiently late factors have $|z/z_n|\le1/2$, so part (a) bounds their [principal complex logarithms](../../../../../principal-complex-logarithm.md) by $2R/|z_n|$. The logarithms converge absolutely and uniformly; [infinite product convergence from logarithmic tails](../../../../../infinite-product-convergence-from-logarithmic-tails.md) proves that

$$
P(z)=\prod_{n=1}^\infty(1-z/z_n)
$$

is [entire](../../../../../entire-function.md) and again has exactly the prescribed simple zeros. For its finite partial products,

$$
\prod_{n=1}^N|1-z/z_n|
\le\prod_{n=1}^N(1+|z|/|z_n|)
\le\exp\left(|z|\sum_{n=1}^N|z_n|^{-1}\right).
$$

Passing to the limit proves

$$
\boxed{|P(z)|\le e^{C|z|},\qquad C=\sum_{n=1}^\infty|z_n|^{-1}<\infty.}
$$

In particular $P$ is an [entire function of exponential type](../../../../../entire-function-of-exponential-type.md). This argument uses a valid modulus estimate and does not require the false logarithm assertion in part (c).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
