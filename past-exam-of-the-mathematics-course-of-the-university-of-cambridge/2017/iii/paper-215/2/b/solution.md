<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the real [inner product](../../../../../../inner-product.md)

$$
\langle f,g\rangle_\pi=\sum_{x\in S}\pi(x)f(x)g(x).
$$

The [stationary distribution](../../../../../../stationary-distribution.md) is strictly positive for an [irreducible Markov chain](../../../../../../irreducible-markov-chain.md). [Detailed balance](../../../../../../detailed-balance.md) gives $\langle Pf,g\rangle_\pi=\langle f,Pg\rangle_\pi$, so $P$ is a [self-adjoint operator](../../../../../../self-adjoint-operator.md). Choose a real [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) $f_1,\ldots,f_m$, where $m=|S|$, $Pf_j=\lambda_jf_j$, $f_1\equiv1$, $\lambda_1=1$, and $\pi(f_j)=0$ for $j\geq2$.

For fixed $y$, apply the [spectral decomposition](../../../../../../spectral-decomposition.md) to $g_y(z)=\mathbf1_{\{y\}}(z)/\pi(y)$. Its coefficient against $f_j$ is $f_j(y)$, whereas $(P^tg_y)(x)=P^t(x,y)/\pi(y)$. Thus the [spectral kernel expansion of a reversible chain](../../../../../../spectral-kernel-expansion-of-a-reversible-chain.md) is

$$
\boxed{\frac{P^t(x,y)}{\pi(y)}=\sum_{j=1}^{m}\lambda_j^t f_j(x)f_j(y).}
$$

This holds for all integers $t\geq0$; at $t=0$ each multiplier is one, including when $\lambda_j=0$. Negative [eigenvalues](../../../../../../eigenvalue.md) are allowed, and retain their signs for odd $t$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
