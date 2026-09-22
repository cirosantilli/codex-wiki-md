<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix a sample path on the probability-one event where $X$ is continuous and the [total-variation process](../../../../../../total-variation-process.md) of $A$ satisfies $V_\infty\leq K$. The signed measure $dA$ has absolute variation measure $dV$. Thus

$$
\sup_{t\geq0}\left|\int_0^t\bigl(f_n'(X_s)-\operatorname{sgn}_-(X_s)\bigr)dA_s\right|\leq\int_0^\infty|f_n'(X_s)-\operatorname{sgn}_-(X_s)|dV_s.
$$

The integrand tends to zero at every time, including times when $X_s=0$, and is bounded by $2$. Since $dV$ is a finite measure on this path, the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) makes the right-hand side tend to zero. Therefore

$$
\boxed{\int_0^t f_n'(X_s)dA_s\longrightarrow\int_0^t\operatorname{sgn}_-(X_s)dA_s\quad\text{almost surely for every }t\geq0\text{ simultaneously}.}
$$

In fact the convergence is uniform over the entire time axis under the given total-variation bound. This pathwise estimate establishes one common full-probability event, rather than separate exceptional events for each time.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
