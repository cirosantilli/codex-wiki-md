<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Stationarity gives $H(X_n)=H(X_{n+1})=H(X_1)$. The Markov relation $X_1\to X_n\to X_{n+1}$ and the [data processing inequality for mutual information](../../../../../../data-processing-inequality.md) imply

$$
I(X_1;X_{n+1})\leq I(X_1;X_n).
$$

Using $H(X_n\mid X_1)=H(X_n)-I(X_1;X_n)$ on both sides gives

$$
\boxed{H(X_{n+1}\mid X_1)\geq H(X_n\mid X_1).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
