<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let

$$
A_k=\{\lVert S_j\rVert\leq t\text{ for }j<k, \lVert S_k\rVert>t\}
$$

be the event that the partial sums first cross level $t$ at time $k$. On $A_k$, write $R_k=S_n-S_k$. Conditional on $X_1,\ldots,X_k$, the random variable $R_k$ is independent and symmetric. Since

$$
2\lVert S_k\rVert
\leq\lVert S_k+R_k\rVert+\lVert S_k-R_k\rVert,
$$

at least one of the two norms on the right exceeds $t$. Symmetry of $R_k$ consequently gives

$$
\mathbb P(\lVert S_n\rVert>t\mid X_1,\ldots,X_k)\geq\frac12
$$

on $A_k$. The events $A_k$ are disjoint, so summation proves the [Lévy maximal inequality](../../../../../levy-maximal-inequality.md)

$$
\mathbb P\left(\max_{1\leq k\leq n}\lVert S_k\rVert>t\right)
\leq2\mathbb P(\lVert S_n\rVert>t).
$$

For the Gaussian series, put $S_m=\sum_{j=1}^mg_ju_j$. Apply the inequality to the symmetric independent increments from $n+1$ through $m$, followed by [Markov inequality](../../../../../markov-inequality.md) in squared norm:

$$
\begin{aligned}
\mathbb P\left(\max_{n<k\leq m}\lVert S_k-S_n\rVert_V>\varepsilon\right)
&\leq2\mathbb P(\lVert S_m-S_n\rVert_V>\varepsilon)\\
&\leq\frac2{\varepsilon^2}\mathbb E\lVert S_m-S_n\rVert_V^2
=\frac2{\varepsilon^2}\sum_{j=n+1}^m\lVert u_j\rVert_V^2.
\end{aligned}
$$

Here the cross terms vanish by [orthogonality of independent centered Hilbert-space random variables](../../../../../orthogonality-of-independent-centered-hilbert-space-random-variables.md). Letting $m\to\infty$ and then $n\to\infty$ shows

$$
\mathbb P\left(\sup_{k\geq n}\lVert S_k-S_n\rVert_V>\varepsilon\right)\longrightarrow0.
$$

The convergence criterion in the question now shows that $\sum_jg_ju_j$ converges almost surely in $V$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 217](../../paper-217-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
