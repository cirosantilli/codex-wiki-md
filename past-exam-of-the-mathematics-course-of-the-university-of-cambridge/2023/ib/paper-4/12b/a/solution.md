<h1 id="12b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Because the [matrix-valued Laplace transform](../../../../../../matrix-valued-laplace-transform.md) is taken componentwise, for every $i,j$ we have

$$
\begin{aligned}
\bigl(\mathcal L\{AB\}(s))_{ij}
&=\int_0^\infty e^{-st}\sum_{k=1}^n A_{ik}B_{kj}(t)\,dt\\
&=\sum_{k=1}^n A_{ik}\int_0^\infty e^{-st}B_{kj}(t)\,dt\\
&=\bigl(A\mathcal L\{B\}(s))_{ij}.
\end{aligned}
$$

The sum is finite and $A$ is constant, so it may be moved outside the integral. Therefore

$$
\boxed{\mathcal L\{AB\}=A\mathcal L\{B\}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12B](../../12b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
