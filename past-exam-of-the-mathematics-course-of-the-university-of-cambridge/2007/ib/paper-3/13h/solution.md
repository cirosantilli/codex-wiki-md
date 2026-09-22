<h1 id="13h/solution">Solution</h1>

↑ **Parent:** [13H](../13h.md)

The proposed [norm](../../../../../norm.md) is finite because every [continuous function](../../../../../continuous-function.md) on $[0,1]$ is bounded and integrable. It is nonnegative. If $\|f\|=0$ and $f(x_0)\ne0$ at some point, [continuity](../../../../../continuous-function.md) gives a nontrivial interval within $[0,1]$ on which $|f|$ is bounded below by a positive constant, contradicting the zero integral. Thus $\|f\|=0$ implies $f=0$. The converse is immediate. Absolute homogeneity follows from $|cf(x)|=|c||f(x)|$, and the pointwise inequality $|f(x)+g(x)|\leq|f(x)|+|g(x)|$ integrates to the [triangle inequality](../../../../../triangle-inequality.md). These establish **all the norm axioms**, so $V$ is a [normed vector space](../../../../../normed-vector-space.md).

To test the [Cauchy sequence](../../../../../cauchy-sequence.md) condition, compare the terms with indices $n$ and $2n$. Put $d_n(x)=\sin(nx)-\sin(2nx)$. The identities $2\sin(nx)\sin(2nx)=\cos(nx)-\cos(3nx)$ and $2\sin^2(nx)=1-\cos(2nx)$ give

$$
\begin{aligned}
\int_0^1d_n(x)^2\,dx
&=\int_0^1\sin^2(nx)\,dx+\int_0^1\sin^2(2nx)\,dx-2\int_0^1\sin(nx)\sin(2nx)\,dx\\
&=1-\frac{\sin(2n)}{4n}-\frac{\sin(4n)}{8n}-\frac{\sin n}{n}+\frac{\sin(3n)}{3n}\longrightarrow1.
\end{aligned}
$$

Because $|d_n(x)|\leq2$, we have $d_n(x)^2\leq2|d_n(x)|$. Therefore

$$
\liminf_{n\to\infty}\|f_n-f_{2n}\|\geq\frac12.
$$

In particular, for all sufficiently large $n$, these arbitrarily late pairs have [norm](../../../../../norm.md) distance greater than $1/4$. This proves the [sine sequence is not Cauchy in the integral norm](../../../../../sine-sequence-is-not-cauchy-in-the-integral-norm.md). Thus **the sequence is not Cauchy and does not converge to an element of $V$**, since every [norm convergent](../../../../../norm-convergence.md) sequence is [Cauchy](../../../../../cauchy-sequence.md). This direct separation argument does not rely on [completeness](../../../../../completeness.md) of $V$.

## ↑ Ancestors (10)

1. [13H](../13h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
