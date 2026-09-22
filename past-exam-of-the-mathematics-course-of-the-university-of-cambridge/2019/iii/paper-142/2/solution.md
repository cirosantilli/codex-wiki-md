<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For variables $x_1,\ldots,x_m$, the [elementary symmetric polynomial](../../../../../elementary-symmetric-polynomial.md) and [power-sum symmetric polynomial](../../../../../power-sum-symmetric-polynomial.md) are

$$
e_r=\sum_{1\leq i_1<\cdots<i_r\leq m}x_{i_1}\cdots x_{i_r},
\qquad
p_r=\sum_{i=1}^m x_i^r.
$$

Put $E(t)=\prod_i(1+x_it)=\sum_{r\geq0}e_rt^r$. Its logarithmic derivative is

$$
\frac{E'(t)}{E(t)}
=\sum_i\frac{x_i}{1+x_it}
=\sum_{r\geq1}(-1)^{r-1}p_rt^{r-1}.
$$

Comparing the coefficient of $t^{n-1}$ in $E'(t)=E(t)E'(t)/E(t)$ gives the [Newton identities](../../../../../newton-s-identities.md)

$$
\boxed{p_n-e_1p_{n-1}+e_2p_{n-2}-\cdots+(-1)^{n-1}e_{n-1}p_1+n(-1)^ne_n=0.}
$$

The given [Bockstein homomorphism](../../../../../bockstein-homomorphism.md) is the first Steenrod square. A real line bundle is pulled back from the universal line bundle over $\mathbb{RP}^{\infty}$, where the degree-one generator $x$ satisfies $\beta(x)=x^2$. By naturality,

$$
\boxed{\beta(w_1(L))=w_1(L)^2.}
$$

Apply the [splitting principle for real vector bundles](../../../../../splitting-principle-for-real-vector-bundles.md), writing the pulled-back bundle as $L_1\oplus\cdots\oplus L_r$ and $x_i=w_1(L_i)$. The pullback in cohomology is injective, $w_j(E)=e_j(x_1,\ldots,x_r)$, and the [Bockstein derivation rule](../../../../../bockstein-derivation-rule.md) gives

$$
\beta(e_j)=\sum_i x_i^2e_{j-1}(x_1,\ldots,\widehat{x_i},\ldots,x_r).
$$

In $e_1e_j$, the terms for which the index from $e_1$ already lies in the $j$-element subset give this sum, while each square-free monomial of degree $j+1$ occurs $j+1$ times. Over $\mathbb F_2$ this yields

$$
\boxed{\beta(w_j(E))=w_1(E)w_j(E)+(j+1)w_{j+1}(E).}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 142](../../paper-142-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
