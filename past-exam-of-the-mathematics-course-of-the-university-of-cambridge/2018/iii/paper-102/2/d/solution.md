<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Suppose first that $x\ne0$, and let $E$ be the real span of the [root system](../../../../../../root-system.md), of dimension equal to the [rank of a semisimple Lie algebra](../../../../../../rank-of-a-semisimple-lie-algebra.md) $\ell$. The images of the roots span $E/\mathbb R\alpha$, so select roots $\beta_1,\ldots,\beta_{\ell-1}$ whose images form a basis of this quotient.

For each $i$, take the highest endpoint $\gamma_i^+$ of the $\alpha$ [root string](../../../../../../root-string.md) through $\beta_i$, and the highest endpoint $\gamma_i^-$ of the [root string](../../../../../../root-string.md) through $-\beta_i$. By construction, $\gamma_i^\pm+\alpha$ is not a root. Moreover $\gamma_i^\pm\ne-\alpha$, since their images in $E/\mathbb R\alpha$ are nonzero. The [root-space decomposition](../../../../../../root-space-decomposition.md) and its bracket rule therefore give

$$
[\mathfrak g_{\gamma_i^\pm},x]=0.
$$

These $2(\ell-1)$ roots are distinct: their quotient images are the two signs of a basis, which are distinct. Their one-dimensional [root spaces](../../../../../../root-space.md) consequently contribute $2(\ell-1)$ independent vectors to the [Lie algebra centralizer](../../../../../../centralizer-of-an-element-of-a-lie-algebra.md).

In addition, the $\ell-1$ dimensional subspace $\ker\alpha\subset\mathfrak t$ commutes with $x$, because $[h,x]=\alpha(h)x$. The line $\mathbb Cx\subset\mathfrak g_\alpha$ also commutes with $x$. These contributions are independent by the [root-space decomposition](../../../../../../root-space-decomposition.md); in particular none of the selected endpoint roots is $\alpha$. Thus the [centralizer lower bound for a root vector](../../../../../../centralizer-lower-bound-for-a-root-vector.md) is

$$
\boxed{\dim Z_{\mathfrak g}(x)\geq2(\ell-1)+(\ell-1)+1=3\ell-2.}
$$

If $x=0$, then $Z_{\mathfrak g}(x)=\mathfrak g$. The [root system](../../../../../../root-system.md) contains the $2\ell$ distinct roots $\pm\alpha_i$, so $\dim\mathfrak g=\ell+|\Phi|\geq3\ell$, which also proves the desired inequality. The argument includes rank one, where the list of $\beta_i$ is empty.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
