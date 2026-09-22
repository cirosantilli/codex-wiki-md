<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $n>m$, define $r_j=\lfloor j2^{m-n}\rfloor2^{-m}$ and $h_j=X_{j2^{-n}}-X_{r_j}$. Each $h_j$ is measurable at time $j2^{-n}$, so the summands in the given difference formula are orthogonal [martingale transforms](../../../../../../martingale-transform.md). Therefore

$$
\mathbb E|M_1^{(n)}-M_1^{(m)}|^2=\mathbb E\sum_{j=1}^{2^n-1}h_j^2\left(X_{(j+1)2^{-n}}-X_{j2^{-n}}\right)^2.
$$

Let

$$
\omega_m=\sup\{|X_t-X_s|:s,t\in[0,1],\ |t-s|\le2^{-m}\}.
$$

Path continuity on the compact interval gives $\omega_m\to0$ almost surely, and $\omega_m\le2C$. Since $0\le j2^{-n}-r_j<2^{-m}$, $|h_j|\le\omega_m$. Thus, by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and part (b),

$$
\mathbb E|M_1^{(n)}-M_1^{(m)}|^2\le\mathbb E[\omega_m^2A_1^{(n)}]\le\sqrt{10}\,C^2(\mathbb E\omega_m^4)^{1/2}\longrightarrow0.
$$

The last step is the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md). The bound is uniform in $n>m$, and the other ordering follows by symmetry. Hence **the terminal martingale transforms are Cauchy in $L^2$**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
