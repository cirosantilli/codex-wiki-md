<h1 id="23f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $s>\tfrac12$, the [Sobolev trace theorem](../../../../../../sobolev-trace-theorem.md) states that the restriction map initially defined on smooth functions extends uniquely to a bounded linear operator

$$
\gamma:H^s(\mathbb R^n)
\longrightarrow H^{s-1/2}(\mathbb R^{n-1}),
\qquad
(\gamma u)(x')=u(x',0).
$$

Take first $u$ in the [Schwartz space](../../../../../../schwartz-space.md). Up to the harmless constant determined by the [Fourier transform](../../../../../../fourier-transform.md) convention,

$$
\widehat{\gamma u}(\xi')
=\int_{\mathbb R}\widehat u(\xi',\xi_n)\,d\xi_n.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), with weights $1+|\xi'|^2+\xi_n^2$, gives

$$
\begin{aligned}
|\widehat{\gamma u}(\xi')|^2
&\leq
\left(\int_{\mathbb R}
(1+|\xi'|^2+\xi_n^2)^s
|\widehat u(\xi',\xi_n)|^2\,d\xi_n\right)\\
&\quad\times
\left(\int_{\mathbb R}
(1+|\xi'|^2+\xi_n^2)^{-s}\,d\xi_n\right).
\end{aligned}
$$

After the substitution $\xi_n=(1+|\xi'|^2)^{1/2}t$, the second factor is

$$
C_s(1+|\xi'|^2)^{1/2-s},
\qquad
C_s=\int_{\mathbb R}(1+t^2)^{-s}\,dt<\infty,
$$

where finiteness is exactly the condition $s>1/2$. Multiplying by $(1+|\xi'|^2)^{s-1/2}$ and integrating in $\xi'$ yields

$$
\lVert\gamma u\rVert_{H^{s-1/2}(\mathbb R^{n-1})}
\leq C_s^{1/2}\lVert u\rVert_{H^s(\mathbb R^n)}.
$$

Density of the Schwartz space in the [Sobolev space](../../../../../../sobolev-space-split.md) completes the unique bounded extension.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [23F](../../23f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
