<h1 id="16e/solution">Solution</h1>

↑ **Parent:** [16E](../16e.md)

For a [rational function](../../../../../rational-function.md), the stipulated decay implies $R(z)=O(|z|^{-2})$ at infinity, unless it vanishes identically. Thus its real-line integral converges absolutely. Close the segment $[-T,T]$ with an upper semicircle, choosing $T$ beyond all finite poles. The arc contribution has modulus at most $\pi T\sup_{|z|=T}|R(z)|=O(T^{-1})$, tending to zero. The [residue theorem](../../../../../residue-theorem.md) therefore gives

$$
\boxed{\int_{-\infty}^{\infty}R(x)\,dx=2\pi i\sum_{\operatorname{Im}z_j>0}\operatorname{Res}_{z=z_j}R(z).}
$$

There are no real poles requiring indentations.

Apply this to $R(z)=1/(1+z^{2n})$. Its upper-half-plane poles are $\zeta_k=e^{i(2k+1)\pi/(2n)}$, $k=0,\ldots,n-1$, all simple. Since $\zeta_k^{2n}=-1$, their residues are

$$
\operatorname{Res}_{\zeta_k}R=\frac1{2n\zeta_k^{2n-1}}=-\frac{\zeta_k}{2n}.
$$

For $\theta=\pi/(2n)$, the finite [geometric series](../../../../../geometric-series.md) gives

$$
\sum_{k=0}^{n-1}\zeta_k=e^{i\theta}\frac{1-e^{i\pi}}{1-e^{2i\theta}}=\frac{i}{\sin\theta}.
$$

The full real-line integral is consequently $\pi/[n\sin(\pi/(2n))]$. Its integrand is even, so **the requested half-line integral is**

$$
\boxed{\int_0^\infty\frac{dx}{1+x^{2n}}=\frac{\pi}{2n}\csc\frac{\pi}{2n}.}
$$

## ↑ Ancestors (10)

1. [16E](../16e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
