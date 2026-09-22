<h1 id="9e/solution">Solution</h1>

↑ **Parent:** [9E](../9e.md)

A [Jordan block](../../../../../jordan-block.md) $J_m(\lambda)$ has $\lambda$ on its diagonal, ones on its superdiagonal, and zeros elsewhere. A matrix is in [Jordan normal form](../../../../../jordan-normal-form.md) when it is block diagonal with Jordan blocks.

On a block $J_m(\lambda)$, $\ker(\alpha-\lambda I)^r$ has dimension $\min(r,m)$. Its increase from $r-1$ to $r$ is one exactly when $m\geq r$. Summing over blocks proves that

$$
\boxed{\dim\ker(\alpha-\lambda I)^r-\dim\ker(\alpha-\lambda I)^{r-1}}
$$

counts the $\lambda$-blocks of size at least $r$.

If $\lambda\ne0$, the polynomial $z^2$ has nonzero derivative at $\lambda$, so

$$
\boxed{J_m(\lambda)^2\sim J_m(\lambda^2).}
$$

If $\lambda=0$, squaring the nilpotent shift separates the odd and even basis chains:

$$
\boxed{J_m(0)^2\sim J_{\lceil m/2\rceil}(0)\oplus J_{\lfloor m/2\rfloor}(0),}
$$

omitting a zero-size block.

The displayed invertible matrix preserves the subspaces spanned by $(e_1,e_4)$ and $(e_2,e_3)$. Its restrictions have characteristic polynomials $t^2-a_1a_4$ and $t^2-a_2a_3$. Since invertibility makes both products nonzero, each restriction has two distinct complex eigenvalues. Its Jordan form is therefore

$$
\boxed{\operatorname{diag}\left(\sqrt{a_1a_4},-\sqrt{a_1a_4},
\sqrt{a_2a_3},-\sqrt{a_2a_3}\right),}
$$

for either choices of the square roots.

## ↑ Ancestors (10)

1. [9E](../9e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
