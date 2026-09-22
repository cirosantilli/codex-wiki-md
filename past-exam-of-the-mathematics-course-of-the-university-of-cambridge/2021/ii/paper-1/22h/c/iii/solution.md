<h1 id="22h/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume (iii), and let $\delta>0$. Choose $I$ such that

$$
\sum_{i\geq I}|\langle x_n,e_i\rangle|^2<\delta
$$

for every $n$. Coordinate convergence implies, for every finite $J\geq I$,

$$
\sum_{i=I}^J|\langle x_\infty,e_i\rangle|^2
=\lim_{n\to\infty}
\sum_{i=I}^J|\langle x_n,e_i\rangle|^2
\leq\delta.
$$

Letting $J\to\infty$ shows that the corresponding tail of $x_\infty$ is also at most $\delta$.

By the [Parseval identity for a Hilbertian basis](../../../../../../../parseval-identity-for-a-hilbertian-basis.md),

$$
\begin{aligned}
\|x_n-x_\infty\|^2
&=\sum_{i<I}
|\langle x_n-x_\infty,e_i\rangle|^2\\
&\quad+\sum_{i\geq I}
|\langle x_n-x_\infty,e_i\rangle|^2.
\end{aligned}
$$

The finite first sum tends to zero by weak coordinate convergence, while the second is at most

$$
2\sum_{i\geq I}|\langle x_n,e_i\rangle|^2
+2\sum_{i\geq I}|\langle x_\infty,e_i\rangle|^2
\leq4\delta.
$$

Since $\delta$ is arbitrary, $\|x_n-x_\infty\|\to0$. Thus (iii) implies (i), completing the equivalence and proving the [uniform basis-tail criterion for strong convergence](../../../../../../../uniform-basis-tail-criterion-for-strong-convergence.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [22H](../../../22h.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
