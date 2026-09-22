<h1 id="12h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\lambda\notin K$, write $g_\lambda(z)=(z-\lambda)^{-1}$. If $\lambda\in\Lambda$ and

$$
|\mu-\lambda|<\operatorname{dist}(\lambda,K),
$$

then

$$
g_\mu
=\frac{g_\lambda}{1-(\mu-\lambda)g_\lambda}
=\sum_{n=0}^{\infty}(\mu-\lambda)^ng_\lambda^{n+1}
$$

uniformly on $K$. Uniformly polynomially approximable functions form an algebra closed under uniform limits, so $\mu\in\Lambda$. Hence $\Lambda$ is open.

The set $\Lambda$ is also closed relative to $\mathbb C\setminus K$. Indeed, if $\lambda_j\in\Lambda$ and $\lambda_j\to\lambda\notin K$, then

$$
\|g_{\lambda_j}-g_\lambda\|_\infty
\leq
\frac{|\lambda_j-\lambda|}
{\operatorname{dist}(\lambda_j,K)\operatorname{dist}(\lambda,K)}
\longrightarrow0,
$$

so $g_\lambda$ is again uniformly approximable by polynomials. Since $K$ is closed, every point of $\Gamma$ has a neighbourhood in $\mathbb C\setminus K$; relative closedness of $\Lambda$ then gives a smaller neighbourhood disjoint from $\Lambda$. Thus **both $\Lambda$ and $\Gamma$ are open**.

It is not always true that $\Lambda$ is nonempty. Take $K=\mathbb R$. Any polynomial uniformly close on $\mathbb R$ to a bounded resolvent $g_\lambda$, with $\lambda\notin\mathbb R$, must itself be bounded on $\mathbb R$, and hence must be constant. Uniform limits of constants are constant, whereas $g_\lambda$ is not. Therefore

$$
\boxed{K=\mathbb R\quad\Longrightarrow\quad\Lambda=\varnothing.}
$$

Boundedness of $K$ does not force $\Gamma$ to be empty either. Take $K=\{z:|z|=1\}$ and $\lambda=0$. If polynomials $p_n$ converged uniformly to $1/z$ on $K$, then [uniform convergence and contour integration](../../../../../../uniform-convergence-and-contour-integration.md) would give

$$
0=\lim_{n\to\infty}\oint_Kp_n(z)\,dz
=\oint_K\frac{dz}{z}=2\pi i,
$$

a contradiction. Hence

$$
\boxed{K=\{z:|z|=1\}\quad\Longrightarrow\quad0\in\Gamma.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12H](../../12h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
