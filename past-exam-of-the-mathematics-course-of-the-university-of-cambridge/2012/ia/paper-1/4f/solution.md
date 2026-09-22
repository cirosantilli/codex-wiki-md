<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

The [extreme value theorem](../../../../../extreme-value-theorem.md) ensures that $M$ is finite. Since $f(x)\leq|f(x)|\leq M$ and $g(x)\geq0$, multiplication preserves the inequality. Monotonicity of the [Riemann integral](../../../../../riemann-integral.md) gives **the required bound**

$$
\boxed{\int_0^1 fg\,dx\leq M\int_0^1g\,dx.}
$$

To prove the [weighted mean value theorem for integrals](../../../../../weighted-mean-value-theorem-for-integrals.md), put $G=\int_0^1g\,dx$ and $I=\int_0^1fg\,dx$. If $G=0$, then $|I|\leq\int_0^1|f|g\,dx\leq MG=0$, so any $\alpha$ works. This includes $g\equiv0$.

If $G>0$, the [extreme value theorem](../../../../../extreme-value-theorem.md) gives $m_0=\min f$ and $M_0=\max f$. Integrating $m_0g\leq fg\leq M_0g$ gives $m_0\leq I/G\leq M_0$. A [continuous function](../../../../../continuous-function.md) on an interval takes every value between its minimum and maximum by the [intermediate value theorem](../../../../../intermediate-value-theorem.md). Choose $\alpha$ with $f(\alpha)=I/G$. Consequently

$$
\boxed{\int_0^1fg\,dx=f(\alpha)\int_0^1g\,dx\quad\text{for some }\alpha\in[0,1].}
$$

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
