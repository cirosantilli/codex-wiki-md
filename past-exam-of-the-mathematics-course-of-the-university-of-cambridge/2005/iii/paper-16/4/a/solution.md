<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $(X,\mathcal B,\mu)$ be a [probability space](../../../../../../probability-space.md), let $T$ be a [measure-preserving transformation](../../../../../../measure-preserving-transformation.md), and let $g\in L^1(\mu)$. The [Birkhoff ergodic theorem](../../../../../../birkhoff-ergodic-theorem.md) asserts that

$$
A_ng(x)=\frac1n\sum_{k=0}^{n-1}g(T^kx)
\longrightarrow g^*(x)=\mathbb E_\mu[g\mid\mathcal I](x)
$$

for almost every $x$, where $\mathcal I=\{B\in\mathcal B:\mu(T^{-1}B\mathbin{\triangle}B)=0\}$ is the [invariant sigma-algebra](../../../../../../invariant-sigma-algebra.md). The limit is integrable, satisfies $g^*\circ T=g^*$ almost everywhere, and has $\int g^*\,d\mu=\int g\,d\mu$. On a [probability space](../../../../../../probability-space.md) the convergence also holds in $L^1$. No invertibility of $T$ is required.

If $T$ is [ergodic](../../../../../../ergodicity.md), its [invariant sigma-algebra](../../../../../../invariant-sigma-algebra.md) is trivial modulo null sets, so its [conditional expectation](../../../../../../conditional-expectation.md) is constant. In that case the concise form is

$$
\boxed{A_ng(x)\longrightarrow\int_Xg\,d\mu\quad\text{for almost every }x.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
