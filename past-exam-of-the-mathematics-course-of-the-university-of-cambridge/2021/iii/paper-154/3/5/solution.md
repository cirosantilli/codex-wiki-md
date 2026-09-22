<h1 id="3/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $T_2>T_1\geq-1$, the dual [Strichartz estimate for the free Schrödinger equation](../../../../../../strichartz-estimate-for-the-free-schrodinger-equation.md) gives

$$
\left\|
\int_{T_1}^{T_2}S(-s)(u_\eta|u_\eta|^2)(s)\,ds
\right\|_2
\lesssim
\|u_\eta|u_\eta|^2\|_{L^{4/3}_{t,x}([T_1,T_2])}
=\|u_\eta\|_{L^4_{t,x}([T_1,T_2])}^3.
$$

The assumed finite global $L^4_{t,x}$ norm makes the right side tend to zero as $T_1,T_2\to\infty$. The displayed family is therefore a [Cauchy sequence](../../../../../../cauchy-sequence.md) in the complete space $L^2$ and has a strong limit $F_\infty$.

The [Duhamel principle](../../../../../../duhamel-s-principle.md) gives

$$
S(-t)u_\eta(t)
=S(1)u_\eta(-1)
+i\int_{-1}^tS(-s)(u_\eta|u_\eta|^2)(s)\,ds.
$$

Define

$$
u_\eta^\infty=S(1)u_\eta(-1)+iF_\infty\in L^2.
$$

Since the free Schrödinger group is [unitary](../../../../../../unitary-connection.md),

$$
\|u_\eta(t)-S(t)u_\eta^\infty\|_2
=\|S(-t)u_\eta(t)-u_\eta^\infty\|_2\longrightarrow0.
$$

This is [scattering from a finite Strichartz norm](../../../../../../scattering-from-a-finite-strichartz-norm.md).

## ↑ Ancestors (11)

1. [5](../5.md)
2. [3](../../3.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
