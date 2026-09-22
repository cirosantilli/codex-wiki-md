<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $t$. Uniform continuity of the sample path on $[0,t]$ gives

$$
\delta_n(t)=\max_k|X_{t\wedge t_k^n}-X_{t\wedge t_{k-1}^n}|\longrightarrow0.
$$

Since $p<2$,

$$
A_t^{(n)}
=\sum_k|\Delta_k^nX|^2
\leq\delta_n(t)^{2-p}B_t^{(n)}.
$$

The assumed pathwise boundedness of $\sup_nB_t^{(n)}$ makes the right-hand side tend to zero almost surely. Part (b) also gives $A_t^{(n)}\to A_t$ in probability, so uniqueness of limits in probability yields $A_t=0$ almost surely. The vanishing-quadratic-variation result from part (a), after localization, makes $X$ identically zero. Consequently every $B_t^{(n)}$ is zero and $\sup_nB_t^{(n)}=0$ almost surely.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
