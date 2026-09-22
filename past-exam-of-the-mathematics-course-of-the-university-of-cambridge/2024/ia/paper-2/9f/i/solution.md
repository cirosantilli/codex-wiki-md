<h1 id="9f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $Q=\sum_{j=1}^nq_j$. Since the variables have continuous distributions, the minimum is unique almost surely. Integrating over its possible value gives

$$
\begin{aligned}
\mathbb P(K=k,T\geq t)
&=\int_t^\infty q_ke^{-q_ks}
   \prod_{j\ne k}\mathbb P(S_j>s)\,ds\\
&=\int_t^\infty q_ke^{-Qs}\,ds
=\boxed{\frac{q_k}{Q}e^{-Qt}}.
\end{aligned}
$$

This is the joint tail calculation for [competing exponential clocks](../../../../../../competing-exponential-clocks.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [9F](../../9f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
