<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose normalized eigenvectors $u_n$ of the finite compressions and embed them as $v_n=P_n^*u_n\in H$. Then

$$
\langle Av_n,v_n\rangle=\lambda_n.
$$

The bounded sequence $(v_n)$ has weakly convergent subsequences. If $v_{n_j}\rightharpoonup v$, then for every $y\in H$, strong convergence $P_n^*P_ny\to y$ and the compressed eigenvalue equation give

$$
\langle(A-\lambda I)v,y\rangle
=\lim_j\langle(A-\lambda_{n_j}I)v_{n_j},P_{n_j}^*P_{n_j}y\rangle=0.
$$

Because $\lambda\notin\sigma(A)$, this forces $v=0$. Every weak cluster point is zero, so $v_n\rightharpoonup0$. Since $\langle Av_n,v_n\rangle=\lambda_n\to\lambda$, the weak-null characterization gives

$$
\boxed{\lambda\in W_e(A)}.
$$

**Thus finite-section [spectral pollution](../../../../../../spectral-pollution.md) of a bounded operator can occur only in its [essential numerical range](../../../../../../essential-numerical-range.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
