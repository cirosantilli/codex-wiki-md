<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The [L1 norm](../../../../../l1-norm.md) properties of absolute homogeneity and the [triangle inequality](../../../../../triangle-inequality.md) follow from the corresponding properties of the absolute value and the [integral](../../../../../integral.md). If $\|f\|_1=0$, the nonnegative [continuous function](../../../../../continuous-function.md) $|f|$ has zero integral. Were $|f(x_0)|>0$, continuity would make it bounded below by a positive number on a nontrivial interval, contradicting the zero integral. Thus $f=0$, proving positive definiteness.

Put $M=\|f\|_\infty$ and choose the continuous [cutoff function](../../../../../cutoff-function.md)

$$
\eta_n(x)=\min\{1,nx,n(1-x)\},\qquad g_n=\eta_n f.
$$

Then $g_n(0)=g_n(1)=0$, $\|g_n\|_\infty\leq M$, and $f-g_n$ is supported in the two endpoint intervals of total length $2/n$. Therefore

$$
\|f-g_n\|_1\leq\frac{2M}{n}\longrightarrow0.
$$

Now suppose $\int_0^1fg=0$ for every $g\in\mathcal S$. Apply this to the above $g_n$. By the [uniform norm](../../../../../supremum-norm.md) bound,

$$
0\leq\int_0^1f^2
=\int_0^1f(f-g_n)
\leq\|f\|_\infty\|f-g_n\|_1\longrightarrow0.
$$

Hence $\int_0^1f^2=0$, and continuity again gives **$f=0$.**

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
