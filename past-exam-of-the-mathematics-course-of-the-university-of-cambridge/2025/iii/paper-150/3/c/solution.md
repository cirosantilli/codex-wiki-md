<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Complete multiplicativity and absolute convergence give the [Euler product](../../../../../../euler-product.md)

$$
D_f(s)=\prod_p\left(1-\frac{f(p)}{p^s}\right)^{-1}
\qquad(\Re s>1).
$$

Set $\sigma=1+1/\log x$. Taking logarithms of absolute values and expanding the local factors gives, uniformly in real $t$,

$$
\log|D_f(\sigma+it)|
=\sum_p\frac{\Re(f(p)p^{-it})}{p^\sigma}+O(1)
=\sum_{p\leq x}\frac{\Re(f(p)p^{-it})}{p}+O(1).
$$

The prime powers with exponent at least two contribute $O(1)$; changing $p^{-\sigma}$ to $p^{-1}$ below $x$ and estimating the tail above $x$ also cost $O(1)$. By [Mertens theorem](../../../../../../mertens-theorems.md),

$$
\sum_{p\leq x}\frac{\Re(f(p)p^{-it})}{p}
=\log\log x-\mathbb D(f,n^{it};x)^2+O(1).
$$

Exponentiating yields

$$
\boxed{\left|D_f\left(1+\frac1{\log x}+it\right)\right|
\asymp(\log x)\exp\left(-\mathbb D(f,n^{it};x)^2\right).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
