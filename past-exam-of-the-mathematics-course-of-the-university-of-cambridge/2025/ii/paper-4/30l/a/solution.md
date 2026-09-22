<h1 id="30l/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The candidate $\Pi$ is tacitly required to belong to $S$, as in the usual [variational characterization of convex projection](../../../../../../variational-characterization-of-convex-projection.md); this feasibility holds for the candidate constructed in part (b). Use the Frobenius inner product

$$
\langle A,B\rangle_F=\operatorname{Tr}(A^TB).
$$

For any $Z\in S$,

$$
M-Z=(M-\Pi)-(Z-\Pi),
$$

and hence

$$
\begin{aligned}
\|M-Z\|_F^2
&=\|M-\Pi\|_F^2+\|Z-\Pi\|_F^2
-2\langle M-\Pi,Z-\Pi\rangle_F\\
&\geq\|M-\Pi\|_F^2+\|Z-\Pi\|_F^2\\
&\geq\|M-\Pi\|_F^2.
\end{aligned}
$$

Thus $\Pi$ minimizes the squared Frobenius distance over $S$. Since that objective is strictly convex,

$$
\boxed{\Pi=\pi(M)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30L](../../30l.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
