<h1 id="23f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Regard the [space of continuous functions vanishing at infinity](../../../../../../space-of-continuous-functions-vanishing-at-infinity.md) $C_0(\mathbb R^n)$ as a subspace of $L^\infty(\mathbb R^n)$. Point evaluation at the origin,

$$
\ell_0(f)=f(0),
$$

is a bounded linear functional of norm one on this subspace because a continuous function's supremum and essential supremum agree. By the [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md), $\ell_0$ extends to a bounded linear functional

$$
\ell:L^\infty(\mathbb R^n)\longrightarrow\mathbb C.
$$

Suppose that some $g\in L^1(\mathbb R^n)$ represented this extension:

$$
\ell(f)=\int_{\mathbb R^n}f(x)g(x)\,dx.
$$

Choose $\varphi\in C_c(\mathbb R^n)$ with $0\leq\varphi\leq1$, $\varphi(0)=1$, and support in the unit ball, and set $\varphi_k(x)=\varphi(kx)$. Then $\ell(\varphi_k)=1$ for every $k$. On the other hand, $\varphi_k(x)\to0$ for almost every $x$ and $|\varphi_k g|\leq|g|$. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives

$$
\int\varphi_k(x)g(x)\,dx\longrightarrow0,
$$

a contradiction. Thus $\ell$ is a [singular functional on L infinity](../../../../../../singular-functional-on-l-infinity.md) and has no $L^1$ density.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [23F](../../23f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
