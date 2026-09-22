<h1 id="23h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Rellich-Kondrashov compactness theorem for H01](../../../../../../rellich-kondrashov-compactness-theorem-for-h01.md) states that if $\Omega\subset\mathbb R^d$ is bounded and open, then the inclusion

$$
H_0^1(\Omega)\hookrightarrow L^2(\Omega)
$$

is compact: every bounded sequence in $H_0^1(\Omega)$ has a subsequence converging strongly in $L^2(\Omega)$.

Let $(u_n)$ be bounded in $H_0^1(\Omega)$. Since this is a Hilbert space, Banach--Alaoglu and reflexivity give a subsequence, still denoted $(u_n)$, and $u\in H_0^1(\Omega)$ such that $u_n\rightharpoonup u$ weakly in $H_0^1(\Omega)$ and hence in $L^2(\Omega)$. Extend all these functions by zero to $\mathbb R^d$. The zero extensions belong to $H^1(\mathbb R^d)$ and remain uniformly bounded there.

For each $\xi\in\mathbb R^d$,

$$
\widehat u_n(\xi)=\int_\Omega u_n(x)e^{-ix\cdot\xi}\,dx
\longrightarrow
\int_\Omega u(x)e^{-ix\cdot\xi}\,dx=\widehat u(\xi),
$$

because $e^{ix\cdot\xi}\mathbf1_\Omega\in L^2(\Omega)$. On each ball $|\xi|\leq R$, Cauchy--Schwarz gives a uniform bound on $|\widehat u_n-\widehat u|$, so dominated convergence yields

$$
\int_{|\xi|\leq R}|\widehat u_n-\widehat u|^2\,d\xi\longrightarrow0.
$$

The gradient bound controls high frequencies. By Plancherel,

$$
\int_{|\xi|>R}|\widehat u_n-\widehat u|^2\,d\xi
\leq \frac1{R^2}
\int_{\mathbb R^d}|\xi|^2|\widehat u_n-\widehat u|^2\,d\xi
\leq\frac C{R^2},
$$

uniformly in $n$. First choose $R$ large and then $n$ large. The low- and high-frequency estimates show $\widehat u_n\to\widehat u$ in $L^2(\mathbb R^d)$, and a final application of Plancherel gives $u_n\to u$ strongly in $L^2(\Omega)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [23H](../../23h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
