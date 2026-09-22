<h1 id="23h/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Weak convergence $u_n\rightharpoonup u$ in $H_0^1(\Omega)$ implies

$$
Du_n\rightharpoonup Du
$$

in $L^2$. The $L^2$ norm is weakly lower semicontinuous, so

$$
\int_\Omega|Du|^2
\leq\liminf_n\int_\Omega|Du_n|^2.
$$

The [Rellich-Kondrashov compactness theorem for H01](../../../../../../../rellich-kondrashov-compactness-theorem-for-h01.md) upgrades the weak convergence to

$$
u_n\longrightarrow u
$$

strongly in $L^2(\Omega)$. Indeed, compactness gives this along every subsequence after passage to a further subsequence, and the weak limit uniquely identifies every such strong limit as $u$. Consequently,

$$
\begin{aligned}
\left|\int_\Omega V(u_n^2-u^2)\right|
&\leq\lVert V\rVert_\infty
\lVert u_n-u\rVert_2
\bigl(\lVert u_n\rVert_2+\lVert u\rVert_2\bigr)\\
&\longrightarrow0.
\end{aligned}
$$

Combining the two terms proves the [weak lower semicontinuity of a bounded-domain Schrodinger energy](../../../../../../../weak-lower-semicontinuity-of-a-bounded-domain-schrodinger-energy.md):

$$
\boxed{E(u)\leq\liminf_nE(u_n)}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [23H](../../../23h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
