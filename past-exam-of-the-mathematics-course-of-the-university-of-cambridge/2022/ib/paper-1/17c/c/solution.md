<h1 id="17c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The constant is sharp because continuous functions bounded by one can approximate $\operatorname{sgn}K$ arbitrarily closely outside an arbitrarily small interval around zero. Choose $f'''$ to be such an approximation and integrate three times to obtain $f\in C^3[-1,1]$. Then

$$
\frac{|L(f)|}{\|f'''\|_\infty}
=\frac{\left|\int K(t)f'''(t)\,dt\right|}
{\|f'''\|_\infty}
\longrightarrow\int_{-1}^1|K(t)|\,dt=\frac13.
$$

**No smaller constant can therefore satisfy the inequality for every $f$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17C](../../17c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
